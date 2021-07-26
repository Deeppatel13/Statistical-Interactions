# PEARSON'S CORRELATION

This assignment aims to statistically assess the evidence, provided by NESARC codebook, in favor of or against the association of number of Cigarettes smokers (Explanatory Variable) and 
both largest number of beers consumed and age on onset of first episode on Dysthymia (Response Variable). More specifically, since my research question includes only categorical variables, 
I selected three new quantitative variables from the NESARC codebook. Therefore, I redefined my hypothesis and examined the correlation between the age when the individuals started smoking 
everyday (S3AQ51) and both largest number of beers consumed on days when drank beer in last 12 months(S2AQ5E) and age on onset of first episode of Dysthymia(S4CQ5). As a result, in the 
first place, in order to visualize the association between Cigarettes smokers and both numbers of beers consumed on days when drank beer in last 12 months and age on onset of first episode 
of Dysthymia, I used seaborn library to produce a scatterplot for each response variables separately and interpreted the overall patterns, by describing the direction, as well as the form 
and the strength of the relationships. In addition, I ran Pearson correlation test (Q->Q) twice and measured the strength of the relationships between each pair of quantitative variables, 
by numerically generating both the correlation coefficients r and the associated p-values. For the code and the output I used Jupyter notebook (IDE).

The three quantitative variables that I used for my Pearson correlation test are:
![img1](https://64.media.tumblr.com/c55c20713678ffbb4161467421f52612/88282302b6603274-fc/s1280x1920/596bbc4779e445a7414b97112360d4cdd1fb879e.png)
![img](https://64.media.tumblr.com/8ed313a4de60d955f3f1e351b56230f9/88282302b6603274-66/s1280x1920/c85c102048e0eb2ad9a8c2953df862f8a8039a26.png)
![img3](https://64.media.tumblr.com/c45dae4aa1d3c7072d6e34d1ce82689f/88282302b6603274-4b/s1280x1920/c12df1c0dfce2a21b744372415d56081f0623fa3.png)

### OUTPUT:
![img4](https://64.media.tumblr.com/c0fc0dca2fcf88245fa149530f796d3d/88282302b6603274-d3/s1280x1920/9c417a8c611d1a0fe5e5792e13dd5c60d1fd1d7a.png)

The scatterplot presented above, illustrates the correlation between the age when started smoking cigarettes everyday (quantitative explanatory variable) and the largest number of beers 
consumed on days when drank beer in the last 12 months (quantitative response variable). The direction of the relationship is positive (increasing), which means that an increase in the age 
when started smoking cigarettes everyday is associated with an increase with the largest number of beers consumed on days when drank beer. In addition, since the points are scattered about 
a line, the relationship is linear. Regarding the strength of the relationship, from the pearson correlation test we can see that the correlation coefficient is equal to 0.11, which 
indicates a fairly weak linear relationship between the two quantitative variables. The associated p-value is equal to 9.40e-25 (p-value is written in scientific notation) and the fact that 
its very small means that the relationship is statistically significant. As a result, the association between the age when started smoking cigarettes everyday and the largest number of beer
s consumed on days when drank beer in the last 12 months is moderately weak, but it is highly unlikely that a relationship of this magnitude would be due to chance alone. Finally, by 
squaring the r, we can find the fraction of the variability of one variable that can be predicted by the other, which is fairly at 0.05.

![img5](https://64.media.tumblr.com/61a77850dc051ea7855e37d5219720ba/88282302b6603274-a1/s1280x1920/78a8dd6f00883ff3d6505326d817f044f0161a18.png)

For the association between the age when started smoking cigarettes everyday (quantitative explanatory variable) and the age when experienced the first episode of Dysthymia (quantitative 
response variable), the scatterplot presented above shows a positive linear relationship. Regarding the strength of the relationship, the pearson correlation test indicates that the 
correlation coefficient is equal to 0.17, which is interpreted to a weak linear relationship between the two quantitative variables. The associated p-values is equal to 4.54e-10 (p-value 
is written in scientific notation), which means that the relationship is statistically significant. Therefore, the association between the age when started smoking cigarettes everyday and 
the age when experienced the first episode on Dysthymia is weak, but it is highly unlikely that a relationship of this magnitude would be due to chance alone. Finally, by squaring the r, 
we can find the fraction of the variability of one variable that can be predicted by the other, which is very low at 0.05.