---
layout: default
title: 3. Empirical Results
parent: § The Volatility Implications of the Chinese Cryptocurrency Ban 
grand_parent: T 
nav_order: 30 
---
<style>
.dont-break-out {
  /* These are technically the same, but use both */
  overflow-wrap: break-word;
  word-wrap: break-word;

     -ms-word-break: break-all;
  /* This is the dangerous one in WebKit, as it breaks things wherever */
  word-break: break-all;
  /* Instead use this non-standard one: */
  word-break: break-word;
}

.youtube-container {
    position: relative;
    width: 100%;
    height: 0;
    padding-bottom: 56.25%;
}
.youtube-video {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}

</style>

<div class="dont-break-out" markdown="1">

1. TOC
{:toc}

## 3. Empirical Results
### *3.1. Correlation Matrix*

To begin the analysis, I first look at a simple pooled correlation matrix of all the variables used in the study. Table 2 reports the pooled Pearson correlation coefficients between price, volume, volatility, and illiquidity. Price and Volume have a correlation coefficient of 0.3728, which is statistically significant. I expected *price* and *volume* to have a positive correlation because the lower priced coins are usually the less popular coins. *Price* and *Rvolt* have a correlation coefficient of -0.0674, which is also statistically significant. This is expected because as volatility increases, I expect that to have a negative impact on the price variable. *Price* and *Illiq* have a correlation coefficient of -0.0247 and is statistically significant. The likely reason they have a negative correlation coefficient is because an illiquid currency has a negative effect on price because of its’ inefficiencies in trading. *Volume* and *Rvolt* have a correlation coefficient of -0.0374, which is statistically significant. I expect this negative correlation given that the more stable currencies usually trade more often. *Volume* and *Illiq* have a correlation coefficient of 0.2508 and is statistically significant. This is expected because more volume would suggest that the crypto is less illiquid. This unexpected result might be caused by the relationship between dollar volume and price. *Rvolt* and *Illiq* has a correlation coefficient of 0.2508 and is statistically significant. This is likely due to fact that the more volatile the coin, the less liquidity in the crypto.

### *3.2. Univariate Tests*
To dig deeper into the variable of interest, *Rvolt*, I conduct a univariate analysis around three different time windows surrounding May 18, 2021 – the Chinese ban date. The results of this analysis are in Table 3. Here, I estimate the means and medians of crypto volatility during the periods before and after the event. I then examine the difference of the means and medians using t-statistics and Wilcoxon sum rank tests. The first event window consists of the five days before and after the ban. The difference in mean volatility during the pre- and post-event periods is 0.1685, which is statistically significant at the .01 level and has a t-statistic of 31.63. The difference in median during this same timeframe is 0.1759 and is also statistically significant at the .01 level. The implications of this result are clear. There seems to be a large short-term effect of the Chinese ban on the volatility of cryptocurrencies. In economic terms, these results suggest that volatility approximately doubled in response to the ban.

The question then shifts to whether or not the ban has a lasting impact on the volatility of cryptos. To test this possibility, I replicate my tests using the ten days before and after the event. The difference in means during this period is 0.0849, and the difference in medians is 0.0634. Again, the test statistics suggest that the differences are statistically significant at the 0.01 level. The results are muted quite a bit when adding only an extra five days to the event window. However, there is still an economic effect, and in a medium length time window, I can still say that the ban of crypto transactions in China had an effect on volatility on the crypto market as a whole. When looking at the 40 days before and after the ban, the difference in means for this event window is 0.0143, and the difference in the medians is 0.0038. These are also statistically significant at the .01 level. Although the 40-day time range has statistical significance it has severely less economic significance. What I can conclude from these univariate tests is that volatility increased dramatically during the time of the ban, but leveled out quickly after the event and went back to previous volatility levels.

I provide graphical representation of volatility surrounding the ban in Figure 1. The results from this simple analysis confirm what I have learned through the univariate tests discussed previously. This graph shows a huge spike in volatility on the day of the announcement. After the event, volatility stays unusually high for a few days then appears mean revert. In the second panel of Figure 1, I plot the price on the y-axis and event days on the x-axis. Price drops on the day of the event and appears to continue to decrease for the rest of the time period.

### *3.3. Multivariate Tests*
To better understand the effect of the ban on crypto volatility, I conduct a multivariate analysis, which is reported in Table 4. More specifically, I estimate the following regression equation on a panel of crypto-day observations:

𝑅𝑣𝑜𝑙𝑡𝑖,𝑡 = 𝛼 + 𝛽<sub>1</sub>𝑃𝑜𝑠𝑡𝑡 + 𝛽<sub>2</sub>𝐿𝑁(𝑃𝑟𝑖𝑐𝑒𝑖,𝑡) + 𝛽<sub>3</sub>𝐿𝑁(𝑉𝑜𝑙𝑢𝑚𝑒𝑖,𝑡) + 𝛽<sub>4</sub>𝐼𝑙𝑙𝑖𝑞𝑡 + 𝜀𝑖,𝑡

