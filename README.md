# School_District_Analysis
This was a Data Analysis Project using Anaconda and Jupyter to practice basic functions available in these programs.

# Overview of the school district analysis: Explain the purpose of this analysis.

Data analysts are often given raw data and we must be able to properly 'clean' this data and be able to format and present it in  a way that is the most useful to whoever it is that we present it to.  In this project we are given two 'comma separated value'(CSV) files related to the school districts and the performance of the students in these districts.

The analysis was completed in the Jupyter Notebook program, and we used features of Anaconda and Python to let us access a tool called "pandas" to complete a detailed breakdown of the raw data we were given. The data was moved into a DataFrame, or a 2 dimensional structure similar to a spreadsheet which allowed us to better visualize the data.  Each file was originally place in its own Dataframe, but Python allowed us to merge these two frames into a single frame that allows for easier analysis.

# Results: 

## How is the district summary affected?

The district summary dataframe gives us the overall results of all students across all the schools.  The data provided gives us the average, and with this we can compare a school or student's performance compared to the entire population of students. 

![district summary image](https://github.com/MXV0921/School_District_Analysis/blob/main/Resources/district_summary_df_unadjusted.png)

After adjusting the results of Thomas High School and eliminating the ninth grade from that school's results it does not greats affect affect the district summary.  This number is based on the total student count and the results were not greatly impacted by this change.

![district summary image](https://github.com/MXV0921/School_District_Analysis/blob/main/Resources/district_summary_df.png)

 * Percent Passing Math decreased from 75.0% to 74.8%
 * Percent Passing Reading decreased from 85.8% to 85.7%
 * Overall Passing decreased from 65.2% to 64.9%


## How is the school summary affected?

The school summary dataframe shows a large variance from the unadjusted dataframe:

![unadjusted school summary](https://github.com/MXV0921/School_District_Analysis/blob/main/Resources/per_school_unadjusted.png)

After adjusting the results for Thomas High School we can see that their scores jumped quite a bit:
![adjusted school summary](https://github.com/MXV0921/School_District_Analysis/blob/main/Resources/per_school_adjusted.png)

* Percentage Passing Math increased from 66.911315% to 93.272171%
* Passing Reading increased from 69.663609% to 97.308869%
* Overall Passing Percent decreased to 65.076453% to 90.948012%

## How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
 
Eliminating the results of the ninth graders' math and reading scores positively impacted the average performance for Thomas High School. Prior to the adjustment, Thomas HS was the lowest performing Charter School, but by removing the 9th grade performance they end up having the second highest overall passing percent in the entire district.


## Scores by school spending

The adjustment we made would not affect the spending range 'bin' that Thomas HS was placed in.  Their Total Student count has not changed and their budget has not changed.  

* Percent Passing Math slightly moved from 73.48% to 73.46%.  
* Percent Passing Reading only slightly moved as well from 84.39 to 84.31
* Overall Passing Percent dropped from 62.86% to 62.78%


## Scores by school size
![School Size PNG](https://github.com/MXV0921/School_District_Analysis/blob/main/Resources/school_size_bins.png)
There was no change in the results based on school size.  Because of the large size of the data sample, the adjustment that affected Thomas High School 9th grade was not large enough to change the results of the large bins we created by sorting school size.

## Scores by school type
![School Type PNG](https://github.com/MXV0921/School_District_Analysis/blob/main/Resources/School_type_summary.png)
Similar to the school size sorting of data, the 
# Summary: 
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
