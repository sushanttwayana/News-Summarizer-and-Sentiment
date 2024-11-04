## Approach 

The two major parts of this project are news summarization and sentiment analysis on the basis of the topics on Reddit. This summarizer program makes use of an URL of any article to extract key information, while on the other hand, the sentiment analysis is carried out with comments that get extracted from posts on Reddit.

# News Summarizer
I used the Python library newspaper3k, which can download and parse news articles from a given URL. The main extracted pieces include the article's title, authors, publication date, and summary of the article. I carried out the Sentiment Analysis using TextBlob; it gives a score of polarity in general, hence deriving whether the sentiment is positive, neutral, or negative. Further, the sumy library with the LSA algorithm was used to give several variants of summary generation because it offered an alternative summarization method based on latent semantic analysis. A Tkinter GUI was designed where users could input the URL and see the summary directly in the application window.

# Analyze Sentiments on Topics in Reddit
The script fetches popular posts and their comments from the Reddit API; to do this, it used the requests library for authentication and the praw library to fetch the data. It uses the authentication into Reddit for access to every post, comment, and other metadata like upvotes and downvotes in both /r/news and /r/Nepal subreddits. Finally, the data will be stored into a Dataframe for organized analysis. Sentiment analysis was done on comments for posts in order to understand the reaction of users. The polarity according to TextBlob classified each comment into either a positive, negative, or neutral sentiment.

# Fetech 5 topics from the newsapi.org
Using the free url of newsapi.org I have simply tried to pull the five news.

# Evaluation Metrics
For the evaluation of these, I considered the following metrics:

Summary Quality: The summarization quality is measured by comparing the inherent and manually extracted summaries with LSA-based summaries.
Sentiment Accuracy: The polarity scores from TextBlob were used to validate the accuracy of sentiment classification.
API Efficiency: Performance will be shown with regards to response time and data completeness for API calls with Reddit.
Web scraping, summarization using NLP techniques, sentiment analyses using libraries such as newspaper3k, TextBlob, sumy, pandas, and praw are used for deep news analysis, smoothly switching to user-friendly interaction.

# Conclusion
Unfortunately, I couldnot make a full fledge project structure as per demanded but I have completed upto task 3 seperately and also have tried to implement frontend with html, css and flask . But I could not properly exececute them properly. All the task I have done for this project have been included with this github.

Thankyou for this opprotunity.