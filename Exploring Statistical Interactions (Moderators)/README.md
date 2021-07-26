# EXPLORING STATISTICAL INTERACTIONS

This assignment aims to statistically assess the evidence, provided by NESARC codebook, in favor of or against the association between alcoholic drinkers and Final weight. More specifically,
I examined the statistical interaction between individuals who drank at least 1 alcoholic drink in life (2-level categorical explanatory ,S2AQ1) and Final Weight of individuals 
(quantitative response variable, WEIGHT (measured in Weighting factor)), moderated by variable “SOCPDX12”(Categorical), which indicates people having social phobia in the last 12 months. 
This effect is characterized statistically as an interaction, which is a third variable that affects the direction and/or the strength of the relationship between the explanatory and the 
response variable and help us understand the moderation. Since I have a categorical explanatory variable (Individuals who drank at least 1 alcoholic drink in life) and a quantitative 
response variable (Final Weight), I ran ANOVA (Analysis of Variance) test to examine the patterns of the association between them (C->Q),by directly measuring the F-statistic value and 
the p-value. In addition, in order visualize graphically this association, I used catplot function (seaborn library) to produce a bivariate graph. Furthermore, I took 2-level categorical 
variable, therefore, I did not perform the post hoc test, using Tukey hsd approach.

Regarding the third variable, I examined if individuals having social phobia in the last 12 months, moderates the significant association between individuals who drank at least 1 alcoholic 
drink in life and Final Weight of individuals. Put it another way, are individuals who drank at least 1 alcoholic drink in life related to Final Weight of individuals for each level of 
moderating variable (0=No and 1=Yes), that is for individuals who did not have social phobia in last 12 months and for individuals who had? Therefore, I set new data frames (sub2 and sub3) 
that include either individuals who fell into each category (Yes or No) and ran the Analysis of Variance(ANOVA) for each subgroup separately, measuring both the F-statistics and the p-values
. Finally, with catplot function (seaborn library) I created two bivariate bar graphs, one for each level of the moderating variable, in order to visualize the differences and the effect of 
the moderator upon the statistical relationship between individuals who drank at least 1 alcoholic drink in life and Final Weight of individuals. For the code and the output I used Jupyter 
notebook (IDE).

The moderating variable that I used for the statistical interaction is:
![img1](https://64.media.tumblr.com/4c3cc4ca9b82db2347d9ed6a97316dab/36fc9b4c455ecaca-8b/s1280x1920/27bc37b46d9a37d2b12324bb4e229ee5e2c1e515.png)

### OUTPUT
![img2](https://64.media.tumblr.com/b43c80c5dc68b8189991d3c781205f1f/36fc9b4c455ecaca-57/s1280x1920/114cbc8953fb67513bffda8f37f245e459f8c556.png)

An Analysis of Variance(ANOVA) test revealed that from the NESARC codebook, the individuals who drank at least 1 alcoholic drink in life (2-level categorical explanatory variable) and Final 
Weight of individuals (quantitative response variable) were significantly associated, F=194.3, 1 df, p=4.52e-44 (where p-value is written in scientific notation).

![img3](https://64.media.tumblr.com/2e6081dc1db746aec6a1f1139a9b79c8/36fc9b4c455ecaca-d0/s500x750/7a7d82e85b7e7013d0cf1fec06fa056ba94668f4.png)

In the bivariate graph (C->Q) presented above, we can see the correlation between individuals who drank at least 1 alcoholic drink in life (explanatory variable) and Final Weight of 
individuals (response variable). Thus, it is explained in the above graph that individuals who drink alcohol gain more weight than those who don’t drink alcohol.

![img4](https://64.media.tumblr.com/807698fb7f94d08fb0e89bc0fbdd0858/36fc9b4c455ecaca-8f/s1280x1920/a9de316db3c25c204c58d0fe377582c49e83f1a3.png)

In the first place, for the moderating variable equal to 0, which is individuals who don’t have social phobia in last 12 months (sub2), a Analysis of Variance(ANOVA) test revealed that 
among the NESARC codebook, the individuals who drank at least 1 alcoholic drink in life (explanatory variable) and Final Weight of individuals (response variable) were significantly 
associated, F=200.6,1 df, p=1.99e-45 (where p-value is written in scientific notation). As a result, since the F-statistic value is very large and the p-value is significantly small, we 
can assume that there is a strong positive relationship between these two variables, when taking into account the subgroup of individuals who did not have social phobia in the last 12 
months.

![img5](https://64.media.tumblr.com/0473773667b213782346b7e73eb6b04d/36fc9b4c455ecaca-85/s500x750/5a4b7c2b699435caae3c21e3d98870853eb3349e.png)

In the bivariate bar graph (C->Q) presented above, we can see the correlation between the individuals who drank at least 1 alcoholic drink in life (explanatory variable) and Final Weight 
of individuals (response variable), in the subgroup of individuals who did not have social phobia in the last 12 months(sub2). Obviously, it shows a positive relationship between these two 
variables, which means that the individuals who drank at least 1 alcoholic drink in life directly affects the Final weight of individuals, regarding the individuals who did not have social 
phobia in the last 12 months.

![img6](https://64.media.tumblr.com/b38ad2ead2b58b1b130b334dd8314b70/36fc9b4c455ecaca-c1/s640x960/0bba7114beedf799ccd7ffc24b98276af371f2c0.png)

Secondly, for the moderating variable equal to 1, which is those  individuals who had social phobia in the last 12 months (sub3), an Analysis of Variance(ANOVA) test revealed that among 
NESARC codebook, the individuals who drank at least 1 alcoholic drink in life (explanatory variable) and Final Weight of individuals (response variable) were not significantly associated, 
F=1.036,1 df, p=0.309. As a result, since the F-statistic value is quite small and the p-value is significantly large, we can assume that there is no statistic relationship between these 
two variables, when taking into account the subgroup of individuals who had social phobia in the last 12 months.

![img7](https://64.media.tumblr.com/dc88b1dc35c13d2fdcc6b5aef1e82430/36fc9b4c455ecaca-a8/s500x750/74df0ae035930dcf6c08a208df995ff345dfdee2.png)

In the bivariate bar graph (C->Q) presented above, we can see the correlation between individuals who drank at least 1 alcoholic drink in life (explanatory variable) and Final Weight of 
individuals (response variable), in the subgroup of individuals who had social phobia in the last 12 months (sub3). In fact, there is no positive relationship between these two variable, 
for those who had social phobia in the last 12 months.

### SUMMARY:
It seems that both the direction and the size of the relationship between individuals who drank at least 1 alcoholic drink in life and Final Weight of individuals, is heavily affected by 
social phobia in the last 12 months. In other words, the individuals who had social phobia in the last 12 months, the correlation is considerably weak, whereas who did not have social 
phobia, the correlation is significantly strong and positive. Thus, the third variable moderates the association between individuals who drank at least 1 alcoholic drink in life and Final 
Weight of individuals.