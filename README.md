# School_District_Analysis
## Overview of the school district analysis: 
The ultimate purpose of this particular analysis was to determine specifically math and reading scores from Thomas High School. The reason behind this was to see overall results from 9th graders  in this school and see how it would affect state-wide standarized testing results. There was dishonesty in some of the grades because they have been altered. Replacing NaNs will keep the data correct in order to do more investigation. Some changes did affect the overall challenge. 

<img width="461" alt="image" src="https://user-images.githubusercontent.com/92067596/158090442-ec38509b-4cd2-4af3-9a94-07182c2941e0.png">

From the original csv code it is then broken down into a data frame which displays student information, grades and school information to later be used to idenity specific results. 
The school summary is affected by displaying all grade levels and grades for them. When you replace the ninth graders math and reading scores frmo Thomas High School compared to the other school you are only recieving information for them. Using thhe follwowing code: 

thomas_high_school_ninth_grade_student_df = student_data_df[(student_data_df["school_name"] == "Thomas High School") 
                                                            & (student_data_df["grade"] == "9th")]

How does replacing the ninth-grade scores affect the following:
 - Math and reading scores, we fisrt have to retrieve the date from the CSV whcih was converted into the "complete" data frame using the specific function from panda .df we must put in the argument.
passing_math_reading = school_data_complete_df[(school_data_complete_df["math_score"] >= 70)
                                               & (school_data_complete_df["reading_score"] >= 70)]

<img width="470" alt="image" src="https://user-images.githubusercontent.com/92067596/158090497-ba45d447-952c-41ae-bfec-410734a88381.png">

-Scores by school spending

<img width="374" alt="image" src="https://user-images.githubusercontent.com/92067596/158091594-35d085cf-5e8a-4172-afe4-a22f2b12fef8.png">

With this code we can get the information and it shows on the data frame that schools with lower budgest tende to have lower testing scores. 
<img width="508" alt="image" src="https://user-images.githubusercontent.com/92067596/158091935-951ec7b4-bb06-49cb-a276-10ebe8fce54c.png">

When updating and making changes in the school district analysis, while also replacing the NaNs, the ninthgraders, and Thomas High School there was a chnage in percentage in overall  the scores of math and reading which highly influence the school's ranking.
