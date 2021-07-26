# CHI_SQUARE TEST OF INDEPENDENCE

This assignment aims to directly test my hypothesis by evaluating, based on a sample of 4946 U.S. which resides in South region(REGION) aged between 25 to 40 years old(subsetc1), my 
research question with a goal of generalizing the results to the larger population of NESARC survey, from where the sample has been drawn. Therefore, I statistically assessed the evidence, 
provided by NESARC codebook, in favor of or against the association between Cigars smoked status and fear/avoidance of heights, in U.S. population in the South region. As a result, in the 
first place I used crosstab function, in order to produce a contingency table of observed counts and percentages for fear/avoidance of heights. Next, I wanted to examine if the Cigars 
smoked status (1= Yes or 2=no) variable ‘S3AQ42′, which is a 2-level categorical explanatory variable, is correlated with fear/avoidance of heights (’S8Q1A2′), which is a categorical 
response variable. Thus , I ran Chi-square Test of Independence(C->C) and calculated the  χ-squared values and the associated p-values for our specific conditions, so that null and 
alternate hypothesis are specified. In addition, in order visualize the association between frequency of cannabis use and depression diagnosis, I used catplot function to produce a 
bivariate graph. Furthermore, I used crosstab function once again and tested the association between the frequency of cannabis use (’S3BD5Q2E’), which is a 10-level categorical explanatory 
variable. In this case, for my second Test of Independence (C->C), after measuring the χ-square value and the p-value, in order to determine which frequency groups are different from the 
others, I performed a post hoc test, using Bonferroni Adjustment approach, since my explanatory variable has more than 2 levels. In this case of ten groups, I actually need to conduct 45 
pair wise comparisons, but in fact I examined indicatively two and compared their p-values with the Bonferroni adjusted p-value, which is calculated by dividing p = 0.05 by 45. By this way 
it is possible to identify the situations where null hypothesis can be safely rejected without making an excessive type 1 error. For the code and the output I used Jupyter Notebook(IDE).

![img1](https://64.media.tumblr.com/532eb794cadc631866a823170d6c59fd/459ea6cb7ded2835-37/s1280x1920/7f31137d9bf850c41d3b9f63c659247048f4e850.png)

When examining the patterns of association between fear/avoidance of heights (categorical response variable) and Cigars use status (categorical explanatory variable), a chi-square test of 
independence revealed that among aged between 25 to 40 in the South region(subsetc1), those who were Cigars users, were more likely to have the fear/avoidance of heights(26%), compared to 
the non-users(20%), X2=0.26,1 df, p=0.6096. As a result, since our p-value is not smaller than 0.05(Level of Significance), the data does not provide enough evidence against the null 
hypothesis. Thus, we accept the null hypothesis , which indicates that there is no positive correlation between Cigar users and fear/avoidance of heights.

![img2](https://64.media.tumblr.com/c20a3ee35b4259a840e2a68a6917c77e/459ea6cb7ded2835-dc/s1280x1920/926f582575f7661056b88d2ca7f5b888771b58f3.png)

A Chi Square test of independence revealed that among cannabis users aged between 18 to 30 years old (susbetc2), the frequency of cannabis use (explanatory variable collapsed into 10 
ordered categories) and past year depression diagnosis (response binary categorical variable) were significantly associated, X2 = 30.99,9 df, p=0.00029.

![img3](https://64.media.tumblr.com/f23452a8814aefc6bc3d46a0bca8a63d/459ea6cb7ded2835-92/s500x750/1e0f2558eeef1e07be687e012e7e316724cd3a63.png)

In the bivariate graph(C->C) presented above, we can see the correlation between frequency of cannabis use (explanatory variable) and major depression diagnosis in the past year (response 
variable). Obviously, we have a left-skewed distribution, which indicates that the more an individual (18-30) smoked cannabis, the better were the cases to have experienced depression in 
the last 12 months.

![img4](https://64.media.tumblr.com/d55cfec04d75b708989d798b04911a8c/459ea6cb7ded2835-ca/s1280x1920/71d629a330cc7123dfc7b4656b895d1810f6c252.png)

The post hoc comparison (Bonferroni Adjustment) of rates of major depression by the pair of “Every day” and “2 times a year” frequency categories, revealed that the p-value is 0.00019 and 
the percentages of major depression diagnosis for each frequency group are 23.7% and 11.6% respectively. As a result, since the p-value is smaller than the Bonferroni adjusted p-value 
(adj p-value = 0.05 / 45 = 0.0011>0.00019), we can assume that these two rates are significantly different from one another. Therefore, we reject the null hypothesis and accept the 
alternate.

![img5](https://64.media.tumblr.com/67c09a7af24c61b27c30183391059574/459ea6cb7ded2835-09/s1280x1920/1604a11b6d220823358f644c0acc280902745695.png)

Similarly, the post hoc comparison (Bonferroni Adjustment) of rates of major depression by the pair of "1 or 2 times a week” and “2 times a year” frequency categories, indicated that the 
p-value is 0.107 and the proportions of major depression diagnosis for each frequency group are 17.1% and 11.6% respectively. As a result, since the p-value is larger than the Bonferroni 
adjusted p-value (adj p-value = 0.05 / 45 = 0.107>0.0011), we can assume that these two rates are not significantly different from one another. Therefore, we accept the null hypothesis.

