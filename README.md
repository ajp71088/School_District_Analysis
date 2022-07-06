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
* % Passing Math and % Passing Reading each saw dramatic reductions (26.360856 & 27.64526, respectively.
* % Overall Passing, therefore, also reduced significantly (by 25.871559).

##### How does replacing the ninth graders' math and reading scores affect Thomas High School's performance relative to the other schools?
- Here's the top 5 schools before replacing the THS ninth graders:
![image](https://user-images.githubusercontent.com/107162310/177622022-15c53adb-3464-4d0e-af32-cad884fbc381.png)
- And here's the top 5 schools after only counting the THS metrics against its 10th-12th graders:
![image](https://user-images.githubusercontent.com/107162310/177622360-0a6ac2e2-b5c9-47c1-8ec4-4a117c5145b3.png)
- When recalculating the scores for THS using only the 10th-12th graders, there is very minimal impact on the school's ranking in the top schools.
- % Overall Passing saw a decrease, but not enough of one to take it down a spot.

##### How does replacing the ninth-grade scores affect the following:
##### - Math and reading scores by grade
The average math score decreased by 0.067412. The average reading score increased by 0.047152.
##### - Scores by school spending

##### - Scores by school size
##### - Scores by school type
