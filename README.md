
# Research Question


I am focusing on finding what and how the sentiments of population/netizens have changed after Elon Musk tweeted about Bitcoins.


# Background

I will be focusing on finding the sentiments of the population after Elon Musk changed the bio of his Twitter account to #bitcoin on Januarry 29, 2022.[1] This is the specific cryptocurrency that I will be focusing on. Bitcoins is one of the oldest cryptocurrency based on Blockchain technology, which was created to make a decentralized system for issuing new coins and recording transactions. The decentralized ideals are the main selling point as they are not owned by any government or authority and the crypto market is open 24/7.[2] 
However, Studies has shown a strong co-movement between the Bitcoin/cryptocurrency price movements and the sentiments of investors using social media. [1,3,4,5]

No one knows what moves the 1.3 trillion Dollar crypto market however they are affected by the tweets made by Elon Musk from January to June 2021 which is against the decentralized ideal of crypto market.[3]


# Data

I will be using the Twitter Developer API to gather at least 500 random English tweets about Bitcoin from Dec 2020 to July 2021 using Elon Musk's Handle(@elonmusk) and hashtags like 
“bitcoin”, “bitcoins”, “Bitcoin”,
“Bitcoins”, “BTC”, “XBT”, and “satoshi”) or any hashtags of Bitcoin’s ticker symbols (“#XBT”, “\$XBT”,“\#BTC”, and “\$BTC”).[6,7]


I will be storing the text of the tweet, the timestamp, retweets and likes.
Using this paper [7], I will be prepossessing the data to remove stopwords, URLs and hashtags as it shows that the data cleaning process helps in giving better results.


# Methods

I will be performing sentiment analysis using VADER model on the tweets that I will be collection to find emotions that the population generates about Bitcoins.
VADER(Valence Aware Dictionary and sentiment Reasoner) lexical sentiment analysis is faster than any Machine Learning algorithms and would process the tweets which are character limited. It one of the best tools for handling social media text data as it can handle unlabelled data as well as understands slang's, punctuation's, emoticon's, etc. It also understands the importance of capitalized words in textual data
It is a model which is freely available in NLTK library and handles polarity(positive/negative sentiments) of data as well as magnitude of emotions.[8]
It categorizes the data into positive, negative and neutral scores which are then normalized in a compound score, in the range of -1 to 1.
I will perform a manual analysis to check if the scores assigned by VADER were correctly identifying the polarity of statements with double negatives and other figure of speech.


# References


- Ante, L., (2021, February 3) How Elon Musk's Twitter Activity Moves Cryptocurrency Markets. Blockchain Research Labs BRL Working Paper Series No. 16 Social Science Research Network. Available at SSRN: https://ssrn.com/abstract=3778844 or http://dx.doi.org/10.2139/ssrn.3778844
- Molla, R., (2021, June 14) When Elon Musk tweets, crypto prices move
How Elon Musk affects bitcoin prices, in one chart. Vox. 
[URL](https://www.vox.com/recode/2021/5/18/22441831/elon-musk-bitcoin-dogecoin-crypto-prices-tesla)
- Parker, E., (2021, May 26) Opinion: Cryptocurrency has an Elon Musk problem. The Washington Post. 
[URL](https://www.washingtonpost.com/opinions/2021/05/26/elon-musk-tweets-crypto-markets/)
- Abdali, S., Hoskins, B., (2021 Spring) Twitter Sentiment Alanysis for bitcoin Price prediction. CS229: Machine Learning Standford University Reports. [URL](http://cs229.stanford.edu/proj2021spr/report2/81988764.pdf)
- Hassan, M & Hudaefi, F & Caraka, R. (2021). Mining netizen's opinion on cryptocurrency: sentiment analysis of Twitter data. Studies in Economics and Finance. 38. 10.1108/SEF-06-2021-0237. 
- Pano, T., & Kashef, R. (2020). A Complete VADER-Based Sentiment Analysis of Bitcoin (BTC) Tweets during the Era of COVID-19. Big Data and Cognitive Computing, 4(4), 33. https://doi.org/10.3390/bdcc4040033
- Zaman, S., Yaqub, U. and Saleem, T. (2022), "Analysis of Bitcoin’s price spike in context of Elon Musk’s Twitter activity", Global Knowledge, Memory and Communication, Vol. ahead-of-print No. ahead-of-print. https://doi-org.proxyiub.uits.iu.edu/10.1108/GKMC-09-2021-0154
- Beri, B., (2020, May 27) Sentimental Analysis Using VADER. TowradsDataScience. [URL](https://towardsdatascience.com/sentimental-analysis-using-vader-a3415fef7664)


