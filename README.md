# School_District_Analysis


## Overview of the project

  The school board asked us to analyze a school district after adjusting the grades in one of the schools. The board wants to know how the changed grades affected the average grades in the district. It was also requested to compare average grades among schools based on certain metrics such as, school size, budgeting, etc. Average math and reading grades for THS also dropped, but not as much as the passing rate.
  

## Results

  - Having replaced the grades of the cheating students with NaN and ran the analysis again, we can see that Thomas High School has dropped by approximately 0.3 point it's passing rate for math, reading and overall. 
  - If we look compare the results based on budgeting per student, we can see that number only changed for $630-$644 range, which is explained by THS falling into that range with it's $638 per student spendings.
  - We can also notice that, suprisengly, schools with smaller budgets per student tend to perform better on overall passing scores.
  - If we look at the analysis of the district based on the size of the schools, we can see that average for Medium size schools, the size of THS, drop on average 0.01 to 0.05 point.
  We can also notice that medium size schools perform a lot better than other size schools, based on all numbers.
  THS along with the rest of the charter type schools also dropped between 0.01 and 0.03 pints on all average numbers, while the district type schools stayed the same.
  Having looked through the numbers and analysis we can conclude that Math and Reading scores got affected negatevily by replacing the ninth-grade scores and both dropped points. Scores by school spending, as well as school size and type have all lost in their value due to replacing the ninth-grade scores.


## Summary

  As was mentioned earlier in the report, having ran the analysis we see a negative change in both Math and Reading scores due to the replacement of the ninth-grade scores. Scores by school spending, as well as school size and type have all lost in their value due to replacing the ninth-grade scores.
  One of the challenging parts of this project was using the .loc just like in this example:
       
       "total_THS_pmath = student_data_df.loc[(student_data_df["school_name"] == "Thomas High School") & 
                                                            (student_data_df["math_score"]>=70) & 
                                                            ((student_data_df["grade"] == "10th")|
                                                             (student_data_df["grade"] == "11th")|
                                                        (student_data_df["grade"] == "12th"))].count()["student_name"]

         percentage_THS_pass_math = total_THS_pmath / total_THS_10_12 * 100"

  I was able to overcome this challenge by looking up documentation and applying different methods.
