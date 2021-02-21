## Overview

For our first project, we're going to take a look at aggregate SAT and ACT scores and participation rates in the United States. We'll seek to identify trends in the data and combine our data analysis with outside research to address our problem statement.

The SAT and ACT are standardized tests that many colleges and universities in the United States require for their admissions process. This score is used along with other materials such as grade point average (GPA) and essay responses to determine whether or not a potential student will be accepted to the university.

The SAT has two sections of the test: Evidence-Based Reading and Writing and Math ([*source*](https://www.princetonreview.com/college/sat-sections)). The ACT has 4 sections: English, Mathematics, Reading, and Science, with an additional optional writing section ([*source*](https://www.act.org/content/act/en/products-and-services/the-act/scores/understanding-your-scores.html)). They have different score ranges, which you can read more about on their websites or additional outside sources (a quick Google search will help you understand the scores for each test):
* [SAT](https://collegereadiness.collegeboard.org/sat)
* [ACT](https://www.act.org/content/act/en.html)

Standardized tests have long been a controversial topic for students, administrators, and legislators. Since the 1940's, an increasing number of colleges have been using scores from sudents' performances on tests like the SAT and the ACT as a measure for college readiness and aptitude ([*source*](https://www.minotdailynews.com/news/local-news/2017/04/a-brief-history-of-the-sat-and-act/)). Supporters of these tests argue that these scores can be used as an objective measure to determine college admittance. Opponents of these tests claim that these tests are not accurate measures of students potential or ability and serve as an inequitable barrier to entry.

---

### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|string|act_sat|The USA's state at which the ACT/SAT tests were recorded.|
|act_participation_17|float|act_sat|Proportion of students who attend the ACT in 2017, '1.0' being 100%.|
|act_composition_17|float|act_sat|ACT's average compository score in 2017. This can range from 0.0 to 36.0.|
|act_participation_18|float|act_sat|Proportion of students who attend the ACT in 2018, '1.0' being 100%.|
|act_composition_18|float|act_sat|ACT's average compository score in 2018. This can range from 0.0 to 36.0.|
|act_participation_19|float|act_sat|Proportion of students who attend the ACT in 2019, '1.0' being 100%.|
|act_composition_19|float|act_sat|ACT's average compository score in 2019. This can range from 0.0 to 36.0.|
|sat_participation_17|float|act_sat|Proportion of students who attend the SAT in 2017, '1.0' being 100%.|
|sat_english_17|int|act_sat|Average SAT English scores in 2017|
|sat_math_17|int|act_sat|Average SAT Math scores in 2017|
|sat_total_17|int|act_sat|Average combined Math and English scores in 2017|
|sat_participation_18|float|act_sat|Proportion of students who attend the SAT in 2018, '1.0' being 100%.|
|sat_english_18|int|act_sat|Average SAT English scores in 2018|
|sat_math_18|int|act_sat|Average SAT Math scores in 2018|
|sat_total_18|int|act_sat|Average combined Math and English scores in 2018|
|sat_participation_19|float|act_sat|Proportion of students who attend the SAT in 2019, '1.0' being 100%.|
|sat_english_19|int|act_sat|Average SAT English scores in 2019|
|sat_math_19|int|act_sat|Average SAT Math scores in 2019|
|sat_total_19|int|act_sat|Average combined Math and English scores in 2019|

---

### Datasets

The data sets used in this project:

* [`act_2017.csv`](./data/act_2017.csv): 2017 ACT Scores by State
* [`act_2018.csv`](./data/act_2018.csv): 2018 ACT Scores by State
* [`act_2019.csv`](./data/act_2019.csv): 2019 ACT Scores by State
* [`sat_2017.csv`](./data/sat_2017.csv): 2017 SAT Scores by State
* [`sat_2018.csv`](./data/sat_2018.csv): 2018 SAT Scores by State
* [`sat_2019.csv`](./data/sat_2019.csv): 2019 SAT Scores by State

---

### My Analysis

### Participation

ACT participation rate decreases every year ~-3.60% ~-3.12
SAT participation rate increases every year ~5.94% ~3.31%
NOTE: ACT has extremely high participation rate in 2017, while SAT has very low participation rate across many states Their Mean: ACT: 65.92%, SAT: 38.6% States that have high participation rate on the SAT tends to have low participation rate on the ACT and vice versa

2017:
ACT Highest: Alabama, Kentucky, Wisconsin, Utah, Tennessee, South Carolina, Oklahoma, North Carolina, Nevada, Missouri, Mississippi, Minnesota, Louisiana, Montana, Wyoming, Arkansas, Colorado
ACT Lowest: Pennsylvania, Rhode Island, New Hampshire, Delaware, Maine
SAT Highest: Michigan, Connecticut, Deleware, New Hampshire, Maine
SAT Lowest: Lowa, Mississippi, North Dekota
NOTE: SAME TREND AS 2017, note that ACT has many states that have 100% act participation. Significant increase in SAT participation rate Their Mean: ACT: 62.32%, SAT: 44.82%

2018:
ACT Highest: Alabama, Kentucky, Wisconsin, Utah, Tennessee, South Carolina, Oklahoma, Ohio, North Carolina, Nevada, Nebraska, Missouri, Mississippi, Louisiana, Montana, Wyoming, Arkansas,
ACT Lowest: Michigan, Pennsylvania, Delaware, New Hampshire, Rhode Island, Maine
SAT Highest: Colorado, Connecticut, Delaware, Michigan, Idaho, Maine, Illinois, Rhode Island, New Hampshire
SAT Lowest: Nebraska, Mississippi, South Dakota, Iowa, Wisconsin, Wyoming, North Dakota
NOTE: SAME TREND AS 2018, ACT decrease in participation rate. More States have 100% participation rate on the SAT Their Mean: ACT: 59.2%, SAT: 48.16%

2019:
ACT Highest: Alabama, Kentucky, Wisconsin, Utah, Tennessee, Oklahoma, Ohio, North Carolina, Nevada, Nebraska, Mississippi, Louisiana, Montana, Wyoming, Arkansas, North Dakota, Minnesota
ACT Lowest: Michigan, Pennsylvania, New Hampshire, Delaware, Rhode Island, Maine
SAT Highest: Michigan, Colorado, Connecticut, Delaware, Florida, Idaho, Illinois, Rhode Island, West Virginia, Maine, New Hampshire
SAT Lowest: Nebraska, Mississippi, South Dakota, Iowa, Wisconsin, Wyoming, North Dakota

ACT
100% most states maintain 100% rate except South Carolina, Missouri, and Minnesota with minor decrease in participation rate. However, Colorado had a massive decline in participation rate
SAT
100% Participation rate states (Michigan, Connecticut, Delaware) maintain 100% rate every year


### Performance

No significant changes in student's performance in either test
2017:
ACT Highest: New Hampshire, Massachusetts, Connecticut, Maine, New York
ACT Lowest: North Carolina, Hawaii, South Carolina, Mississippi, Nevada
SAT Highest: Minnesota, Wisconsin, Iowa,Missouri, Kansas
SAT Lowest: Florida, Maine, Idaho, Michigan, Delaware
2018:
ACT Highest: Connecticut, Massachusetts, New Hampshire, New York, Michigan
ACT Lowest: Alabama, Hawaii, Mississippi, South Carolina, Nevada
SAT Highest: Minnesota, Wisconsin, North Dakota, Iowa, Kansas
SAT Lowest: Utah, Hawaii, Idaho, West Virginia, Delaware
2019:
ACT Highest: Connecticut, Massachusetts, New Hampshire, Rhode Island, New York
ACT Lowest: Alabama, South Carolina, Louisiana, Mississippi, Nevada
SAT Highest: Minnesota, Wisconsin, South Dakota, North Dakota, Nebraska
SAT Lowest: Rhode Island, Idaho, Delaware, Oklahoma, West Virginia
NOTE: The best and the worst performing states tends to be consistant thorughout each year

### College Admission

ACT
California Institute of Technology
Massachusetts Institute of Technology
Johns Hopkins University
Northwestern University
Carnegie Mellon University

SAT
Harvey Mudd College
Washington University in St. Louis
Harvard College
Yale University
Johns Hopkins University

### Sorted by District (CA)

ACT: HIGHTEST SCORING DISTRICT (CALIFORNIA)
Fremont Union High
Fremont Unified
Los Gatos-Saratoga Joint Union High
Anaheim Union High
ACT: LOWEST SCORING DISTRICT (CALIFORNIA)
Fontana Unified
Los Angeles Unified
San Francisco Unified
Oakland Unified

### Conclusion/Suggestion

Most states are heavily leaning towards only one test. The support and resources that the students are receiving is on one of the two tests. This can be problematic for students who are can perform better on test that the state didn’t mandate.
Based on the data, it is suggested that students should be given the opportunity to take both tests, due to differing strengths and weaknesses of each individual student.
