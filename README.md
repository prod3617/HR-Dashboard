# Tableau Data Analysis

# HR DashBoard
### Table of Contents

- [Project Description](#project-description)
- [Data Source](#data-source)
- [Data Cleaning](#data-cleaning)
- [Tools](#tools)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results/Findings](#resultsfindings)
  

### Project Description
The project aims to create a comprehensive dashboard to analyze human resource data to generate insights about the employees who are working and terminated. It also provides employees details records to perform in-depth analysis by applying the different filter options. 

![HR DashBoard Image](./HR%20DashBoard.png)


### Data Source
- Human Resources Data: The data is available in the "HumanResources.csv" file which contains all the information about the employees in the company.

### Tools
- Tableau Public: For data cleaning and visualization.

### Data Cleaning
- In the Tableau Public, we have inserted the csv data. I have checked each column for missing values and formatting issues. I have also checked whether the datatypes assigned to each column are correct.

### Exploratory Data Analysis
Performed some exploratory data analysis to find some information about key questions like
- Total number of employees who are actively working versus employees who are terminated.
- Overview of employees by Departments and job location.
- Employee demographics by gender, education, and age category.
- Salary comparison between male and female based on education level.

### Data Analysis
To find the answer to the key questions, I have created some calculated fields in the Tableau as
```Tableau
Total Active = COUNT(IF ISNULL([Termdate]) THEN [Employee ID] END)
```

### Results/Findings
[Dashboard View](https://public.tableau.com/app/profile/manjeet.kumar8420/viz/HRDashBoard_17379103129800/HRDetails#1)

- From the employee overview, most employees are hired in operations, and least are hired in HR.
- Most of the employees work in the headquarters (New York) around 70%.
- Employees with a Bachelor's degree are employed most and employees between the age of 35 to 44 are the most.
- Employees with a High School degree are the ones who need to work on their skills.
- As the education level increases, the average salary of females increases as compared to males.
- HR Manager are the one who is young and earn salary higher than the average salary of the entire company.

