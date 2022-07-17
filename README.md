# School_District_Analysis
## Purpose of Analysis 
Previously we assited the chief data scientist for a city school, Maria, who is responsible for analyzing information from a variety of sources and in a variety of formats. Data was collected from the schools within the district and conevrted into data files "schools_complete.csv" and "students_complete.csv." Using the Pandas library in Jupyter Notebook software, we provided insights into performance trends and patterns that were meant to help make decisions at the school and district level. Data was analyzed on student funding and students' standardized test scores. 

It was later revealed that the data files used for the analysis showed evidence of academic dishonesty where reading and math grades for Thomas High School ninth graders appear to have been altered. Because the data for that group of students was deemed inaccuarate, we need to help Maria again to make sure that the data from that group of students does not impact the overall analysis we need to provide to the school board. 

Our goal is to replace the math and reading scores for Thomas High School with "NaNs" while keeping the rest of the data intact. Once we’ve replaced the math and reading scores, we need to repeat the school district analysis that we did previously and review how these changes affected the overall analysis.


Results: Using bulleted lists and images of DataFrames as support, address the following questions.

### How is the district summary affected?

##### Table 1: Original District Summary
![Original_district_summary](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_district_summary2.PNG)

##### Table 2: New District Summary
![New_district_summary](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_district_summary.PNG)



### How is the school summary affected?
###### Table 3: Original Thomas High School Performance Summary
![Original_THS_performance](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_THS_performance1.PNG)

##### Table 4: New Thomas High School Performance Summary
![New_THS_performance](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_THS_performance.PNG)



### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

##### Table 5: Original School Performance Ranking
![Original_school_performance](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_school_performance1.PNG)

##### Table 6: New School Performance Ranking
![New_school_performance](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_school_performance.PNG)


### How does replacing the ninth-grade scores affect the following:

#### Math and reading scores by grade

##### Table 7: Original Math Scores By Grade
![Original_math_grade](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_math_grade.PNG)

##### Table 8: Original Reading Scores By Grade
![Original_reading_grade](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_reading_grade.PNG)

##### Table 9: New Math Scores By Grade
![New_math_grade1](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_math_grade1.PNG)

##### Table 10: New Reading Scores By Grade
![New_reading_grade](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_reading_grade.PNG)


#### Scores by school spending

##### Table 11: Original School Spending Ranges Per Student
![Original_school_spending](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_school_spending.PNG)

##### Table 12: New School Spending Ranges Per Student
![New_school_spending](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_school_spending.PNG)

#### Scores by school size

##### Table 13: Original Scores By School Size
![Original_school_size_spending](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_school_size_spending.PNG)

##### Table 14: New Scores By School Size
![New_school_size_spending](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_school_size_spending.PNG)

#### Scores by school type

##### Table 15: Original Scores By School Type
![Original_school_type_spending](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_school_type_spending.PNG)

##### Table 16: New Scores By School Type
![New_school_type_spending](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_school_type_spending.PNG) 

Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
