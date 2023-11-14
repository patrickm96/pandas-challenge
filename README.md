# pandas-challenge
Module 4

Analysis location: https://github.com/patrickm96/pandas-challenge/tree/main/PyCitySchools
Please refer to PyCitySchools.ipynb

The following sources were referenced for completing the Module 4 Challenge:

- Count of unique elements in a series - https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.nunique.html
- Hide index column in results - https://stackoverflow.com/questions/34714145/pandas-styler-how-to-ignore-the-index-column-from-the-rendered-html
- Rename column - https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.rename.html
- Calculate mean of attribute elements - https://www.geeksforgeeks.org/python-pandas-dataframe-mean/#
- Calculate sum of attribute elements - https://www.w3schools.com/python/pandas/ref_df_sum.asp
- Conditional count - Module 4 starter code
- Create DataFrame - Instructor Eli Rosenberg covered this during class
- Format numbers with commas to represent thousands - Module 4 starter code
- Merge 2 dataframes - Instructor Eli Rosenberg covered this during class
- Group by function - Instructor Eli Rosenberg covered this during class
- Reset index function - https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.reset_index.html#pandas.DataFrame.reset_index
- Sort values - https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.sort_values.html
- Get element count as integer - https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.size.html
- pd.cut binning and labeling - Instructor Eli Rosenberg covered this during class
- Create headers in Jupyter Labs - https://www.tutorialspoint.com/jupyter/jupyter_notebook_markdown_cells.htm

## Instructions
Using Pandas and Jupyter Notebook, create a report that includes the following data. Your report must include a written description of at least two observable trends based on the data.

Hint: Check out the sample solution called PyCitySchools_starter.ipynb located in the .zip file to review the desired format for this assignment.

## District Summary
Perform the necessary calculations and then create a high-level snapshot of the district's key metrics in a DataFrame.

Include the following:

Total number of unique schools
Total students
Total budget
Average math score
Average reading score
% passing math (the percentage of students who passed math)
% passing reading (the percentage of students who passed reading)
% overall passing (the percentage of students who passed math AND reading)

## School Summary
Perform the necessary calculations and then create a DataFrame that summarizes key metrics about each school.

Include the following:

School name
School type
Total students
Total school budget
Per student budget
Average math score
Average reading score
% passing math (the percentage of students who passed math)
% passing reading (the percentage of students who passed reading)
% overall passing (the percentage of students who passed math AND reading)

### Highest-Performing Schools (by % Overall Passing)

Sort the schools by % Overall Passing in descending order and display the top 5 rows.

Save the results in a DataFrame called "top_schools".

### Lowest-Performing Schools (by % Overall Passing)

Sort the schools by % Overall Passing in ascending order and display the top 5 rows.

Save the results in a DataFrame called "bottom_schools".

### Math Scores by Grade
Perform the necessary calculations to create a DataFrame that lists the average math score for students of each grade level (9th, 10th, 11th, 12th) at each school.

### Reading Scores by Grade
Create a DataFrame that lists the average reading score for students of each grade level (9th, 10th, 11th, 12th) at each school.

### Scores by School Spending
Create a table that breaks down school performance based on average spending ranges (per student).

Use the code provided below to create four bins with reasonable cutoff values to group school spending.

![image](https://github.com/patrickm96/pandas-challenge/assets/135382512/1997aa62-c0e1-4e1a-a14f-5356abf025fe)

Use pd.cut to categorize spending based on the bins.

Use the following code to then calculate mean scores per spending range.

![image](https://github.com/patrickm96/pandas-challenge/assets/135382512/4981d98f-1230-4066-8d2b-e7b8dfe65580)

Use the scores above to create a DataFrame called spending_summary.

Include the following metrics in the table:

Average math score
Average reading score
% passing math (the percentage of students who passed math)
% passing reading (the percentage of students who passed reading)
% overall passing (the percentage of students who passed math AND reading)

### Scores by School Size

Use the following code to bin the per_school_summary.

![image](https://github.com/patrickm96/pandas-challenge/assets/135382512/34445cea-7dba-4dbc-b74a-05982a1e5b68)

Use pd.cut on the "Total Students" column of the per_school_summary DataFrame.

Create a DataFrame called size_summary that breaks down school performance based on school size (small, medium, or large).

### Scores by School Type

Use the per_school_summary DataFrame from the previous step to create a new DataFrame called type_summary.

This new DataFrame should show school performance based on the "School Type".
