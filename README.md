
## Problem Statement
### Context:
The SAT and ACT are standardized tests that many colleges and universities in the United States require for their admissions process. This score is used along with other materials such as grade point average (GPA) and essay responses to determine whether or not a potential student will be accepted to the university.

Standardized tests have long been a controversial topic for students, administrators, and legislators. Since the 1940's, an increasing number of colleges have been using scores from sudents' performances on tests like the SAT and the ACT as a measure for college readiness and aptitude ([*source*](https://www.minotdailynews.com/news/local-news/2017/04/a-brief-history-of-the-sat-and-act/)). Supporters of these tests argue that these scores can be used as an objective measure to determine college admittance. Opponents of these tests claim that these tests are not accurate measures of students potential or ability and serve as an inequitable barrier to entry. Lately, more and more schools are opting to drop the SAT/ACT requirement for their Fall 2021 applications ([*read more about this here*](https://www.cnn.com/2020/04/14/us/coronavirus-colleges-sat-act-test-trnd/index.html)).

### The Problem:
While the many studies that have called into question the usefulness of standardized testing as a measure of student potential and ability have their merits, as long as these tests remain one of the primary tools that colleges and universities employ to evaluate student achievement, we cannot neglect to expolore the most promising aveneues for making these measures more equitable and more representative of student potential. One of the primary ways that policy makers can approach this question is by analyzing the relationships between public funding and student achievement. 

I am seeking to explore whether there are general trends that exist between public spending on education and welfare and student achievement on the SAT and ACT. Does higher per capita spending on education translate to higher average test scores, especially in the states that consistently perform at the lowest levels? Does public welfare spending per capita follow a similar trend? Is either education or public welfare more closely aligned with student achievement? And, given the trends analyzed above, where would resources be most effectively allocated to conduct further research into improving student achievement for the most disadvantaged students?

background research and inspiration for this project: https://www.law.upenn.edu/live/files/8924-44americaneconomist81pdf

## Description of Data
### Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|**state**|object|SAT Scores 2017-2019|U.S. State with year of observations appended to the end| 
|**participation_sat**|float|SAT Scores 2017-2019|The percentage of graduating students in a given state who took the SAT| 
|**total_sat**|int|SAT Scores 2017-2019|The average total ACT score for students in a given state in a given year| 
|**participation_act**|float|ACT Scores 2017-2019|The percentage of graduation students in a given state who took the ACT| 
|**composite_act**|float|ACT Scores 2017-2019|The average composite ACT score for students in a given state in a given year| 
|**state_spending_education**|float|State and Local Education Spending 2017-2019|State education spending per capita for a given year| 
|**local_spending_education**|float|State and Local Education Spending 2017-2019|Local education spending per capita for a given year in a given state| 
|**state_and_local_spending_education**|float|State and Local Education Spending 2017-2019|Sum of state and local education spending for a given year| 
|**state_spending_welfare**|float|State and Local Education Spending 2017-2019|State spending on public welfare per capita in a given year| 
|**local_spending_welfare**|float|State and Local Education Spending 2017-2019|Local spending on public welfare per capita for a given state in a given year| 
|**state_and_local_spending_welfare**|float|State and Local Education Spending 2017-2019|Sum of state and local welfare spending per capita in a given year| 
|**total_education_and_welfare_spending**|float|State and Local Education Spending 2017-2019|Total education and welfare spending per captia for a given state in a given year| 

**State and Local Welfare/Education Spending data was sourced from:**
https://www.usgovernmentspending.com/compare_state_spending_2017b40a

#### I found a clear negative relationship between participation and test scores
![](/images/scatter_act_participation_and_scores.png)

#### But among high participation testing states, data was more normally distributed and this useful for drawin insights
![](/images/distribution_of_avg_act_scores.png)


#### The most interesting insight was the more than 1 standard deviation difference between high participation states with high and low welfare spending.
![](/images/act_scores_top_bottom_50%25_wf_spending.png)
Average ACT Score (Participation > 75%)
**19.75**

Average ACT Score High Welfare Spending
**20.29**

Average ACT Score Low Welfare Spending
**19.24**




## Conclusions and Recommendations
* The clearest relationship that needs to be explored further is the relationship betwen participation rates and test scores. One can speculate that high acheiving students are more likely to go out of their way to take a test that is not required of them or strongly recommended in hopes of gaining access to a more competitive post-secondary education. Alternatively it may be the case that low income students are less likely to be made aware of fee waivers for tests that are not either required or strongly encouraged. It is likely a combination of these and other underlying factors that explain this phenomenon, but this would be a promising avenue for future research. 
* The states that ranked in the top 50% in welfare spending per capita had average test scores of roughly 1 standard deviation higher on average than states in the bottom 50% of welfare spending per capita. Education spending per capita yeilded similar results with slightly less than 1 standard deviation difference between high participation states in the top and bottom 50% of per capita spending.
* There is support in this analysis to suggest that public welfare spending is at least as effective as education spending in its positive impact on test scores, but the findings do not suggest that one has a significantly stronger positive relationship with test scores than the other. Further research needs pursuing on the effect of different kinds of welfare spending on student achievement and what balances of education and welfare spending correspond with the greatest increase in test scores among the lowest acheiving students. 

## Next Steps
* The trends in the coming 5 plus years of universities deciding to either forgo testing or continue to use standardized tests as indicators of future student achievement will likely determine the utility of further research into public welfare and education spending on SAT and ACT scores. The low participation rates in many states already cause difficulty in extracting useful insights into how changes in environmental factors influence student test scores. A continued decrease in test participation would likely make it disproportionately more difficult to gain insight into how to improve the achievement of the most disadvantaged students, as they appear to be more likely not to participate. 
* Given the controversies that exist around questions of education funding, public welfare programs specifically aimed at improving living conditions and indirectly improving student achievement may be a creative avenue for public fund allocation that may be more likely to gain a broader base of support across party and ideological lines and make it more likely that the most disadvantaged students benefit directly from these fund reallocations.
