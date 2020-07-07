
# Project 3: Pushshift's API WebScrapping for Predicting Comments and Modeling: Excutive summamry

  Dereje Workneh  April 24, 2020

  Data Science Immersive Student @ General Assembly


### Introduction
Reddit claims to be the front page of the internet, and that's because they are. With an average of 11 million daily active users. Reddit is one of the top social news distribution and websites rating by users every day from politics to specific daily life. The Reddit website was 5th most visted and ranked here in the united states and accessed globally with high 13's rank. Reddit is subdivided into subreddits, which are themed discussion boards created and populated by Reddit users with links, text, videos and images. These subreddits span an endless array of interests including world news, sports, economics, movies, music, fitness, and more.The site was significantly dependent on users comments and the comments ups(votes).

## Objective
The objective of this project by using Reddit or Pushshift.io API, collect posts from two subreddits of my choosing Physics and chemistry. Using the natural language processing  to train a classifier model on which subreddit agiven post came from and finally using sentimnet anaysis which one more comments physics vs chemistry.




## Procedure:
1. Data collection
2. Data cleaning and Explatory data analysis (EDA)
3. Preprocessing and modeling(tuning)
4. Validation of models
5. Conclusion and recommendation


### Data collection:
There are three main endpoints for the API to get information on comments, submissions and subreddits. I used Pushshift was used for the final data collection for this project. Data collected from pushshift was about 15, 000 commnets for both physics and chemistry. Most of data were texts which were a comparable between the two subreddits.

### Data Cleaning and EDA
During data cleaning of comments, I removed hyperlinks, html, punctuation, the same words with two or more letters, duplicate messages, whitespace, non standard characters. After cleaning there were 13, 000 recorded. Stop words were removed and some of the words in the commnents were lemmatized. The EDA result showed tha more than 20 most frequent words were unique classes in both physics and chemistry.


### Preprocessing, Modeling and Evaluation
After performing a train-test-split, I then vectorized the top 20 most common words into a sparse dataframe, which I then concatenated onto my X_train and X_test matrices with the hope that more information would improve my model performance. After standardizing my dataset with Standard Scaler, I was ready to run my models. Having fit and scored my models,  In total, Logistic regression, Random forest, and Multinomial naive Bayes models were tested with Gridsearch. While I remain skeptical of the perfect test scores for the Multinomial naive Bayes models, the R2 scores of the other two models seem to make sense. Sentiment analysis using TextBlob showed that comments in physics had a better mean positive sentiment. 

### Conclusions and Recommendation
My findings suggest that Multinomial naive Bayes, Train / test scores: 0.8202 / 0.8210 best fit. Better improvemnet by adding feattur engineering and increaing data collection time. Improve the data cleaning and preprocessing methods and further trying more models like Ada boosting, SVM.
Sentiment analysis showed that more comments in physics than chemistry.










