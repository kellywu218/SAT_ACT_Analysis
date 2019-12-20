# Project 1: SAT & ACT Analysis

## Problem Statement

With the continuously advancing society we live in, the minimum requirements and qualifications for job positions is increasing. In addition to relevant field experience, many positions are beginning to add in a college education as a minimum; some are even adding in a continued education as a minimum. So when looking at higher education institutions, we notice that there is an application requirement known as the SAT or ACT, which are exams that measure a person's readiness for college. 

The learning curve is different for everyone, no matter what. We have those who grasp new concepts and material immediately, those who remain bewildered despite countless hours of studying, and those who fall somewhere in between the two. Almost all of the states in the U.S. have adopted what are known as the common core standards - the basics of what you should know and takeaway from English, Math, History, and Science during each grade - that way the national curriculum and performance should be relatively the same. With this logic, academic performance should be generally equal across states and individuals, right? 

Unfortunately, it isn't. With data collected from College Board and ACT, Inc., we will try to identify any major factors that may have contributed to performances on the SAT and ACT in 2017 and 2018. Ultimately, conclude a general statement that can explain what we notice and create recommendations on how to close any found gaps. 

## Executive Summary

We took the individual datasets and began with cleaning it up to ensure that all the data was accurate and efficient to work with when comparing different variables such as participation rates and overall exam scores. Upon arriving at a polished data set, we were able to view statistics of each state in the U.S. (including the District of Columbia) regarding participation, overall scores, and test section scores. 

|Feature|Type|Dataset|Description|
|---|---|---|---|
|State|Object|2017 ACT/2017 SAT|50 States of the US and District of Columbia| 
|Participation|Float|2017 ACT/2017 SAT|The participation rate of each state for the ACT/SAT|
|SAT Reading and Writing|Integer|2017 SAT|Each state's average reading and writing score (On a scale of 200 to 800)|
|SAT Math|Integer|2017 SAT|Each state's average math score (On a scale of 200 to 800)|
|SAT Total|Integer|2017 SAT|Each state's total score of the average reading and writing and math (On a scale of 400 to 1600)|
|ACT English|Float|2017 ACT|Each state's average english score (On a scale of 1 to 36)|
|ACT Math|Float|2017 ACT|Each state's average math score (On a scale of 1 to 36)|
|ACT Reading|Float|2017 ACT|Each state's average reading score (On a scale of 1 to 36)|
|ACT Science|Float|2017 ACT|Each state's average science score (On a scale of 1 to 36)|
|ACT Total|Float|2017 ACT|Each state's average total score of all four sections (On a scale of 1 to 36)|

Through exploratory analysis, the data yielded nothing significant that required immediate attention. Participation was notable as the SAT participation rates in 2017 and 2018 were significantly lower than the ACT participation rates in 2017 and 2018 - more than double. This does pose interest given the following differences between the two exams: 

- SAT is a longer exam (by about 10 minutes when opting for the essay)
- ACT has more questions (61 more questions than the SAT)
- ACT costs more ($3 more than the SAT or 2.50 more when opting for the essay)

Given these three factors, the SAT would seem more appealing than the SAT, but the ACT had significiantly higher national participation rates than the SAT. Based on this line of interest, we delved into correlations between years and other variables like overall score. For 2017, SAT participation and SAT total scores have almost a perfect negative correlation meaning that a state with a higher participation rate had a lower total score. However, for 2018, the correlation between the two are almost perfectly positive meaning that a state with a higher participation rate had a higher total score. On the other hand, when we looked at the correlation between participation and composite score for the ACT, both years yielded near perfect negative correlations. 

Given some interesting relationships, we dived deeper into looking at signficant states. In this case, Maine, Minnesota, and the District of Columbia were analyzed. 

- District of Columbia has one of the highest SAT participation rates, but has the lowest total score in both 2017 and 2018. 

- Minnesota has one of the lowest SAT participation rates, but has the highest total score in both 2017 and 2018. 

