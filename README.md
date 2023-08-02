# Web-Analysis
This is a my project for web scraping. We selected the website Home Sweet Home | eHow that provides the web articles we are interested in. eHow.com is dedicated to topics related to home and living, such as home
improvement, decor, gardening, cooking, and cleaning. Articles provide step-by-step guides to help people improve their living spaces and make their homes more comfortable and functional. This website has more than 3000 articles with many
sentiments rather than full of just neutral facts. This web page meets the three main steps of our project:

• Scraping of web articles
• Developing a sentiment classifier
• Performing a cluster and topic analysis

# Step 1:
When we collect all articles, parse the HTML code of each article and extract article title, article body text, posting date and time, and author. We will extract information
from all the articles and save it in a single CSV file in which a row corresponds to an article.

# Step2:

First, we tokenize the body text in all articles into sentences and merge all the identified sentences. Second, we create a random sample 2000 sentences out of all the sentences.
Third, we read the 2000 sentences one by one and manually label each sentence to label each of the following three sentiments (positive, negative, and neutral) and then we
create a CSV file, in which each row has a sentence and its sentiment. Lastly, we develop a sentiment classifier that predicts the sentiment of a new sentence. We apply
all the classifications algorithms that we have learned and select the best performing classifier, test it to show how to respond diverse types of sentences.
# Step3:

First, we apply k-means clustering to all the 3000 articles and find some clusters of related articles which explain the data. Second, we apply LDA topic modeling to the
same data to find some topics with contributing keywords that have been the best explanation of data.
The notebook consists of 3 main sections:

- Parepare the data set
- 1. K-means clustering
- 2.1 Fit the model
- 2.2 Evaluate model performance
  
- 2. LDA topic modeling
- 3.1 Fit the model
- 3.2 Model evaluation and visualizaiton
  
📌 In summary, the K-Means model found 6 clusters that could be differentiated by keyword analysis; the LDA model generated 3 topics for the data set.
