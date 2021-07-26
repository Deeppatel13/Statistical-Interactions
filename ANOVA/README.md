# ANALYSIS OF VARIANCE (ANOVA)

This assignment aims to directly test my hypothesis by evaluating, based on a sample of 2051 U.S. candidates who drink when they are not with family(H1TO13) and are White(H1GI6A) OR 
American Indian or Native American(H1GI6B) in race(subset1), my research question with the goal of generalizing the results to the larger population of ADDHEALTH survey, from where the 
sample has been drawn. Therefore, I statistically assessed the evidence, provided by  ADDHEALTH codebook, in favor of or against the association between Drinkers and Special Romantic 
Relationship, in U.S. population. As a result, in the first place I used the OLS function in order to examine if Special Romantic Relationship in the past 18 months(H1RR1), which is a 
categorical explanatory variables, is correlated with the quantity of drinks an individual had each time during the past 12 months(H1TO16), which is a quantitative response variable. Thus, 
I ran ANOVA (Analysis of Variable) method (C- >Q) once and calculated the F-statistics and the associated p-values, so that null and alternate hypothsis are specified. Furthermore, I used 
OLS function once again and tested the association between frequency of drinks had during the past 12 months(H1TO15),which is a 6-level categorical explanatory variable, and the quantity 
of drinks a particular had each time during the past 12 months(H1TO15),which is a quantitative response variable. In this case, for my second one-way ANOVA(C- >Q),after measuring the 
F-statistic and the p-value, I used Tukey HSDT to perform a post hoc test, that conducts post hoc paired comparisons in the context of my ANOVA, since my explanatory variable has more 
than 2 levels. By this way it is possible to identify the situations where null hypothesis can be safely rejected without making an excessive type 1 error. In addition, both means and 
standard deviations of quantity response variable, were measured separately in each ANOVA, grouped by the explanatory response variables using the groupby function. For the code and the 
output I used Jupyter Notebook (IDE).

### OUTPUT:
![img1](https://64.media.tumblr.com/dd3d048548de2468784ccb98860df492/79980301fee51d7c-70/s1280x1920/92cf454c55e675edd6e6f317d32bf1580783d66f.png)

When examining the association between the number of drinks had each time (quantitative response variable) and Special Romantic Relationship (categorical explanatory variable), an Analysis 
of Variance(ANOVA) revealed that drinkers when not with family and are American Indian or Native America in race(subset1), those with Special Romantic Relationship reported drinking 
marginally equal quantity of drinks each time (Mean=6.34,s.d.  ±7.33) compared to those without Special Romantic Relationship(Mean=5.67,  ±6.35) , F(1,1779)=3.016, p=0.0862>0.05. As a 
result, since our p-value is significantly large, in this case the data is not considered to be surprising enough when the null hypothesis is true. Consequently, there are not enough 
evidence to reject the null hypothesis and accept the alternate, thus there is no positive association between Special Romantic Relationship and quantity of drinks had each time.

![img2](https://64.media.tumblr.com/bc321158b60e9f62e22059c4007cb8dc/79980301fee51d7c-1d/s1280x1920/1be05cb254103635ffb1f982d00bb58fb83dc788.png)
![img3](https://64.media.tumblr.com/e1130eac2006a8422de50f4da73f5188/79980301fee51d7c-ee/s640x960/bbd39d53f3e15387975c474cd6d05b2f5f21b719.png)

ANOVA revealed that among U.S. population who drink when they are not with family(H1TO13) and are White(H1GI6A) OR American Indian or Native American(H1GI6B) in race(subset1), frequency of 
drinks on days(collapsed into 6 ordered categories, which is the categorical explanatory variable) and quantity of drinks had each time per day (quantitative response variable) were 
relatively associated, F(5,1777)=27.63, p=5.09e-27<0.05 (p value is written in scientific notation). Post hoc comparisons of mean number of drinks each time by pairs of drinks frequency 
categories, revealed that those individuals drinking every day (or 3 to 5 days a week) reported drinking significantly more on average daily (every day: Mean=10.27, s.d.  ±9.47, 3 to 5 days 
a week: Mean=8.26, s.d.  ±5.57)  compared to those drinking 2 or 3 days a month (Mean=7.29, s.d.  ±8.16), or less. As a result, there are some pair cases in which frequency and drinking 
quantity of drinkers, are positive correlated.

![img4](https://64.media.tumblr.com/88a8888333d1ae3c126e69e04ed001b7/79980301fee51d7c-40/s540x810/6cce887a86c47a2e3739d681d3334839bc0ee2e5.png)

In order to conduct post hoc paired comparisons in the context of my ANOVA, examining the association between frequency of drinks and number of drinks had each time, I used the Tukey HSD 
test. The table presented above, illustrates the differences in drinking quantity for each frequency of drinks use frequency group and help us identify the comparisons in which we can 
reject the null hypothesis and accept the alternate hypothesis, that is, in which reject equals true. In cases where reject equals false, rejecting the null hypothesis resulting in 
inflating a type 1 error.