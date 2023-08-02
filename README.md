# Web-Analysis
This is a my project for web scraping. We selected the website Home Sweet Home | eHow that provides the web articles we are interested in. eHow.com is dedicated to topics related to home and living, such as home
improvement, decor, gardening, cooking, and cleaning. Articles provide step-by-step guides to help people improve their living spaces and make their homes more comfortable and functional. This website has more than 3000 articles with many
sentiments rather than full of just neutral facts. This web page meets the three main steps of our project:

• Scraping of web articles
• Developing a sentiment classifier
• Performing a cluster and topic analysis

# Step 1:
When we collect all articles, parse the HTML code of each article and extract article title, article body text, posting date and time, and author. We will extract information from all the articles and save it in a single CSV file in which a row corresponds to an article.

- The notebook consists of two main sections:

- Download the HTML Files
- Extract and Store Articles

# Step2:

We randomly selected 2000 sentences from the body texts of the downloaded articles as the data set. After manually labelling the sentences as positive, negative, and neutral, we randomly selected 80% of the sentences in the data set as training data to train 8 different kinds of classification algorithms. We then compared the algothrims' performances to select the best classifier for our data set.

- The notebook consists of 4 main sections:

- Construct the data set
- Prepare the data for modeling
- Classifier selection
- 3.1. K-Nearest Neighbours
- 3.2. Logistic Regression
- 3.3. Multinomial Naive Bayes
- 3.4. Devision Tress
- 3.5. Random Forest
- 3.6. Linear Support Vector Machines
- 3.7. Kernalized Support Vector Machines
- 3.8. Neural Network
- Test the selected model
  
📌 By comparing their performances regarding test accuracy and other indexes, we selected Random Forest as the best classification algorithm for our data set, and tested it on 10 new sentences.
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
