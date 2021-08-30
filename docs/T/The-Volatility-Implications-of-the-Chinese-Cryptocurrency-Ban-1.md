---
layout: default
title: 1. Introduction
parent: § The Volatility Implications of the Chinese Cryptocurrency Ban  
grand_parent: T 
nav_order: 10 
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

## 1. Introduction
Cryptocurrencies (hereafter cryptos) have been in the news a lot lately as policy makers continue to debate their viability as a currency or if they are simply speculative investment vehicles. Although cryptos have been mostly used as investment vehicles (Hileman 2017), it is important to identify the value they might have over other more traditional currencies. Cryptos have a few advantages. First, the new technology that Bitcoin introduced in the blockchain. The blockchain is a series of ledgers that creates a system to keep track of payments using a “proof of work” method to broadcast the correct ledger. This creates the advantage of the ledger being decentralized, which means the holder of the crypto can mitigate the risk of destabilization in a country like you would with a regular currency. Second, cryptos have the ability to have an anonymous ledger, so that the holder can remain anonymous, which can be a real power in today’s limited privacy environment. Lastly, there is a surge of advancements in the crypto field happening today. For example, Ethereum has developed a programming language that you can build apps on their platform and use Ether as the primary currency on the applications. This is just one example of progress that is taking the blockchain technology and providing further innovations. Perhaps this is why there are so many people interested in cryptos and why they get so much attention in the news.

However, this attention ends up being a double edge sword, with high profile figures, like Elon Musk, being able to affect the price of different cryptos just by sending out a tweet or a news release. A recent study built a supervised model to test cryptocurrency pricing using news and social media sentiment, which was able to correctly predict the biggest price fluctuations over a 67-day time period (Lamon, Nielsen, Redondo 2017). This correlation between news, social media and price – as well as the cryptos’ speculative nature – creates a situation that makes cryptos a risky investment with extreme fluctuations that can create price instability. Therefore, big news events involving cryptos can be of intrigue for any investor, or holder, of the cryptocurrency.

The increase in news, size, and intrigue around cryptos has also caught the attention of world governments. Although China has been the biggest country in mining and trading cryptos (Hileman 2017), the country has also been the most stringent in terms of regulation. For instance, China recently banned public coin offerings (Zhang 2020). In addition, on May 18, 2021 China took an even further step in announcing the ban of cryptocurrency transactions altogether. While many can speculate on the reasons for the Chinese government to ban cryptocurrencies, the purpose of this paper is to look into the effects this ban had on the volatility of the overall crypto market. To measure volatility, I follow Alizadeh, Brandt, and Diebold (2002) and estimate a rangebased measure of volatility, which has been shown to properly capture important properties of stochastic volatility. In particular, I calculate range volatility by taking the difference between the natural log of the daily high price minus the natural log of the daily low price (Alizadeh, Brandt, and Diebold 2002). I then examine this measure of volatility before and after the Chinese ban in an attempt to extrapolate whether this ban had any effect on the market as a whole.

To carry out this event study, I examine the prices (in USD) of 372 different cryptocurrencies, the corresponding volume in the number of coins traded, and the measure of volatility, discussed earlier. I also control for illiquidity, which is calculated using absolute continuously compounded return divided by daily dollar volume (Amihud 2002). I examine volatility around three different event windows: five days, ten days, and forty days before and after the ban of cryptocurrency transactions in China. This way I can test for the short-, medium-, and long-term effects of the news of the ban. I also estimate multivariate regressions that control for a number of important factors that might explain changes in volatility. I also provide a graphical analysis of volatility during the event days so I can observe an overall trend in order to can infer any information about the long-term effects of the event.

Results show that for all three event windows, volatility statistically increases. There is clearly a short-term economic effect from the event as the average five-day post-event volatility is 0.1685 more than the average five-day pre-event volatility. However, the long-term economic effect is questionable, as the 40-day post-event volatility is .0143 more than the 40-day pre-event volatility. While the post-minus-pre-period difference is still statistically significant in the longer window at the .01 significance level, there really does not appear to be much of an economic increase. When focusing on the multivariate analysis, I observe similar findings as the short-term economic effect of the event is statistically and economically significant, but the longer-term effect on overall volatility is too small to draw meaningful conclusions. The results from my analysis suggests that a country-wide ban on cryptocurrency transactions, like the one in China, has a dramatic, short-term effect on volatility. This information has practical importance to those using cryptos as an investment vehicle, or store of value, and to those using cryptos as a currency in a more traditional sense.

The rest of the paper follows. Section 2 presents a discussion of the data used throughout the analysis. Section 3 reports the empirical tests and results. Section 4 offers some concluding remarks.

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
