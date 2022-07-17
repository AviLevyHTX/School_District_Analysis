# School_District_Analysis
## Purpose of Analysis 
Previously we assited the chief data scientist for a city school, Maria, who is responsible for analyzing information from a variety of sources and in a variety of formats. Data was collected from the schools within the district and conevrted into data files "schools_complete.csv" and "students_complete.csv." Using the Pandas library in Jupyter Notebook software, we provided insights into performance trends and patterns that were meant to help make decisions at the school and district level. Data was analyzed on student funding and students' standardized test scores. 

It was later revealed that the data files used for the analysis showed evidence of academic dishonesty where reading and math grades for Thomas High School ninth graders appear to have been altered. Because the data for that group of students was deemed inaccuarate, we need to help Maria again to make sure that the data from that group of students does not impact the overall analysis we need to provide to the school board. 

Our goal is to replace the math and reading scores for Thomas High School with "NaNs" while keeping the rest of the data intact. Once we’ve replaced the math and reading scores, we need to repeat the school district analysis that we did previously and review how these changes affected the overall analysis.



## Analysis

We were able to successfully remove the data from 9th grade students at Thomas High School and completed all the analysis with the newly edited data. It was determined that there were 461 students in the 9th grade class so the math and reading scores for those students were replaced with “NaN.” This ensured that those students would still be evaluated in the school analysis but the dishonestly altered scores would not skew the performance of Thomas High School. The results showed small changes in the data and this will help the school board make better decisions with more accurate data. The following results and tables demonstrate the changes that occurred when the second round of analysis was completed. 


### How Is The District Summary Affected?
The removal of the 9th grade students at Thomas High School did little to change the District Summary. This can attributed by the fact that those 461 students represented a small amount compared to the overall 39,170 students in the district, so therefore their data would not strongly influence the overall district performance. Table 1 and Table 2 represent the original district summary and new district summary, respectively. The columns, understandably, not affected were total schools, total students, and total budget. However, the other variables minimally changed while only average reading score remained the same. 

##### Table 1: Original District Summary
![Original_district_summary](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_district_summary2.PNG)

##### Table 2: New District Summary
![New_district_summary](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_district_summary.PNG)


### How Is The School Summary Affected?
When Thomas High School was evaluated individually, the changes from the newly corrected data became more apparent, which can be seen in Table 3 and Table 4. The average math and reading scores did not appear to change but there was drastic change in the passing percentage for math, reading, and overall. Since the 9th grade scores were all replaced with “NaN” and therefore note evaluated, the scores and passing percentages would have only been calculated from students in 10th, 11th, and 12th grades at Thomas High School. This reveals that the 9th grade scores had drastically improved the passing percentage for math, reading, and overall. The original 9th grade data was clearly meant to show that students at Thomas High School were performing better than they actually were. 

###### Table 3: Original Thomas High School Performance Summary
![Original_THS_performance](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_THS_performance1.PNG)

##### Table 4: New Thomas High School Performance Summary
![New_THS_performance](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_THS_performance.PNG)


### How Does Replacing The Ninth Graders’ Math and Reading Scores Affect Thomas High School’s Performance Relative To The Other Schools?
Previously with the data of the 9th grade students, Thomas High School was able to have a better ranking amongst the other schools in the district. Table 5 and Table 6 rank the schools according to overall passing percentage. Table 5 shows that Thomas High School ranked second amongst all the schools. However using the new data, Table 6 shows that the ranking for Thomas High School significantly drops. This occurred because the data from the 9th grade students did not contribute to the performance at Thomas High School so the overall passing percentages dropped. 

##### Table 5: Original School Performance Ranking
![Original_school_performance](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_school_performance1.PNG)

##### Table 6: New School Performance Ranking
![New_school_performance](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_school_performance.PNG)


### How does replacing the ninth-grade scores affect the following:

#### Math and Reading Scores By Grade
Since only the 9th grade data from Thomas High School was removed, the performance at the other schools did not change for math and reading scores in grades 9-12. Table 7 and 8 show how the data was affected for math scores, while Table 9 and Table 10 show how the data was affected for reading scores. The data for the 9th grade students was clearly seen as changed to “NaN.” Because that data was changed to “NaN”, the scores for the 9th grade students did not count towards the performance at Thomas High School. 

##### Table 7: Original Math Scores By Grade
![Original_math_grade](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_math_grade.PNG)

##### Table 8: New Math Scores By Grade
![New_math_grade1](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_math_grade1.PNG)

##### Table 9: Original Reading Scores By Grade
![Original_reading_grade](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_reading_grade.PNG)

##### Table 10: New Reading Scores By Grade
![New_reading_grade](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_reading_grade.PNG)


#### Scores by School Spending
The scores at Thomas High School were changed because of removing the 9th grade students, so that in turn impacted scores of spending range group of schools that Thomas High School was apart of. As part of the original analysis, the schools in the district were divided according to how much each school spent per student. Four groups were made and (in dollars) were 0-585, 586-630, 631-645, and 646-675. The original and new data can be visualized in Table 11 and Table 12. Three of the groups did not have scores that changed, however the group of schools in spending range $631-$645 did have passing percentage scores that changed. It can be inferred that Thomas High School is in that group since that was the only school with grades that changed. Since the grades for Thomas High School changed, the scores for that group of schools also decreased. 

##### Table 11: Original School Spending Ranges Per Student
![Original_school_spending](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_school_spending.PNG)

##### Table 12: New School Spending Ranges Per Student
![New_school_spending](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_school_spending.PNG)


#### Scores by School Size
In the previous analysis, the schools were also separated by school size to compare the scores of differently sized schools in the district. The schools were categorized as small with less than 1,000 students, medium with 1,00 to 1,999 students, or large with 2,000 to 5,000 students. Table 13 and Table 14 show how the data changed as a result of the score changes for Thomas High School. The small and large schools did not change. The only group affected was the medium sized group of schools with decreased passing percentages, with all the passing percentages dropping by 6 percentage points. This can be expected since Thomas High School was shown to have 1,635 students and would therefore fall in the medium size category of schools. 

##### Table 13: Original Scores By School Size
![Original_school_size](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_school_size.PNG)

##### Table 14: New Scores By School Size
![New_school_size](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_school_size.PNG)


#### Scores by School Type
All the schools were also divided into two groups of school types, where one was Charter Schools and the other group was District Schools. Thomas High School is a Charter School, so the grades for that group of schools changed when the grades at Thomas High School changed. Table 15 and Table 16 show the difference in grades. The Charter Schools are shown to have lower passing percentages, while the District Schools did not change. 

##### Table 15: Original Scores By School Type
![Original_school_type_spending](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/Original_school_type_spending.PNG)

##### Table 16: New Scores By School Type
![New_school_type_spending](https://github.com/AviLevyHTX/School_District_Analysis/blob/main/analysis/New_school_type_spending.PNG) 



## Summary
The school board relies on accurate data to evaluate the performance of their schools and make important decisions. The revelation of dishonest data of 9th grade students at Thomas High School required that those scores to not be assessed in order to maintain the accurate and honest data. With the new data, there are various changes evident from the new results. The first change is that the performance of the 9th grade students have limited impact on the overall district performance, which can help indicate to the school board whether their goals are being met. Another change is that while the average math and reading scores at Thomas High School may not have changed, the passing percentage for math, reading, and overall were drastically changed. Is clear the 9th grade data played a large role in the passing percentages. A third change is that without the 9th grade data, the ranking of Thomas High School significantly dropped and that can have impacts on the resources allocated to that school. A final change is that the performance of the groups that Thomas High School is apart of all changed and decreased. 
