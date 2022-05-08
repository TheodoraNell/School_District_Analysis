# School District Analysis
Performing an analysis on school district data using Pandas

## Overview
The purpose of this analysis is to examine two sets of school and student data and create a summary of metrics evaluating math/reading performance and school spending based on several factors. There is a repetition of the analysis using the same script but with the removal of potentially innacurate grade data. The results of the analysis are then compared to explore the impact of the questionable data on the overall results. 

## Results

The data that was removed for the repeated analysis consists of math and reading scores for all 9th Grade students at Thomas High School. This removal was by request due to suspected academic dishonesty to which the extent is unknown. Each datapoint removed was replaced with `'NaN'`. In this section, the results of the repeated analysis will be diplayed using images. In all instances, the top image shown represents the first analysis and the bottom image(s) represent the repeated analysis with the replaced datapoints.

- ### Impact on District Summary 
The district summary remains largely unaffected, the only change being the decrease of "Average Math Score" from 79.0 to 78.9
![district_summary_original](https://user-images.githubusercontent.com/99051640/167316955-1ab7f642-9dd5-474e-89fb-4acd91877cef.png)
![district_summary_challenge](https://user-images.githubusercontent.com/99051640/167316941-40d7488a-cd80-4a46-b829-bf49590924d0.png)

- ### Impact on School Summary
The School Summary is most impacted by the removal of the data. Large decreases can initially be seen for Math, Reading, and Overall passing percentages due to replacing the data with `'NaN'`. The columns displaying averages are unafeccted since the `'NaN'` values are not considered as part of the whole. However, they are when calculaing percentages. This is demonstrated below and then corrected for:
![school_summary_original](https://user-images.githubusercontent.com/99051640/167317078-5a06e362-9ce6-47a8-b1d8-c77b58937ce9.png)
![school_summary_challenge](https://user-images.githubusercontent.com/99051640/167317080-473190e2-f322-4c26-b57f-13617bbc5f55.png)

To adjust for the replaced values when calculating the passing percentages, the scores for 10th-12th grade students are calculated separately and then replaced in the dataframe using the `loc()` method. After adjusting, the school summary still shows impact from the data removal, though far less with values only changing by tenths of a percent at most.
![school_summary_original](https://user-images.githubusercontent.com/99051640/167317078-5a06e362-9ce6-47a8-b1d8-c77b58937ce9.png)
![school_summary_adjusted](https://user-images.githubusercontent.com/99051640/167318160-5b88b585-fbed-45bf-86aa-59f9db345419.png)

- ### Impact on Thomas High School’s performance relative to the other schools?
Granted the values for passing percentages are adjusted, there is no effect on the relative perfromance of Thomas High School. It remains second on the "Top Schools" list. 
![top_schools_original](https://user-images.githubusercontent.com/99051640/167317378-9b5077b8-4ab5-485a-902b-f02a5e78e387.png)
![top_schools_challenge](https://user-images.githubusercontent.com/99051640/167317383-005a6322-b0b2-4b2e-9802-df03ca007173.png)

- ### Impact on math and reading scores by grade
The only change is the value for 9th Grade students which corresponds to the assigned grade values of `'NaN'`.
![math_by_grade_original](https://user-images.githubusercontent.com/99051640/167317758-d90ac4b3-9301-4d23-a69b-4c1e5e4d5e73.png)
![reading_by_grade_original](https://user-images.githubusercontent.com/99051640/167319796-35bd7c5f-0d73-458c-832e-7f88ce9a3e45.png)

![math_by_grade_challenge](https://user-images.githubusercontent.com/99051640/167317498-3d6a3875-50e1-4357-a254-268710e307b5.png)
![reading_by_grade_challenge](https://user-images.githubusercontent.com/99051640/167317510-2c9206dd-d2da-44f1-8df9-517bc03a34f6.png)

- ### Impact on scores by school spending
There is almost no visible impact on this metric
![spending_summary_original](https://user-images.githubusercontent.com/99051640/167319487-de4d7634-92ae-4d47-8ae9-81df41ff127b.png)
![spending_summary_challenge](https://user-images.githubusercontent.com/99051640/167317692-f296904e-2439-428d-a395-8c40df3d15cf.png)

- ### Scores by school size
![size_summary_original](https://user-images.githubusercontent.com/99051640/167317908-9c8d2731-2480-491d-8cc9-e84e258e38f4.png)
![size_summary_challenge](https://user-images.githubusercontent.com/99051640/167319298-c4fba750-247d-4187-9023-5f544e915a21.png)


- ### Scores by school type
There is no visible change in these metrics
![type_summary_original](https://user-images.githubusercontent.com/99051640/167317938-72bc932c-3039-4759-9189-acb0041761f3.png)
![type_summary_challenge](https://user-images.githubusercontent.com/99051640/167317940-6089eb6b-87e7-4578-b6c5-932bb54f25ba.png)

## Summary
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
The four most significant changes in the udated school district analysis are:
- Average Math and Reading scores
- Percent Passing Math and Reading Scores
- Overall Percent Passing
- District Average Math Score: this decrease is seemingly insignificant since it is only .1%, but with rounding it appears to be a 1% difference