,where *Rvolt* is the measure of range- based volatility. *Post* is an indicator variable equal to one on days after the announcement of the Chinese ban and zero otherwise. We include as control variables, the natural log of price and volume as well as Amihud’s (2002) measure of illiquidity. We have taken the natural log of the price and volume variables to help normalize the distribution of both of these variables. This regression allows me to test whether the event has any effect on the volatility of cryptos while controlling for other important factors, such as price, volume, and illiquidity. To help with possible heteroskedasticity, I report heteroskedastic robust standard errors. I again look at the three different periods surrounding the ban.

First, I look at the five days before and after the event. The intercept for the regression is 0.064 with a 7.10 t-statistic and a .10 significance level. *Post* has a 0.1647 coefficient with a 32.49 t-statistic and a .01 significance level. This means that, on average, volatility is 0.1647 greater in the five days after the event then before the event. So even when controlling for price, volume and illiquidity, the event still effects the volatility of cryptos in the short term. Regarding the control variables, the *LN(price)* variable has a -.0079 coefficient with a corresponding t-statistic of -7.81, which is statistically significant at the .01 significance level. This coefficient suggests that if we increase price by one percent we expect volatility to decrease by .0079 units. This variable is not economically significant and does not give us any real insights. The *LN(volume)* variable produces a coefficient of 0.0052 with a t-statistic of 6.95. This result indicates that an increase in volume by one percent increases volatility by 0.0052 units. Like *LN(price),* this variable is not economically significant either and does not provide us with important insights. The *Illiq* variable has a 0.0084 coefficient and a 7.93 t-statistic, which suggests that *Illiq* is statistically significant at the .01 level. This result indicates that a one unit increase in illiquidity has a 0.0084 unit increase in volatility. The findings for this coefficient is also economically insignificant as well. This model had 3,956 observations and had an adjusted R-squared as 0.2366 suggesting that the model explains 23.66% of the variation in volatility.

Next, I examine the ten days before and after the Chinese ban to see if controlling for these variables has any differing effect on volatility in the medium term. The intercept coefficient is 0.1136 and has a t-statistic of 13.44, which is statistically significant at the .01 significance level. Again, the *Post* variable has a coefficient of 0.0819 and a t-statistic of 22.67, which is significant at the .01 significance level. This result suggests that the time after the event has a 0.0819 higher volatility, on average, when compared to the pre-event period. Again, I find that after controlling for price, volume and illiquidity, there is a moderate economic effect on the volatility due to the event. I will not review the coefficients of the control variables here as they had no significant change when I examined the different time period. This model had 7,554 observations and an adjusted R-squared of 0.1159.

Given the univariate analysis – conducted in the previous subsection – I next determine whether controlling for price, volume and illiquidity variables had any change in the post-event variable in the long-term of forty days before and after the event. The intercept for this model is 0.1657 and has a t-statistic of 39.86. The *Post* variable has a coefficient of .0083 and has a tstatistic of 4.85 and is statistically significant at the .01 significant level. This result indicates that, relative to the pre-event window, volatility is .0083 greater after the event, which is not very economically significant. I find that as the longer the event window is, the less economically significant the *Post* variable becomes. This confirms what I learned in the univariate analysis as the event impacted the volatility in the short term, but as time went on, the volatility returned to pre-event levels. The intercept follows the opposite trend as we might predict because all the other variables are very similar. The intercept starts to explain the volatility instead of the post variable, this simply means that volatility is explained more by a constant as time goes on or another explanatory variable we have not included in our model. I note that there are 29,016 observations used in this analysis and the adjusted R-squared is 0.0711. The R-squared has also decreased significantly which means the model is explaining less when looking longer term.

***

#### Table of Contents
{: .no_toc}

<ul><li> <a href="/docs/T/The-Volatility-Implications-of-the-Chinese-Cryptocurrency-Ban-1/">
1. Introduction</a></li><li> <a href="/docs/T/The-Volatility-Implications-of-the-Chinese-Cryptocurrency-Ban-2/">
2. Data Description</a></li><li> <a href="/docs/T/The-Volatility-Implications-of-the-Chinese-Cryptocurrency-Ban-3/">
3. Empirical Results</a></li><li> <a href="/docs/T/The-Volatility-Implications-of-the-Chinese-Cryptocurrency-Ban-4/">
4. Concluding Remarks</a></li><li> <a href="/docs/T/The-Volatility-Implications-of-the-Chinese-Cryptocurrency-Ban-5/">
References</a></li></ul>

***

</div>
