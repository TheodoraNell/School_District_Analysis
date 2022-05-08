# School District Analysis
Performing an analysis on school district data using Pandas

## Overview
The purpose of this analysis is to examine two sets of school and student data and create a summary of metrics evaluating math/reading performance and school spending based on several factors. There is a repetition of the analysis using the same script but with the removal of potentially innacurate grade data due to suspected academic dishonesty. The results of the analysis compared to explore the impact of the questionable data on the overall results. 

## Results

The data that was removed for the repeated analysis consists of all math and reading scores for 9th Grade students at Thomas High School. All datapoints removed were replaced with `'NaN'`

- ### How is the district summary affected?

![district_summary_original](https://user-images.githubusercontent.com/99051640/167316955-1ab7f642-9dd5-474e-89fb-4acd91877cef.png)
![district_summary_challenge](https://user-images.githubusercontent.com/99051640/167316941-40d7488a-cd80-4a46-b829-bf49590924d0.png)

- ### How is the school summary affected?

The School Summary is most impacted by the removal of the data
![school_summary_original](https://user-images.githubusercontent.com/99051640/167317078-5a06e362-9ce6-47a8-b1d8-c77b58937ce9.png)
![school_summary_challenge](https://user-images.githubusercontent.com/99051640/167317080-473190e2-f322-4c26-b57f-13617bbc5f55.png)
![school_summary_adjusted](https://user-images.githubusercontent.com/99051640/167318160-5b88b585-fbed-45bf-86aa-59f9db345419.png)

How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

It does not, granted they are adjusted:
![top_schools_original](https://user-images.githubusercontent.com/99051640/167317378-9b5077b8-4ab5-485a-902b-f02a5e78e387.png)
![top_schools_challenge](https://user-images.githubusercontent.com/99051640/167317383-005a6322-b0b2-4b2e-9802-df03ca007173.png)


How does replacing the ninth-grade scores affect the following:

Math and reading scores by grade
![math_by_grade_original](https://user-images.githubusercontent.com/99051640/167317758-d90ac4b3-9301-4d23-a69b-4c1e5e4d5e73.png)
![math_by_grade_challenge](https://user-images.githubusercontent.com/99051640/167317498-3d6a3875-50e1-4357-a254-268710e307b5.png)

![reading_by_grade_original](https://user-images.githubusercontent.com/99051640/167317752-b079016d-8311-403e-b274-eff467a50e3a.png)
![reading_by_grade_challenge](https://user-images.githubusercontent.com/99051640/167317510-2c9206dd-d2da-44f1-8df9-517bc03a34f6.png)

Scores by school spending
![spending_summary_original](https://user-images.githubusercontent.com/99051640/167317689-eb25b0e6-dc88-4d14-bf02-6aa2d25b2f17.png)
![spending_summary_challenge](https://user-images.githubusercontent.com/99051640/167317692-f296904e-2439-428d-a395-8c40df3d15cf.png)

Scores by school size
![size_summary_original](https://user-images.githubusercontent.com/99051640/167317908-9c8d2731-2480-491d-8cc9-e84e258e38f4.png)
![spending_summary_challenge](https://user-images.githubusercontent.com/99051640/167317849-562eeef8-541c-44c8-9d3b-e11f81559478.png)

Scores by school type
![type_summary_original](https://user-images.githubusercontent.com/99051640/167317938-72bc932c-3039-4759-9189-acb0041761f3.png)
![type_summary_challenge](https://user-images.githubusercontent.com/99051640/167317940-6089eb6b-87e7-4578-b6c5-932bb54f25ba.png)

## Summary
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
