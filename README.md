# School_District_Analysis_Challenge

## Overview of the school district analysis: Explain the purpose of this analysis.
A school district asked for a snapshot of several key metrics by each school campus and by the district level.  The main analysis focused on the performance of math and reading scores disaggregated several ways in preparation for a board meeting.  However, after the school board reviewed the data, it was determined that the data from Thomas High School's 9th grade class was suspect of cheating.  The school board asked for the data to be removed and analyzed again for a comparison. 

## PythonData Environment
Anaconda version 1.7.2
Conda version 4.9.0
Jupyter-Notebook version 6.1.4
ipykernal version 5.3.4
Python version 3.7.7
Pandas version 1.1.3
Numpy version 1.19.1
GitBash version 2.28.0.windows.1

## Results: Using bulleted lists and images of DataFrames as support, address the following questions.

### How is the district summary affected?
Original Analysis:
![Pic 1](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/1_dist_sum_2_decimals.PNG)

The testing data of 461 9th graders at Thomas High School was turned into null data, which recalculated the percents of passing math, passing reading, and the overall passing.  The total count of students did not change as that was run on the count of the student ids, which was not turned into null data. 

Adjusted Analysis:
![Pic 2](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_dist_sum_2_decimals.PNG)

When comparing the two charts, removing less than 500 test scores had a nominal impact on the almost 40,000 student data set.  The change was less than a 1% difference and the numbers would still round to the same whole number.  

### How is the school summary affected?

In the original anlaysis, Thomas High School school started with a 91% overall passing rate, which was a concern to the school board as being too high.  After calculationg the total number of 10th - 12th grade students as the new denominator, the rest of the testing data was adjusted accordingly.  

Original Analysis:
![Pic 3](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_THS_90.PNG)

Adjusted Analysis:
![Pic 4](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_THS_65.PNG)

Removing the 9th grade students from the data set had a huge impact by dropping from 91% to 65% for the overall passing rate. 

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
In the original analysis, Thomas High School ranked 2nd in the district raising red flags with the school board. 

Original Analysis:
![Pic 5](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/1_top_5_schools.PNG)

After adjusting the 9th grade data, Thomas High School ranked in the exact middle of 15 campuses at 8th from the bottom. 

Adjusted Analysis:
![Pic 6](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_bottom_8_schools.PNG)

## How does replacing the ninth-grade scores affect the following:

### Math and Reading Scores by Grade


#### Adjusted Math and Reading Scores 

In the original analysis, Thomas High School had 83.6 math average and 83.7 reading average for the 9th grade tests. 
Now the scores have been replaced with null values and shows up in Python programming as NAN in the following charts. 

Adjusted Average Math Scores ----------------------------------------------------- Adjusted Average Reading Scores: 

![Pic 7](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_math_by_grade_HS.PNG)
![Pic 8](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_read_by_grade_HS_correct.PNG)

### Scores by school spending

Thomas High School falls in the $630-$644/student spending range.  However, the hundreths place was needed to see the nominal changes. 
Original Analysis:
![Pic 9](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/1_spend_updated.PNG)
Adjusted Analysis:
![Pic 10](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_spending_updated.PNG)

There was very little spending impact by changing the 9th grade scores. 

### Scores by school size
Thomas High School is defined as a medium sized school.  The hundreths place was needed to see the nominal changes.

![Pic 11](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/1_size_updated.PNG)
![Pic 12](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_size_updated.PNG)

There was very little impact by campus size due to changing the 9th grade scores. 

### Scores by school type

Thomas High School is a charter school type. The hundreths place was needed to see the nominal changes.

![Pic 13](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/1_type_updated.PNG)
![Pic 14](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_type_updated.PNG)

There was very little impact by school type by changing the 9th grade scores. 

## Summary: Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.


