# Pisa Dataset Exploration
## by Ayse Isin Budak
 
 
## Introduction
***
This project is completed under Udacity Data Analyst Nanodegree program and focused on performing an exploratory data analysis and creating visualizations using seaborn & matplotlib.
 
PISA 2012 results will be analyzed in this notebook. PISA is a "survey of students' skills and knowledge as they approach the end of compulsory education.
 
Throughout the course of my project I  questioned average scores, general mood of students, presence of parents, relationship/correlation among scores, presence of parents and general mood of students.
 
 
 
## Dataset
***
This dataset includes 635  columns, I will be limiting my exploration on scores, the general mood of students, and presence of parents. I limited my dataset to dimensions & measures listed below:
 
- Student Id 
- Math Score
- Reading Score
- Science Score
- Mother Present
- Father Present
- Feel Like Outsider
- Feel Lonely at School
- Feel Happy at School
 
 
 
 
 
 
## Summary of Findings
***
 
- Test scores for all the fields are normally distributed centering around 500.
- 277.8k students' both parents are present. %17.4 of the students either have a single parent or none of the parents is present.
- It is observed that the loss of a parent has a negative effect on scores. The average score distribution of students who lost both parents is the lowest and lower scores are consistent over different subjects.
-  Variability in average scores is highest when only father is present. 
- Students mostly strongly disagrees to feel like an outsider and feel lonely.
- Most of the students agree on feeling happy at school.
- Feeling outsider and feeling lonely has a negative but insignificant correlation with scores.
- Students who strongly disagrees and who strongly agrees to feel happy at school has lower scores. 
- We observed that out of 276K students, most of the students agrees to feel happy at school and more than 60K of them scores between 450 and 550.
- We understand student who feels lonelier and outsider has lower average scores regardless of the presence of parents. Also, the loss of a parent has a negative effect on average results. Which was also observed above.
 
 
 
## Key Insight for  the Presentation
***
Using the findings, I summarized above, I tried to highlight the following findings in my presentation:
 
- Student who has both parents present are the most successful on average. Average scores in decreasing order: Both parents are present, only mother present, only father present, none of the parents is present.
- Students who have felt lonelier or feel more like an outsider has lower grades. However, there is no direct correlation found with average grades and how happy they feel.
 
--



```python

```
