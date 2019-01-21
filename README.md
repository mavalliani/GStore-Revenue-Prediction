# GStore-Revenue-Prediction
Predict how much GStore customers will spend

**Objective of the notebook:**

In this notebook, let us explore the given dataset and make some inferences along the way. Also finally we will build a baseline light gbm model to get started. 

**Objective of the competition:**

In this competition, we a’re challenged to analyze a Google Merchandise Store (also known as GStore, where Google swag is sold) customer dataset to predict revenue per customer. 

**About the dataset:**

Similar to most other kaggle competitions, we are given two datasets
* train.csv
* test.csv

Each row in the dataset is one visit to the store. We are predicting the natural log of the sum of all transactions per user. 
    
The data fields in the given files are 
* fullVisitorId- A unique identifier for each user of the Google Merchandise Store.
* channelGrouping - The channel via which the user came to the Store.
* date - The date on which the user visited the Store.
* device - The specifications for the device used to access the Store.
* geoNetwork - This section contains information about the geography of the user.
* sessionId - A unique identifier for this visit to the store.
* socialEngagementType - Engagement type, either "Socially Engaged" or "Not Socially Engaged".
* totals - This section contains aggregate values across the session.
* trafficSource - This section contains information about the Traffic Source from which the session originated.
* visitId - An identifier for this session. This is part of the value usually stored as the _utmb cookie. This is only unique to the user. For a completely unique ID, you should use a combination of fullVisitorId and visitId.
* visitNumber - The session number for this user. If this is the first session, then this is set to 1.
* visitStartTime - The timestamp (expressed as POSIX time).

Also it is important to note that some of the fields are in json format. 
