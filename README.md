# Twitter-Sentiment-Analysis
A machine learning project to analyze and classify tweets based on sentiment using natural language processing, implemented in Python

### Libraries Used:-
1. numpy - used for working with arrays
2. pandas -  used to analyse data
3. re – used for string matching
4. sklearn -  useful and robust library for machine learning in Python
5. math -  used for mathematical tasks
6. nltk -  Python package that you can use for NLP.

### Text Preparation:-
Before classifying the sentiment of tweets or reviews, the following steps are applied on datasets.
- Converting all the words to lower case.
- Stop words removal: stop words such as I, and, the, for, should and etc., are removed from the tweets using NLTK’s(Natural Language Toolkit) stop word list.
- URL removal: all the URLs from the tweets are removed using Regex module
- Username removal: all the username (@hello) are removed using Regex module
- Segregations: in this process, the special characters such as “’ ? !;: # $ % & () * +  − / <  >  = [] n ˆ _ {} |~ are removed from the tweets.
- Tokenization: in this process, tweets are splitted into phrases or tokens, symbols and words.
- Lemmatization: the main work of Lemmatization process is to reduce the words to its base forms with the help of morphology Lemmatization. For instance, the words ‘advising’ and ‘advised’ are reduced to their root word as ‘advice’.
- Converting Abbreviations to sentences


### Models used in this study:-
1. COMPLEMENT NAÏVE BAYES - In complement Naive Bayes, instead of calculating the probability of an item belonging to a certain class, we calculate the probability of the item belonging to all the classes. This is the literal meaning of the word, complement and hence is called Complement Naive Bayes

2. LOGISTIC REGRESSION - Logistic regression estimates the probability of an event occurring, such as voted or didn’t vote, based on a given dataset of independent variables. Since the outcome is a probability, the dependent variable is bounded between 0 and 1.


### Limitations:-
- Tone can be difficult to interpret verbally, and even more difficult to figure out in the written word. Things get even more complicated when one tries to analyze a massive volume of data that can contain both subjective and objective responses. Brands can face difficulties in finding subjective sentiments and properly analyzing them for their intended tone.

- Words such as “love” and “hate” are high on positive (+1) and negative (-1) scores in polarity. These are easy to understand. But there are in-between conjugations of words such as “not so bad” that can mean “average” and hence lie in mid-polarity (-75). Sometimes phrases like these get left out, which dilutes the sentiment score.

- People use irony and sarcasm in casual conversations and memes on social media. The act of expressing negative sentiment using backhanded compliments can make it difficult for sentiment analysis tools to detect the true context of what the response is actually implying. This can often result in a higher volume of “positive” feedback that is actually negative.