- Maine has the lowest ACT participation rates and the highest ACT Composite Scores in both 2017 and 2018 - well above the national average.

After comparing multiple variables from the datasets about the 2017 and 2018 SAT and ACT, we can conclude that participation rates don't truly affect the overall score. While SAT participation rates are generally on the lower side versus ACT participation rates which were generally on the upper side, looking at the individual distributions of the overall scores, the SAT and ACT fell in the middle. 

Upon more in-depth research as to what factors may contribute to these results, we came across racial demographics. From what we noticed through exploring the data, the following were noted: 

- District of Columbia has one of the highest SAT participation rates, but has the lowest total score in both 2017 and 2018. 

- Minnesota has one of the lowest SAT participation rates, but has the highest total score in both 2017 and 2018. 

- Maine has the lowest ACT participation rates and and the highest ACT Composite Scores in both 2017 and 2018 - well above the national average.

## Conclusions and Recommendations

Based on racial/ethinic breakdowns, it can be seen that test takers from Minnesota and Maine were mostly White (about 60% to 70% across 2017 and 2018) while a fraction of those test takers were African Americans and Latinos (about 5% to 10% across 2017 and 2018). Furthermore, looking at the racial breakdown of test takers in the District of Columbia, most were African American (about 60% to 70% across 2017 and 2018) while a fraction of total test takers were White (about 15% across 2017 and 2018). 

It's difficult to say why there is such a large gap between academic performance and race as many factors can contribute such as finances for SAT/ACT prep classes or the accessibility to SAT/ACT resources (at school and outside of school). The data also doesn't explain as to why the ACT participation is much higher than the SAT. However, based on research on the exams, the ACT does seem more appealing to STEM individuals as a calculator is allowed on all math questions and there is less reading comprehension involved. 

In order to promote SAT participation, some ways to entice potential test takers are: 

- Hosting the exam on a school day as this can prevent any part-time job conflicts and also allow students to maintain that 5 day school week instead of having a "6 day school week." 

- Consulting with Boards of Education in regards to providing classes or electives that are centered around SAT prep in school.

## Source Documentations

1. [2017 SAT for DC](https://reports.collegeboard.org/pdf/2017-district-columbia-sat-suite-assessments-annual-report.pdf)

2. [2018 SAT for DC](https://reports.collegeboard.org/pdf/2018-district-columbia-sat-suite-assessments-annual-report.pdf)

3. [2017 SAT for Minnesota](https://reports.collegeboard.org/pdf/2017-minnesota-sat-suite-assessments-annual-report.pdf)

4. [2018 SAT for Minnesota](https://reports.collegeboard.org/pdf/2018-minnesota-sat-suite-assessments-annual-report.pdf)

5. [2017 ACT for Maine](https://www.act.org/content/dam/act/unsecured/documents/cccr2017/Maine-CCCR-2017-Final.pdf)

6. [2018 ACT for Maine](https://www.act.org/content/dam/act/unsecured/documents/cccr2018/Maine-CCCR-2018.pdf)

7. [DC Demographics](http://worldpopulationreview.com/states/district-of-columbia-population/)

8. [Minnesota Demographics](http://worldpopulationreview.com/states/minnesota-population/)

9. [Maine Demographics](http://worldpopulationreview.com/states/maine-population/)

10. [California Healthy Kids Survey WestEd](https://data.calschls.org/resources/FACTSHEET-9.pdf)

11. [ACT College Readiness](https://www.act.org/content/dam/act/unsecured/documents/National-CCCR-2019.pdf)

12. [How Students View Learning](http://www.sedl.org/change/issues/issues53.html)

13. [What Teens Want From School](https://fordhaminstitute.org/national/commentary/what-teens-want-their-schools)

14. [SAT vs ACT](https://www.usnews.com/education/best-colleges/articles/act-vs-sat-how-to-decide-which-test-to-take)











