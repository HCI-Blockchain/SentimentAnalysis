
# Sentiment Analysis for Blockchain and Beyond
In this pilot study, we replicate three literatures: All of them work on researching the influence of media on the cryptocurrency, especially bitcoin. 

Glaser (2014):
Glaser, F., Zimmermann, K., Haferkorn, M., Weber, M. C., and Siering, M. (2014). Bitcoin-
asset or currency? revealing users’ hidden intentions. In ECIS 2014 Tel Aviv.

Kristoufek (2015)
x L. (2015). What are the main drivers of the bitcoin price? evidence from wavelet coherence analysis. PloS one, 10(4):e0123923.

Mai et al. (2015)
Mai, F., Bai, Q., Shan, Z., Wang, X. S., and Chiang, R. H. (2015). The impacts of social
media on bitcoin performance. In Proceedings of the 2015 International Conference on
Information Systems


# Data Dictionaries

## Dataset 1 
|                 | Glaser(2014)                                                                                    | My Replication                                           |
|-----------------|-------------------------------------------------------------------------------------------------|----------------------------------------------------------|
| Data Variables  | Wikipedia Searches, Bitcoin Prices, Positive & Negative events, Exchange Volume, Network Volume | Tweet Volume, Bitcoin Prices, Positive & Negative Events |
| Data Range      | 2011-01-01 ~ 2013-10-02 (1004 observation)                                                      | 2019-01-01 ~ 2021-10-28 (1031 observations)              |
| Data Frequency  | Daily                                                                                           | Daily                                                    |
| Method          | ARCH/GARCH with Exogenous Regressors                                                            | ARCH/GARCH with Exogenous Regressors                     |


## Dataset 2

|                 | Kristoufek (2013)                                                              | Kristoufek (2015)                               | My Replication                                                                                                                                                                        |
|-----------------|--------------------------------------------------------------------------------|-------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Data Variables  | The Logarithmic Returns of Stock Indices (NASDAQ, FTSE, CAC, DAX, HSI, NIKKEI) | Wikipedia Searches, Google Trend, Bitcoin Price | Wikipedia Searches, Google Trend, Bitcoin Price, Logarithmic Returns of Bitcoin Price                                                                                                 |
| Data Range      | 2000-2013                                                                      | 2011-09-14 ~ 2014-02-28                         | 2017-01-01 ~ 2019-11-23                                                                                                                                                               |
| Data Frequency  | Daily                                                                          | Daily                                           | Daily                                                                                                                                                                                 |
| Method          | Continuous wavelet transform                                                   | Wavelet Coherence                               | Continuous wavelet transform (https://github.com/mabelcalim/waipy); Wavelet Coherence (https://ww2.mathworks.cn/matlabcentral/fileexchange/47985-cross-wavelet-and-wavelet-coherence) |

## Dataset 3
Daily Bitcoin Price and trading volume is crawled from cryptocmd API

Reddit Comments are crawled through PushShift API (20, 000+)

Tweets are crawled through snscrape API (300, 000+)

Google trend is crawled through pytrend API

Finance sentiment dictionary (Loughran and McDonald 2014)
