# An Analysis of Kickstarter Campaigns
Performing analysis on Kickstarter data to uncover trends

# Kickstarter Challenge – Written Analysis

##Overview of Project

###Purpose:
The purpose of this project is to compare the play ‘Fever’ in relation to other works in different categories using a data set of over 4000 works. Louise’s play ‘Fever’ had a goal of $2,885.00 but was only 86% funded at $2,485.00. She wants to know other campaign performance compared to hers based on their launch dates and funding goals. We will perform these analyses to see how others stack up against hers.   

##Analysis and Challenges
To help perform this analysis, the date set was cleaned up by converting UNIX data stamp information to a more readable date format using the formula =(((J4110/60)/60)/24) +DATE (1970,1,1). We isolated the year using the excel formula “=Year ()” and with the new manageable date format, we were able to determine success rates based on the identified categories in the data set. We determined that there were 1,369 project lunch in the Theater category which is the same category as Louise’s play.

##Results

###Analysis of Outcomes Based on Launch Date:

***-What two conclusions can you draw-***
From the analysis we conducted, we categorized data under the number of projects cancelled, failed and successful by months. The two conclusions from the analysis showed that the most successful theater projects were launched in May and began to decline in June. There was a steep decline in projects’ success rate. Secondly, while it shows graphically that the highest failure rate was in October due to the sharp increase from September, the greatest failure rate occurred in May. This also happened to be the period with the most project launch.

###Analysis of Outcomes Based on Goals:

***-What can you conclude about the Outcomes based on Goals?-***
The data set fund was grouped into twelve goal ranges and four categories - successful, failed, live, and cancelled. Using the “COUNTIFS” function, (COUNTIFS(Kickstarter!$F:$F,"successful",Kickstarter!$D:$D,"<1000",Kickstarter!$R:$R,"plays") we categorized project outcome goals under these categories. Also, the SUM(B2:D2) function helped to derive the project totals under each group and the percentage of totals. The most successful project had goals between $1,000 to $4,999 while plays with goals between $45,000 and $49,999 recorded the highest failure. We can conclude from this that putting in more money into a project does not equal success. 

***-What are some limitations of this dataset?:-*** 
The data set is a sample size from across the world and may not be a true representation of the entire population. Also, there are several outliers in the data set that may have skewed the statistic far to the left.

***-What are some other possible tables and/or graphs that we could create?-*** 
Other possible tables and/or graphs that we could create include an Area chart that shows the concentration of successes, etc. a Bar Chat or a histogram that could easily represent the skewness of the population mean.
