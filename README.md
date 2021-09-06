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
	2.7. Models
	2.8. Result
  
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

# Bias Data and Solution of Bias Data

The common definition of bias data is that the available data is not presented in a proper way; it means that the data is not representative of the whole population. In my situation the data is appropriate.
The solution of this problem is using the re-sampling method in python. Re-sampling method are two type:
1. Over sampling						2. Under sampling

Now we handle a bias data by **Random Under Sampling** procedure

# Data Visualization 

I have discussed the importance of data for ML algorithms along with some Python notebook to understand the data with statistics. There is another way called visualization, to understand the data. With the help of data visualization, we can see how the data looks like and what kind of correlation is held by the attributes of data. It is the fastest way to see if the features correspond to the output. With the help of following Python recipes, we can understand ML data with statistics.

Some Imp points due to visualize data

1.The ratings of each advertisment is 0.01 to 0.03.
2. On an average run time of the advertising is an approx 40mpw (minutes per week).
3.  According to the above data **72.4%female** and **27.6%** male are seen in advertisements. It means the maximum number of females are interested to see advertisements.
4.  According to the above data, **low products** are getting more advertisement **(i.e.60.2%)** and **medium products** are getting less advertisement **(i.e. 11.5%)**.
5.  According to above data, **Primetime** is the best time for advertisement **(i.e. 68.0% advertisement is seen in primetime)**.
6.  In **Infomercial** related advertisement companies will be profitable in netgain. But **drama** genre related advertisement company will be lost in netgain.

# Missing Value

It is common in data analytics tasks to encounter missing values in datasets, where by missing we mean that some particular values does or should exist, and failed to be observed or recorded. In machine learning tasks, it is common to handle missing data by removing observations with missing values, or replacing missing data with the mean value for its feature. To show why this is problematic, we use listwise deletion and mean imputation to recover missing values from artificially created datasets, and we compare those models against ones with full information.Now we check missing value in our data and there is no mising value.

# Transfer the Categorical Data into Numerical Data 

By the LabelEncoder,Transform the categorical data into numerical data

# Models

We used two models and then we selected a model having the highest accuracy score after parameter tuning to do the prediction on test data.
1. Logistic Regression
2. Random Forest Algorithm

# Results

The perfomance of the Logistic Regression

**C+Solver**			**Accuracy Score**

**10+liblinear**		0.7274683884853377

**10+newton-cg**		0.7288135593220338

**10+saga**			0.6785041700295937

**100+liblinear**		0.7309658326607479

**100+newton-cg**		0.7312348668280871

**100+saga**			0.6785041700295937

The perfomance of the Random Forest

**Number of estimators(n_estimators)**		**Accuracy score**

**10**						0.7589453860640302

**50**						0.7635189669087974

**100**						0.7678235135862255

# Conclusion

1.  The maximum accuracy obtained for the **logistic Model is 73.12%** and **Naïve for Random Forest is 76.78%**. 
2. In advertising, Pharma industry are get profitable and if we focus on female gender then this campaign are get more profit, the best time to advertising products is Prime time and the video time of the advertisement should be less.




