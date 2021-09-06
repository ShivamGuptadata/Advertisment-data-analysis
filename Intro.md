# Advertisment-data-analysis

**Object**
1. Compering two models and check which are the given better accuracy
2. Which variables increased the net profit in advertising and which better method shoud be used to get more profit in advertising

# Introduction

The topic is **The success of an advertisement campaign** and now we talk about the advertisement campaign, it is the most important topic for marketing.

**The great art of writing advertisements is finding the proper method to catch the reader's eye, without which a good thing may pass unobserved---Joseph Addison**

**Advertising is to business what steam is to machinery, the grand propelling power-----Lord Macaclay**

**Elements of a Successful Advertising Campaign**

The importance of marketing in today's business environment is undoubtedly immense. No firm can sit back and watch their competitors take over the market. The right time to launch a product is an essential factor to decide the fate of a new launch. Marketing strategies govern the success of products and advertising forms the subset of a marketing plan.
1. Importance of Market Research
2. Marketing Mix Strategy
3. Promotion Strategy

According to the above information our project is based on a **Promotion Strategy**.

# 2. Data Analysis (Step by Step)

  2.1. Data Preprocessing
	2.2. Data Dictionary
	2.3. Bias Data and Solution of Bias Data
	2.4. Data Visualization 
	2.5. Missing Value
	2.6. Transfer the Categorical Data into Numerical Data 
	2.7. Model Performance Measure 
	2.8. Models
	2.9. Result
  
 # Data Preprocesing
 
The preprocessing of the text data is an essential step as it makes the raw data ready for regression, i.e., it becomes easier to extract information from the related data and 
apply machine learning algorithms to it. If we skip this step then there is a higher chance that you are working with noisy and inconsistent data.
In the data preprocessing stage, first we will combine train and test data using the following code. This saves the trouble of performing the same steps twice on test and train

**test=pd.read_csv('advertis_Test.csv')**
**train=pd.read_csv('advertise_train1.csv')**

# Data Dictionary

Variable definitions are shows in following:

**Id** -Unique id for each row

**Ratings** -Metric out of 1 which represents how much of the targeted demographic watched the advertisement

**Airlocation** -Country of origin

**Airtime** -Time when the advertisement was aired

**Average_runtime(minutes_per_week)** -Minutes per week the advertisement was aired

**Targeted_sex** -Sex that was mainly targeted for the advertisement

**Genre** -The type of advertisement

**Industry** -The industry to which the product belonged

**Economic_status** -The economic health during which the show aired

**Relationship_status** -The relationship status of the most responsive customers to the advertisement

**Expensive** -A general measure of how expensive the product or service is that the ad is discussing.

**Money_back_guarantee** -Whether or not the product offers a refund in the case of customer dissatisfaction.

**Netgain [target]** -Whether the ad will incur a gain or loss when sold


