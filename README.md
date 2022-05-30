# School_District_Analysis_Challenge


## Purpose
The purpose of this project is to evaluate the math and reading grades for Thomas High School students. A key dataset  analysis indicates that there is evidence of academic dishonesty, as the grades for ninth grade students appear to have been altered. In an effort to uphold state-testing standards, a comparative analysis will be completed which will indicate whether replacing math and reading scores for Thomas High School ninth grade students with NaNs, which means ‘not a number’ and cannot be equal, will affect the overall analysis.


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
<img width="830" alt="image" src="https://user-images.githubusercontent.com/104603177/171021329-5936951e-c3dc-40a3-8299-25d670b062ef.png">


When comparing the two charts, removing less than 500 test scores had a nominal impact on the almost 40,000 student data set.  The change was less than a 1% difference and the numbers would still round to the same whole number.  

### How is the school summary affected?

In the original analysis, Thomas High School started with a 91% overall passing rate, which was a concern to the school board as being too high.  After calculating the total number of 10th - 12th grade students as the new denominator, the rest of the testing data was adjusted accordingly.  

Adjusted Analysis:
<img width="1097" alt="Screen Shot 2022-05-29 at 23 41 21" src="https://user-images.githubusercontent.com/104603177/170913198-5f3f0f31-1ff6-4aad-b7f3-4db5fac48036.png">

Removing the 9th grade students from the data set had a huge impact by dropping from 91% to 65% for the overall passing rate. 

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
In the original analysis, Thomas High School ranked 2nd in the district raising red flags with the school board. 

Original Analysis:
<img width="1103" alt="image" src="https://user-images.githubusercontent.com/104603177/171008957-0163d885-c7be-4de3-ae87-8d8e535d1c7e.png">

After adjusting the 9th grade data, Thomas High School ranked in the exact middle of 15 campuses at 8th from the bottom. 

Adjusted Analysis:
![image](https://user-images.githubusercontent.com/104603177/171008316-6c393083-c843-47b5-9c08-fae7cfbee8d8.png)

## How does replacing the ninth-grade scores affect the following:

### Adjusted Averages using the Math and Reading Scores 

In the original analysis, Thomas High School had 83.6 math average and 83.7 reading average for the 9th grade tests. 
Now the scores have been replaced with null values and shows up in Python programming as NaN in the following charts. 

Adjusted Average Math Scores ----------------------------------------------------- Adjusted Average Reading Scores: 
![image](https://user-images.githubusercontent.com/104603177/171009233-ba8abb95-06ad-4391-920f-839f69b6fcb6.png)
![image](https://user-images.githubusercontent.com/104603177/171009273-f4a118c0-7eee-4239-90c3-bef2caabc780.png)




### Scores by school spending

Thomas High School falls in the $630-$644/student spending range.  However, the hundredths place was needed to see the nominal changes. 

Original Analysis:
![image](https://user-images.githubusercontent.com/104603177/171009444-0217afcd-5e7f-4963-a525-d9f08e7eed1f.png)

Adjusted Analysis:
![image](https://user-images.githubusercontent.com/104603177/171009470-ad7fccb2-7bd8-4856-93cc-a52436ea3623.png)

There was very little spending impact by changing the 9th grade scores. 

### Scores by school size
Thomas High School is defined as a medium sized school.  The hundredths place was needed to see the nominal changes.

Original Analysis:
![image](https://user-images.githubusercontent.com/104603177/171009618-b270419d-cdea-426b-931d-52cfc2f78d50.png)

Adjusted Analysis:
![image](https://user-images.githubusercontent.com/104603177/171009650-91ac4b97-2e2b-4577-b396-f4064d05257d.png)

There was very little impact by campus size due to changing the 9th grade scores. 

### Scores by school type

Thomas High School is a charter school type. The hundredths place was needed to see the nominal changes.

Original Analysis:
![image](https://user-images.githubusercontent.com/104603177/171009787-2b5552bb-b6cf-446e-a41f-7e762bddd53e.png)

Adjusted Analysis:
![image](https://user-images.githubusercontent.com/104603177/171009824-adc0a9ca-a31e-4ea9-be13-56e11ec25150.png)

There was very little impact by school type by changing the 9th grade scores. 

## Summary: Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

1. The overall passing rate for Thomas High School changed dramatically from 91% to 65%. 

2. Thomas High School's ranking dropped from 2nd to 8th in the district of 15 campuses. 

3. Data at the grade level will now show as "NaN" in reports for the 9th grade students at Thomas High School  

4. In addition to the overall passing rate, the campus math and reading averages and passing percentages all saw shifts.  

The major changes will be seen at the lower views of the disaggregated data with minor impact to the larger data views.
