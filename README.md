# MCAS watertown public school score  analysis 
 This project emphasizes an analysis in order to indicate if Watertown public schools have an impact of socio econominc factors such as race and econnomic distress while performing well at the MCAS involving subjets , math , ELA and STE . This is done to obeserve if these scores pf 2018-19 are impacted by such factors and what re the important factors that contribute to that score.  
 
# cleaning the data 
The student  id and ssid has to  be merged to gauage factors such  as race and economic distress  to form the merged dataset 

After that null  values are  categorical  and hence they are replaced by frequenlty occuring values usin DataImputer() and Transformixin
rather than using one hot encoding 

# prediction model creation
The models used  in order to  achieve this are linear regression and neural networks as we are dealing with continous  variables 

# Conclusion:
It was found out that important factors were actually the patter innvolved in grading and race and socio- economic disadvantage didnt contibute significantly according to the linear regression model . But it was also known that for every student as a pacific islander they can score a grade of 2 units more in math in comparision to other students and mixed racial students have the ability to secure a grade higher than other race students when it came to english.
