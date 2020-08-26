![alt text](https://datahack-prod.s3.ap-south-1.amazonaws.com/__sized__/contest_cover/practice_prob_1-thumbnail-1200x1200.png)
**Twitter Sentiment Analysis**

Sentiment Analysisrefers to the use ofnatural language processing,text analysis,computational linguistics, andbiometricsto systematically identify, extract, quantify, and study affective states and subjective information. Sentiment analysis is widely applied tovoice of the customermaterials such as reviews and survey responses, online and social media, and healthcare materials for applications that range frommarketingtocustomer serviceto clinical medicine

**Objective**

The objective of this task is to detect hate speech in tweets. For the sake of simplicity, we say a tweet contains hate speech if it has a racist or sexist sentiment associated with it. So, the task is to classify racist or sexist tweets from other tweets.

Formally, given a training sample of tweets and labels, where label '1' denotes the tweet is racist/sexist and label '0' denotes the tweet is not racist/sexist, your objective is to predict the labels on the test dataset.

 

**Motivation**

Hate  speech  is  an  unfortunately  common  occurrence  on  the  Internet.  Often social media sites like Facebook and Twitter face the problem of identifying and censoring  problematic  posts  while weighing the right to freedom of speech. The  importance  of  detecting  and  moderating hate  speech  is  evident  from  the  strong  connection between hate speech and actual hate crimes. Early identification of users promoting  hate  speech  could  enable  outreach  programs that attempt to prevent an escalation from speech to action. Sites such as Twitter and Facebook have been seeking  to  actively  combat  hate  speech. In spite of these reasons, NLP research on hate speech has been very limited, primarily due to the lack of a general definition of hate speech, an analysis of its demographic influences, and an investigation of the most effective features.

 

**Data**
Our overall collection of tweets was split in the ratio of 65:35 into training and testing data. Out of the testing data, 30% is public and the rest is private.

 

**Data Files**
 

train.csv - For training the models, we provide a labelled dataset of 31,962 tweets. The dataset is provided in the form of a csv file with each line storing a tweet id, its label and the tweet.
There is 1 test file (public)

test_tweets.csv - The test data file contains only tweet ids and the tweet text with each tweet in a new line.

**Score**

nltk + word2vec + XGBoost   =  0.6959

spacy + tf-idf + svc = 0.6964

bert = 0.7668
