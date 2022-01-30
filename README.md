# School District Analysis

## Overview
Using student and school data from 15 high schools, I sought reach conclusions regarding student test score performance (both reading and math), school spending (both overall and per student), and student passing percentage (math, reading, and overall). In completing this analysis, I created several data frames that each organized the performance and spending data differently. I initially executed the analysis with the complete dataset. To experiment and challenge myself, I replaced all the scores of Thomas High School 9th graders with null grades and observed how my results changed. I used python 3.7.6 with Jupyter Notebook along with the Pandas package to perform my analysis.

## Results
### District Summaries

#### School District Summary using full dataset

![Screen Shot 2022-01-29 at 10 36 17 PM](https://user-images.githubusercontent.com/95651156/151689475-c263a27d-24dc-42c2-8567-3d337177842c.png)




#### School District Summary after removing THS 9th graders

![Screen Shot 2022-01-29 at 10 37 42 PM](https://user-images.githubusercontent.com/95651156/151689499-fb8d0cb3-e100-4427-90a4-6b9549a324d3.png)

*	From the above images, it’s apparent that removing the THS ninth grader data had a marginal effect on the overall performance of the entire district
*	Average math score decreased by 0.1 
*	Average reading score stayed the same when rounding to the nearest tenth of a point
*	% Passing Math dropped 0.2 percentage points
*	% Passing Reading dropped 0.1 percentage points
*	% Overall Passing (the percentage of students who scored 70 or above on both math and reading) dropped by 0.3 percentage points

### School Summaries

#### Thomas High School Summary using full dataset

![Screen Shot 2022-01-29 at 11 34 25 PM](https://user-images.githubusercontent.com/95651156/151690929-620c7928-c073-44b4-823f-a0905b56608c.png)



#### Thomas High Schoool Summary after removing THS 9th graders

![Screen Shot 2022-01-29 at 11 35 26 PM](https://user-images.githubusercontent.com/95651156/151690967-1d7de12e-0dd3-4854-8591-ee92969c354d.png)

#### THS scores with 9th Graders Data vs. without (all calculations rounded to nearest hundredth)

* Average math score is .07 points lower after removing 9th graders
* Average reading score is .05 points higher after removing 9th graders
* % Passing Math is 0.09 percentage points lower after removing 9th graders
* Passing Reading is 0.29 percentage points lower after removing 9th graders
* Overall Passing is 0.32 percentage points lower after removing 9th graders
* NOTE: No other rows in the school summary dataframe changed since only data from THS was altered


### THS performance relative to other schools

#### Top Five Overall Performing Schools with THS 9th Graders Included

![top_5-fll](https://user-images.githubusercontent.com/95651156/151691752-a3b198f7-047c-404c-86cf-936e505810b4.png)

#### Top Five Overall Performing Schools without THS 9th Graders

![top_5_without](https://user-images.githubusercontent.com/95651156/151691783-a7a99ee3-da85-4895-9905-fe6771f0f108.png)

While THS math, reading, and overall performance drops when 9th graders data is removed, THS still ranks second out of 15 in overall performance in both cases.

### Math Scores Organized by Grade Level

#### Math scores by grade level before removing THS 9th Graders

![Math Scores by grade](https://user-images.githubusercontent.com/95651156/151709613-aa476891-85ae-4213-891b-ef408e99bbdc.png)

#### Math scores by grade level after removing THS 9th Graders

![Math Scores by Grade-Challenge](https://user-images.githubusercontent.com/95651156/151709652-7d8f496e-5e98-4b19-9b91-98a643b68103.png)

* The average math score of 83.6 for THS 9th graders is replaced with a null score after removing THS 9th graders from the data frame.
* All other scores remain the same

### Reading Scores Organized by Grade Level

#### Reading scores by grade before removing THS 9th Graders

![Reading Scores by grade](https://user-images.githubusercontent.com/95651156/151709729-3bcfd847-2f0e-4c21-91c4-03d96d98bf05.png)

#### Reading scores by grade after removing THS 9th Graders

![Reading Scores by Grade-Challenge](https://user-images.githubusercontent.com/95651156/151709752-771ade00-beca-4692-ba98-da4d669e4413.png)

* The average reading score of 83.7 for THS 9th graders is replaced with a null score after removing THS 9th graders from the data frame.
* All other scores remain the same

### Scores by School Spending

#### Scores by school spending with THS 9th Graders

![Scores by spending](https://user-images.githubusercontent.com/95651156/151709865-69d0e835-334c-4457-ac5a-dee2b163d8e9.png)

#### Scores by school spending without THS 9th Graders

![Scores by spending-challenge](https://user-images.githubusercontent.com/95651156/151709879-ded5274b-0bf3-4fbf-aff5-2a6047b4f2a9.png)

* The two charts display identical metrics with rounding
* Removing the THS ninth graders had minimal impact on the scores and passing percentages filtered by school spending per student

### Scores by School Size

#### Scores by school size with THS 9th Graders

![Scores by school size](https://user-images.githubusercontent.com/95651156/151709899-765ae038-a373-43a3-a81e-70678b726298.png)

#### Scores by school size without THS 9th Graders

![Scores by size-challenge](https://user-images.githubusercontent.com/95651156/151709906-7c9452a1-0ade-49ca-bdfb-421cc2858e31.png)

* The two charts display identical metrics with rounding
* Removing the THS ninth graders had minimal impact on the scores and passing percentages filtered by school size per student

### Scores by School Type

#### Scores by school type with THS 9th Graders

![Scores by school type](https://user-images.githubusercontent.com/95651156/151709919-d27cb14e-d3ec-466e-846d-5239dfafaf32.png)

#### Scores by school type without THS 9th Graders

![Scores by type-challenge](https://user-images.githubusercontent.com/95651156/151709930-3d7a1773-99fa-4f61-989b-6bd005006743.png)


* The two charts display identical metrics with rounding
* Removing the THS ninth graders had minimal impact on the scores and passing percentages filtered by school type (district vs. charter)

## Summary of Results

#### 4 Key Changes from dropping THS 9th Graders' Scores

*  Overall passing percentage for the entire school district dropped after removing THS 9th grade scores, which shows that THS 9th graders scored above average overall when considering the entire school district
* Ovrall passing percentage for THS dropped after removing THS 9th grade scores, which shows that THS 9th graders scored above average overall compared to other grade levels at THS
* THS rankes second out of 15 schools in overall performance with and without including their 9th grade test scores
* With slight rounding, average scores organized by school spending, school size, and school type remained the same after removing THS 9th grade scores, which is likely due to the fact that THS 9th graders make up a relatively small portion of the overall school district population

