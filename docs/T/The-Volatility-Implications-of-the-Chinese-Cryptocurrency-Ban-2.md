---
layout: default
title: 2. Data Description
parent: § The Volatility Implications of the Chinese Cryptocurrency Ban 
grand_parent: T 
nav_order: 20 
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

## 2. Data Description
The data used in the analysis come from 372 different cryptocurrencies during an 80-day period (40 days before and 40 days after) surrounding the Chinese ban of crypto transactions on May 18th, 2021. I obtain daily pricing and volume data from the largest cryptos, like Bitcoin, as well as smaller coins in order to capture a broad crypto market trend. The data is obtained from *CoinMarketCap*. The daily price variable is the exchange rate between each coin and USD. Volume is the number of coins traded per day. *Rvolt* is a ranged based volatility, or the natural log of the daily high price minus the natural log of the daily low price following Alizadeh, Brandt, and Diebold (2002). *Illiq* is the absolute continuously compounded return divided by daily dollar volume following Amihud (2002). After obtaining this information, I clean the data by dropping any missing data cells and winsorizing at the 1 st and 99th percentile levels. I note that winsorizing the data forces the maximum values, such as price, to be to be lower than expected. My final sample consists of 29,016 crypto-day observations.

In table 1, we report the summary statistics of the sample. The average price is $69.42 and the standard deviation is $410.46. The minimum price is $0.00, the maximum $3,587.51 and the median is $0.52. The price variable is highly right skewed as the median is lower than the mean, meaning that most of the cryptos exchange at a low price and there are some high outliers including the maximum, like Bitcoin. For this reason, I take the natural log of this variable in my multivariable regression analysis. The average of dollar volume is $438,318,185 and the standard deviation is $1,862,961,214. The minimum volume is $32, the maximum is $14,310,000,000, and the median is $3,184,751. Again, the volume is right skewed because most coins have little trade volume and there are the bigger coins have massive trade volume amounts. Again, I take the natural log of this variable in my multivariable regression analysis to account for this type of skewness. *Rvolt* has a mean of 0.1685 and a standard deviation of 0.1390. The minimum *Rvolt* is 0.0018, the maximum is 0.9086 and the median is 0.1313. This variable is pretty close to normally distributed and no adjustments need to be made. The *Illiq* variables mean is 0.4417, while the standard deviation 2.9596. The minimum volume is 0.0000, the max is 30.2439 and the median is 0.0001. This variable is also right skewed, but since there are days with zero illiquidity (the absolute value of the daily return in the numerator is zero), we are unable to take the natural log of this variable.

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
