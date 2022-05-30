# School_District_Analysis_Challenge


## Purpose
The purpose of this project is to evaluate the math and reading grades for Thomas High School students. A key dataset utilized in evaluating the analysis, indicates that there is evidence of academic dishonesty, as the grades for ninth grade students appear to have been altered. In an effort to uphold state-testing standards, a comparative analysis will be completed which will indicate whether replacing math and reading scores for Thomas High School ninth grade students with NaNs, which means ‘not a number’ and cannot be equal, will affect the overall analysis.


## PythonData Environment
1. Anaconda version 1.9.0
2. Conda version 4.13.0
3. Jupyter-Notebook version 6.4.8


## Process
1. Open Jupyter Notebook files from local directories using a development environment.
2. Read an external CSV file into a DataFrame.
3. Format a DataFrame column.
4. Determine data types of row values in a DataFrame.
5. Retrieve data from specific columns of a DataFrame.
6. Merge, filter, slice, and sort a DataFrame.
7. Apply the groupby() function to a DataFrame.
8. Use multiple methods to perform a function on a DataFrame.
9. Perform mathematical calculations on columns of a DataFrame or Series.

## Results

### How is the district summary affected?

Adjusted Analysis:
![Pic 2](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_dist_sum_2_decimals.PNG)

When comparing the two charts, removing less than 500 test scores had a nominal impact on the almost 40,000 student data set.  The change was less than a 1% difference and the numbers would still round to the same whole number.  

### How is the school summary affected?

In the original analysis, Thomas High School started with a 91% overall passing rate, which was a concern to the school board as being too high.  After calculating the total number of 10th - 12th grade students as the new denominator, the rest of the testing data was adjusted accordingly.  

Adjusted Analysis:
<img width="1097" alt="Screen Shot 2022-05-29 at 23 41 21" src="https://user-images.githubusercontent.com/104603177/170913198-5f3f0f31-1ff6-4aad-b7f3-4db5fac48036.png">

Removing the 9th grade students from the data set had a huge impact by dropping from 91% to 65% for the overall passing rate. 

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
In the original analysis, Thomas High School ranked 2nd in the district raising red flags with the school board. 

Original Analysis:
![Pic 5](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/1_top_5_schools.PNG)

After adjusting the 9th grade data, Thomas High School ranked in the exact middle of 15 campuses at 8th from the bottom. 

Adjusted Analysis:
![Pic 6](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_bottom_8_schools.PNG)

## How does replacing the ninth-grade scores affect the following:

### Adjusted Averages using the Math and Reading Scores 

In the original analysis, Thomas High School had 83.6 math average and 83.7 reading average for the 9th grade tests. 
Now the scores have been replaced with null values and shows up in Python programming as NaN in the following charts. 

Adjusted Average Math Scores ----------------------------------------------------- Adjusted Average Reading Scores: 

![Pic 7](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_math_by_grade_HS.PNG)
![Pic 8](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_read_by_grade_HS_correct.PNG)

### Scores by school spending

Thomas High School falls in the $630-$644/student spending range.  However, the hundredths place was needed to see the nominal changes. 

Original Analysis:
![Pic 9](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/1_spend_updated.PNG)

Adjusted Analysis:
![Pic 10](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_spending_updated.PNG)

There was very little spending impact by changing the 9th grade scores. 

### Scores by school size
Thomas High School is defined as a medium sized school.  The hundredths place was needed to see the nominal changes.

Original Analysis:
![Pic 11](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/1_size_updated.PNG)

Adjusted Analysis:
![Pic 12](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_size_updated.PNG)

There was very little impact by campus size due to changing the 9th grade scores. 

### Scores by school type

Thomas High School is a charter school type. The hundredths place was needed to see the nominal changes.

Original Analysis:
![Pic 13](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/1_type_updated.PNG)

Adjusted Analysis:
![Pic 14](https://github.com/Baylex/School_District_Analysis/blob/main/Resources/2_type_updated.PNG)

There was very little impact by school type by changing the 9th grade scores. 

## Summary: Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

1. The overall passing rate for Thomas High School changed dramatically from 91% to 65%. 

2. Thomas High School's ranking dropped from 2nd to 8th in the district of 15 campuses. 

3. Data at the grade level will now show as "NaN" in reports for the 9th grade students at Thomas High School  

4. In addition to the overall passing rate, the campus math and reading averages and passing percentages all saw shifts.  

The major changes will be seen at the lower views of the disaggregated data with minor impact to the larger data views.
