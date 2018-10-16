Analyzing Happiness in Italian Tweets - Happy Factor
=======================================================

Our study is based on TWITA [1], the largest available corpus of Italian tweets.
In particular, we analyze a subset of 400M tweets obtained by filtering-out  re-tweets from all the 500M tweets collected from February 2012 to September 2015.
Following the idea proposed in [2, 3], we select positive and negative tweets based on the presence of positive or negative emoticons (we use :-) and :) for happy and :-( and :( for sad). Since a tweet can contain multiple emoticons, we selected only tweets that contain a single emoticon appearing at the end of the tweet. Using this procedure we obtain a corpus of 8,648,476 tweets.

From the corpus, we extract a subset of words and we assign them an happiness factor computed according to the log of the odds ratio between the probability that the word occurs in positive tweets and the probability that it occurs in negative tweets.
We adopt additive smoothing (Laplace smoothing) for computing both *happy* and *sad* probabilities. In our lexicon, we include and compute the happiness factor only for words that occur at least 10,000 times, for a total of 718 words.
We call this list *the happiness dictionary*.

If you use the dictionary, please cite our work as follows:

* Pierpaolo Basile, Nicole Novielli. "*'Buon appetito!'* - Analyzing Happiness in Italian Tweet". In Proceedings of the of Fifth Italian Conference on Computational Linguistics (CLiC-it 2018), Turin, Dec. 2018 (to appear).  

References
---------------
1. Valerio Basile and Malvina Nissim. 2013. Sentiment analysis on Italian tweets. In Proceedings of the 4th Workshop on Computational Approaches to Subjectivity, Sentiment and Social Media Analysis, pages 100–107.
2. Jonathon Read. 2005. Using emoticons to reduce dependency in machine learning techniques for sentiment classification. In Proceedings of the
ACL student research workshop, pages 43–48. Association for Computational Linguistics.
3. Alec Go, Lei Huang, and Richa Bhayani. 2009. Twitter sentiment analysis. Entropy, 17:252.
