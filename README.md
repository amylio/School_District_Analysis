# School_District_Analysis

## Overview of School District Analysis

The purpose of this project is to provide an analysis on Student funding and standardized test scores. The analysis will showcase trends in school performance and will be used to drive discussions and make strategic decisions at the school and district level. The results will contain:

* A high-level snapshot of the district's key metrics
* An overview of the key metrics for each school
* Tables presenting each of the following metrics:
	* Top 5 and bottom 5 performing schools, based on the overall passing rate
	* The average math score received by students in each grade level at each school
	* The average reading score received by students in each grade level at each school
	* School performance based on the budget per student
	* School performance based on the school size 
	* School performance based on the type of school

In order to complete this request and aggregate the data, Pandas Library and Jupyter notebook was used to read raw data, clean and inspect data, merge dataset, and perform calculations

The data was provide in two .csv files at the [school](https://github.com/amylio/School_District_Analysis/blob/main/Resources/schools_complete.csv) and [student](https://github.com/amylio/School_District_Analysis/blob/main/Resources/students_complete.csv) level. 


## The Results

At the district level, 64.9% of the students (25,421 students) passed both reading and math across 15 schools. The results were the same with or without the ninth graders at Thomas High School removed.

![district_summary](https://github.com/amylio/School_District_Analysis/blob/main/MOD4_Challenge_Submission/Images/District_Summary.png)

**How is the school summary affected?**

The top 5 schools with the highest percentage of overall passing grade had a marginal difference shown in Thomas High School's performance compared to the original with the Ninth graders data included. The overall passing % for the data with the Ninth grader removed reduced 31 bases points from the original (90.63% vs. 90.95%)

**Original Top 5**

![orig_top_5](https://github.com/amylio/School_District_Analysis/blob/main/MOD4_Challenge_Submission/Images/Orig_Top%205.png)

**Updated Top 5**

![top_5](https://github.com/amylio/School_District_Analysis/blob/main/MOD4_Challenge_Submission/Images/Top_5.png)

Replacing the ninth graders’ math and reading scores affected Thomas High School’s performance in a positive way compared to other schools. The overall passing % went from 65.1% to 90.6% once the ninth graders' data was removed.

**Original Results**

![Orig_THS_Results](https://github.com/amylio/School_District_Analysis/blob/main/MOD4_Challenge_Submission/Images/Orig_THS_Results.png)

**Revised Results without Ninth Graders for Thomas High School**

![Revised_THS_Results](https://github.com/amylio/School_District_Analysis/blob/main/MOD4_Challenge_Submission/Images/Revised_THS_Results.png)

**How does replacing the ninth-grade scores affect the following:**

* **Math and reading scores by grade:** For the ninth grade, the results showed "NaN" whereas the rest of the grades show a value.

![math_results](https://github.com/amylio/School_District_Analysis/blob/main/MOD4_Challenge_Submission/Images/Math_Score.png)
![reading_results](https://github.com/amylio/School_District_Analysis/blob/main/MOD4_Challenge_Submission/Images/Reading_Score.png)

* **Scores by school spending:** There was no visible change to the results by school spending compared to the original results that contained all of the student data. However, locations that spent less than $584 per student had 90% overall passing grade vs. only 54% in the highest spending range of $645-$675.

![spend](https://github.com/amylio/School_District_Analysis/blob/main/MOD4_Challenge_Submission/Images/Orig_spend.png)

* **Scores by school size:** There was no visible change to the results by school size compared to the original results that contained all of the student data. Medium sized schools (1,000 - 2,000) had the best results compared to the schools that had more than 2,000 students.

![size](https://github.com/amylio/School_District_Analysis/blob/main/MOD4_Challenge_Submission/Images/Score_by_Size.png)

* **Scores by school type:** There was no visible change to the results by school type compared to the original results that contained all of the student data. Charter schools outperformed District schools by 67% with 90% overall passing grade compared to 54%.

![type](https://github.com/amylio/School_District_Analysis/blob/main/MOD4_Challenge_Submission/Images/Score_by_type.png)

## Summary

In summary, when the Ninth grader data for Thomas High School was replaced with "NaN", the overall results were positive and the following metrics changed:

* Count of students reduced 12% (461) from 39,170 to 38,709
* % Passing math increased from 66.9% to 93.2%
* % Passing reading increased from 69.7% to 97.0%
* % Overall Passing increased from 65.1% to 90.6%
 
