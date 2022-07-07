# School_District_Analysis

### Overview of the School District Analysis
Analysis was provided to the school board so that they would have the information they need to make informed decisions about school performance and budgets. However, upon initial review, it was determined that academic dishonesty of one entire grade's worth of students in one school had skewed the results. So the dataset was cleaned of those dishonest scores and the analysis was re-run.

#### Results

##### How is the district summary affected?
- The district summary from the initial analysis (before the data was corrected to eliminate the impact of the academic dishonesty) looked like this:
![image](https://user-images.githubusercontent.com/107162310/177040418-50367578-2866-405e-878f-a0e3b97b0adc.png)
- Here's the corrected district summary:
![image](https://user-images.githubusercontent.com/107162310/177590084-6b4c087e-1730-45da-bb0e-23a1ef8ec53c.png)
* The district summary was minimally affected by the removal of Thomas High School's 9th grade math and reading scores.
* The Average Math Score and % Overall Passing both fell by 0.1.
* % Passing Math dropped by 0.2, from 75 to 74.8.
* % Passing Reading saw the greatest change at a 0.3 decrease, from 86 to 85.7.
* All other statistics were not impacted enough for the district summary to shift.

##### How is the school summary affected?
- The initial school summary:
![image](https://user-images.githubusercontent.com/107162310/177591074-5054b04c-1898-42cc-9101-707ca767ecf7.png)
- The corrected school summary:
![image](https://user-images.githubusercontent.com/107162310/177591179-0ae38f1f-dbf3-480d-b384-03853db5e516.png)
* Thomas High School's summary metrics were impacted in several ways.
* Average Math Score fell by 0.067412, while Average Reading Score increased by 0.047152.
* % Passing Math and % Passing Reading each saw dramatic reductions (26.360856 & 27.64526, respectively).
* % Overall Passing, therefore, also reduced significantly (by 25.871559).

##### How does replacing the ninth graders' math and reading scores affect Thomas High School's performance relative to the other schools?
- Here's the top 5 schools before replacing the THS ninth graders:
![image](https://user-images.githubusercontent.com/107162310/177622022-15c53adb-3464-4d0e-af32-cad884fbc381.png)
- And here's the top 5 schools after only counting the THS metrics against its 10th-12th graders:
![image](https://user-images.githubusercontent.com/107162310/177622360-0a6ac2e2-b5c9-47c1-8ec4-4a117c5145b3.png)
- When recalculating the scores for THS using only the 10th-12th graders, there is very minimal impact on the school's ranking in the top schools. THS is still ranked 2nd in % Overall Passing.
- % Overall Passing saw a decrease, but not enough of one to take it down a spot.

##### How does replacing the ninth-grade scores affect the following:
##### - Math and reading scores by grade
- Prior to removing the dishonest THS scores, the average 9th grade math score could be found using the mean function:
![image](https://user-images.githubusercontent.com/107162310/177664423-a00798fa-2a52-4594-afe0-e14be9ade2ae.png)

- And the average 9th grade reading score:

![image](https://user-images.githubusercontent.com/107162310/177664643-b50c535a-ddcc-4d32-99e9-4d82485e6912.png)

- Removing the dishonest 9th grade scores caused the average 9th grade math score district wide to go down by about 0.2:
![image](https://user-images.githubusercontent.com/107162310/177664938-23276c14-a192-4fe9-bb90-9f833c475dd5.png)

- And without the dishonest scores, the average 9th grade reading score reduced by about 0.1:
![image](https://user-images.githubusercontent.com/107162310/177665213-69258abb-d1e6-4742-81df-4060c3695e78.png)

##### - Scores by school spending
- Prior to removing the THS 9th graders:

![image](https://user-images.githubusercontent.com/107162310/177666838-2a6b14a3-b258-407a-a100-b329daad0d73.png)


- After removing the THS 9th graders:

![image](https://user-images.githubusercontent.com/107162310/177666798-67ba73ff-85c7-44b5-8a8e-4a1c1316c266.png)

- With the formatting applied to the spending summary dataframe, there is no impact on the average scores. (However, if the rounding extended into further decimal places, there would be some minor changes.)

##### - Scores by school size
- Original scores in the school size dataframe:

![image](https://user-images.githubusercontent.com/107162310/177667280-649288fa-db31-4d91-9aa9-5428b5bcb4fd.png)

- Updated dataframe:

![image](https://user-images.githubusercontent.com/107162310/177667353-786bdbbf-f37f-452e-962d-25905b612d7a.png)

- Similar to the school spending dataframe, with the formatting applied there is no difference in the average math or reading scores.

##### - Scores by school type
- Original school type dataframe:

![image](https://user-images.githubusercontent.com/107162310/177667482-a5b336ae-1de9-404d-a940-bde6e4e51335.png)

- Updated:

![image](https://user-images.githubusercontent.com/107162310/177667535-663f3dec-6156-4713-bec9-50448f6b6907.png)

- Unsurprisingly, this trend continues. When rounding to the first decimal point, there is no change to the scores.

### Summary

Thomas High School's ninth graders only amounted to 461 students, which is just 1.2% of the entire school district. Given that minor adjustment, the school district analysis was minimally impacted when their scores were replaced:
1. Chief among the changes after changing all of Thomas High School's ninth grader scores to NaN, their overall passing percentage dropped by 25.871559, in line with the school's reading and math passing percentages. 
2. Despite the large change for THS, the overall district passing percentage fell by just 0.1.
3. After excluding the THS ninth graders entirely, its overall passing percentage reduced by 0.317688 (although it still ranked second in that statistic).
4. District-wide, after excluding THS, the ninth grade math and reading scores reduced by approximately 0.2 and 0.1, respectively.
