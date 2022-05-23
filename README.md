# **Zomato Restaurant clustering and sentiment analysis**

# **Problem Description**

Zomato is an Indian restaurant aggregator and food delivery start-up founded by Deepinder Goyal and Pankaj Chaddah in 2008. Zomato provides information, menus and user-reviews of restaurants, and also has food delivery options from partner restaurants in select cities.

India is quite famous for its diverse multi cuisine available in a large number of restaurants and hotel resorts, which is reminiscent of unity in diversity. Restaurant business in India is always evolving. More Indians are warming up to the idea of eating restaurant food whether by dining outside or getting food delivered. The growing number of restaurants in every state of India has been a motivation to inspect the data to get some insights, interesting facts and figures about the Indian food industry in each city. So, this project focuses on analysing the Zomato restaurant data for each city in India.

The Project focuses on Customers and Company, you have to analyze the sentiments of the reviews given by the customer in the data and made some useful conclusion in the form of Visualizations. Also, cluster the zomato restaurants into different segments. The data is vizualized as it becomes easy to analyse data at instant. The Analysis also solve some of the business cases that can directly help the customers finding the Best restaurant in their locality and for the company to grow up and work on the fields they are currently lagging in.

This could help in clustering the restaurants into segments. Also the data has valuable information around cuisine and costing which can be used in cost vs. benefit analysis

Data could be used for sentiment analysis. Also the metadata of reviewers can be used for identifying the critics in the industry.

# **Data Summary:**

***For Clustering***

**Data Set Name :-** Zomato Restaurant names and Metadata.csv

**Statistics : –**
**Rows -** 105
**Features -** 6

**Data Fields:-**

Name : Name of Restaurants

Links : URL Links of Restaurants

Cost : Per person estimated Cost of dining

Collection : Tagging of Restaurants w.r.t. Zomato categories

Cuisines : Cuisines served by Restaurants

Timings : Restaurant Timings

***For Sentiment Analysis***

**Data Set Name :-** Zomato Restaurant reviews.csv

**Statistics:–**
**Rows -** 10000
**Features -** 7

**Data Fields:-**

Restaurant : Name of the Restaurant

Reviewer : Name of the Reviewer

Review : Review Text

Rating : Rating Provided by Reviewer

MetaData : Reviewer Metadata - No. of Reviews and followers

Time: Date and Time of Review

Pictures : No. of pictures posted with review

# **Problem Statement**

* Our task is analyze the sentiments of the reviews given by the customer in the data and made some useful conclusion in the form of Visualizations. 
* Also, cluster the zomato restaurants into different segments. The Analysis also solve some of the business cases that can directly help the customers finding the Best restaurant in their locality

![image](https://user-images.githubusercontent.com/101592102/169803414-14e41f4c-16f8-4eb7-923a-517a8e80e342.png)

# **Approach Overview**

![image](https://user-images.githubusercontent.com/101592102/169800590-f9d3d6e6-4b98-46bf-a54e-15c163b81fca.png)


# **Clustering**

Clustering is the task of dividing the population or data points into a number of groups such that data points in the same groups are more similar to other data points in the same group than those in other groups. In simple words, the aim is to segregate groups with similar traits and assign them into clusters.

![image](https://user-images.githubusercontent.com/101592102/169801960-723daa59-cb30-4833-983d-c16c8f557a5e.png)

# **Sentiment Analysis**

Sentiment Analysis is the most common text classification tool that analyses an incoming message and tells whether the underlying sentiment is positive, negative our neutral. Sentiment analysis is contextual mining of text which identifies and extracts subjective information in source material, and helping a business to understand the social sentiment of their brand, product or service while monitoring online conversations.

![image](https://user-images.githubusercontent.com/101592102/169802121-1986b996-c972-42dd-b87d-b1ef1b04b09b.png)

**Stemming**

Stemming is a process to reduce the word to its root stem for example run, running, runs, runed derived from the same word as run. basically stemming do is remove the prefix or suffix from word like ing, s, es, etc. NLTK library is used to stem the words. The stemming technique is not used for production purposes because it is not so efficient technique and most of the time it stems the unwanted words.

**Lemmatization**

Lemmatization is similar to stemming, used to stem the words into root word but differs in working. Actually, Lemmatization is a systematic way to reduce the words into their lemma by matching them with a language dictionary.

**Frequent Keywords Used for good reviews**
![image](https://user-images.githubusercontent.com/101592102/169802471-4feb59e2-4a20-48e0-aeee-ca903ba30a1a.png)

**Frequent Keywords Used for average reviews**
![image](https://user-images.githubusercontent.com/101592102/169802567-37dbd194-7fa6-4e3b-aea3-eb05c2f4c74f.png)

**Frequent Keywords Used for Bad reviews**
![image](https://user-images.githubusercontent.com/101592102/169802644-5b376218-b436-4cc3-9592-502848b24b1a.png)

# **Conclusion**

**Clustering Analysis**

* silhouette score at n_clusters = 4, we get highest silhouette score is 0.47229. 
* From elbow method we get 4 number of cluster is best among all. 
* Applied agglomerative hierarchical clustering from this we find 4 number of cluster good fit our model. 
* By applying different clustering algorithm to our dataset. we get the optimal number of cluster is equal to 4. 

**Sentiment Analysis**

* Categorize rating in 3 types i.e. good, bad and average. 4500+ good, 1700+ bad and 900+ average ratings given by customer.
* By using logistic regression and random forest regression model on reviews dataset, we get 89% accuracy at logistic regression & 99% accuracy at random forest    regression.


