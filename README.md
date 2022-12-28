# Zomato Restaurant Clustering and Sentiment Analysis

Built clustering model around cuisine and cost to use cost vs benefit analysis in business. Developed Sentiment analysis model that directly help customers finding best restaurants.

# Problem Statement

Zomato is an Indian restaurant aggregator and food delivery start-up founded by Deepinder Goyal and Pankaj Chaddah in 2008. Zomato provides information, menus and user-reviews of restaurants, and also has food delivery options from partner restaurants in select cities.

India is quite famous for its diverse multi cuisine available in a large number of restaurants and hotel resorts, which is reminiscent of unity in diversity. Restaurant business in India is always evolving. More Indians are warming up to the idea of eating restaurant food whether by dining outside or getting food delivered. The growing number of restaurants in every state of India has been a motivation to inspect the data to get some insights, interesting facts and figures about the Indian food industry in each city. So, this project focuses on analysing the Zomato restaurant data for each city in India.

The Project focuses on Customers and Company, you have to analyze the sentiments of the reviews given by the customer in the data and made some useful conclusion in the form of Visualizations. Also, cluster the zomato restaurants into different segments. The data is vizualized as it becomes easy to analyse data at instant. The Analysis also solve some of the business cases that can directly help the customers finding the Best restaurant in their locality and for the company to grow up and work on the fields they are currently lagging in.

This could help in clustering the restaurants into segments. Also the data has valuable information around cuisine and costing which can be used in cost vs. benefit analysis

Data could be used for sentiment analysis. Also the metadata of reviewers can be used for identifying the critics in the industry.

# Attributes

# Zomato Restaurant names and Metadata

Name : Name of Restaurants

Links : URL Links of Restaurants

Cost : Per person estimated Cost of dining

Collection : Tagging of Restaurants w.r.t. Zomato categories

Cuisines : Cuisines served by Restaurants

Timings : Restaurant Timings

# Zomato Restaurant reviews

Restaurant : Name of the Restaurant

Reviewer : Name of the Reviewer

Review : Review Text

Rating : Rating Provided by Reviewer

MetaData : Reviewer Metadata - No. of Reviews and followers

Time: Date and Time of Review

Pictures : No. of pictures posted with review

# Text Preprocessing

Performed Text preprocessing techniques like Stemming, Lemmatization, TfidfVectorizer.

Stemming

It is a technique used to extractbthe base form of the words by removing affixes from them. It is just like cutting down the branches of a tree to its stems.

Lemmatization

Lemmatization is a method responsible for grouping different inflected forms of words into the root form, having the same meaning.

TfidfVectorizer

Term frequency-inverse document frequency is a text vectorizer that transforms the text into a usable vector. It combines 2 concepts, Term Frequency (TF) and Document Frequency (DF). The term frequency is the number of occurrences of a specific term in a document.

# Clustering

It is the task of dividing the population or data points into a number of groups such that data points in the same groups are more similar to other data points in the same group than those in other groups.

Implemented K-means Clustering, Agglomerative Clustering and obtained optimal number of cluster using Elbow method.

K-means

The K-means clustering algorithm computes centroids and repeats until the optimal centroid is found. It is presumptively known how many clusters there are. It is also known as the flat clustering algorithm. The number of clusters found from data by the method is denoted by the letter ‘K’ in K-means.

![image](https://user-images.githubusercontent.com/102653523/209869956-4330dd50-c2e3-414c-aead-5e1f3bbe5913.png)


DBSCAN Clustering

DBSCAN is a density-based clustering algorithm that works on the assumption that clusters are dense regions in space separated by regions of lower density. It groups ‘densely grouped’ data points into a single cluster. It can identify clusters in large spatial datasets by looking at the local density of the data points. The most exciting feature of DBSCAN clustering is that it is robust to outliers.

# Performed Vader and Textblob Sentiment analysis.

Vader

Sentiment analysis is a text analysis method that detects polarity (e.g. a positive or negative opinion) within the text, whether a whole document, paragraph, sentence, or clause. Sentiment analysis aims to measure the attitude, sentiments, evaluations, attitudes, and emotions of a speaker/writer based on the computational treatment of subjectivity in a text.

![image](https://user-images.githubusercontent.com/102653523/209870038-6644bc68-8699-4d58-9424-4f7cb224cad6.png)


Textblob

TextBlob is a python library for Natural Language Processing (NLP).TextBlob actively used Natural Language ToolKit (NLTK) to achieve its tasks. NLTK is a library which gives an easy access to a lot of lexical resources and allows users to work with categorization, classification and many other tasks. TextBlob is a simple library which supports complex analysis and operations on textual data.

![image](https://user-images.githubusercontent.com/102653523/209870089-c72745c0-915a-4cc5-9f99-4ec586c642ad.png)


Conclusion

* Achieved Silhouette score of 0.204 and was able to generate insights on cost vs benefit and Sentiment analysis.
* North Indian cuisine is most common cuisine found in the restaurants.
* Collage - Hyatt Hyderabad Gachibowli is most expensive restaurant.
* Amul and Mohammedia Shawarma are the most affordable restaurants.
* The Restaurants are clustered on cuisines into 15 clusters by using KMeans clustering algorithm with the Silhouette score of 0.195.
* DBSCAN algorithm is also used to cluster the restaurants into 15 clusters and also helps us to detect the outliers with the Silhouette score of 0.107.
* Anvesh Chowdary has given the most number of reviews.
* AB’s – Absolute Barbecues is the top rated restaurant.
* Almost 79 percent of the observations have Positive sentiment and 14 and 7 percent of the observations have Neutral and Negative sentiments respectively
* Good is the most common word in the Highly positive sentiment.
* Worst is the most common word in the Highly negative sentiment.
* AB’s – Absolute Barbecues, The Indi grill and B-Dubs are the restaurants with the most number of positive reviews.
* Arena Eleven and Banana leaf Multicuisine restaurant are the restaurants with the most number of negative reviews.
* Udipi's Upahar is the most affordable restaurant with the best rating.
* Feast - Sheraton Hyderabad Hotel is the most expensive restaurant with the best rating.
* Asian Meal Box is the most affordable restaurant with the worst rating.
* Club Rogue is the expensive restaurant with worst rating.
