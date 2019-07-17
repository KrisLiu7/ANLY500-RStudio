# ANLY500-RStudio
All the projects are using RStudio/R  Lab3 and 4 all use linear regression model, however lab4 use much more complicated and plus a Hierarchical Linear Modeling(HLM), as Multiple linear regression(MLR).

# Lab1b Correlations research of memory & mental abilities
The purpose of this short project is to compare the effectiveness of two typing programs for a teacher. She divides the 100 students into two group. So, we are using the Z-Test in R to determine the confidence interval and sample mean. Then comparing the standard error and effect size for each group.

# Lab3 Maximizing parking capacity & utilization
This project is targeted to solve the park problem and maximize the parking capacity in the campus for Missouri State University. These 350 students are given some short questions about their perception/reason of parking in campus. So the data would include with some demographic information like Gender, Class Level. And if they think MSU need additional parking.
#Data Screening# first. Data screening is a process to clean the data, making these data being reliable and usable. Data screening has several processes.
For the data accuracy, we check the categorical data.
For the missing data, we check the null value and remove them.
For the outliers(outliers are these data which may incorrect and effect your accuracy. Reason of outliers are like: people type wrong answer, people choice without reason, etc.). We need to use Mahalanobis' distance based on a Chi-Square distribution, then we would find the cutoff score. 
 Next one is about #Assumption#. There are several common types assumptions in statistic, for this project we test:
Additivity, Include the symnum bivariate correlation table for continuous measures.
Normality, using kurtosis and skewness to test the multivariate normality.
Homogeneity/Homoscedasticity, build the plot and scale to check the homogeneity.

# Lab4 Correlations research of memory & mental abilities
The study is finding the associations between working memory and both reading and math abilities. The possible factors are intelligence, verbal abilities , short term memory and phonological awareness. The sample are these disabilities of 6-11 years old child. This sample people have deficits in complex memory and visuospatial STM and low IQ scores. So we are trying to make contribution of working memory to learning ,and help for educational practice in the future. 
In #Data Screening#, we check the outliers using Leverage cut off score and Cook’s cut off score.
The leverage cut off score, we using the “lm” function to build the linear regression model to help us get the leverage cut off score. Then we use Cook’s distance then Mahalanobis distance to get each outlier. (So we are using three method to get outliers, like bad data or error data)
Then we clean these outliers.
 # Hierarchical Regression
They we move to Hierarchical Linear Modeling(HLM), one kind of the Multiple linear regression(MLR). We build three model and run the Anova test, compare the F-Statistic and P value so get the best model from them. The result prove that “Math” has a significant positive influence on “Reading”. 
 # Moderation
Examine the interaction between verbal and math scores predicting reading scores. (Build the linear model of Data and Reading)
Build the linear model for low, average, and high math levels (split on math) for verbal predicting reading.
Generate the graph of the interaction.
The result is: The stronger the mathematics ability, the more the reading skill is reduced by 0.0005 units for each additional unit of verbal ability. In other words, there is an interaction between mathematical ability and verbal ability.
