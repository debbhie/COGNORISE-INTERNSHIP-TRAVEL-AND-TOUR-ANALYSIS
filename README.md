# TRAVEL AND TOUR CUSTOMER ANALYSIS

## TABLE OF CONTENT

## TRAVEL AND TOUR CUSTOMER ANALYSIS OVERVIEW
This report presents an in-depth analysis of the "Tour and Travel Customer" dataset, which consists of 954 entries. The dataset includes various attributes related to customers such as age, frequent flyer status, income level, service usage, and whether they have synced their account to social media or booked a hotel through the company. The primary goal of this analysis is to provide insights into customer behavior, identify key factors influencing customer churn, and recommend strategies for improving customer retention and engagement.

##  LANDING PAGE
* Age: This column consists of the ages of the customers.
* Frequent flyers: Column consists of whether customers takes frequent flights with the company or not.
* Annual Income Class: consits of class of annual income of customers. high income, middle income, low income.
* Services opted: contains number of times the company services were used by the customers.
* Account synced to social media: consis of whether account of customers are sychronized to their social media.
* Booked hotel or not: Whether the customer book lodging/hotel using the company services
* Target: 1-customers churn, 0-customer did not churn.

## DATA SOURCE
This dataset is from cognorise internship.
-[download here](https://www.kaggle.com/datasets/tejashvi14/tour-travels-customer-churn-prediction)

## TOOLS
- Microsoft excel- data analysis
- Microsft excel- dashboard/report

## TYPES OF ANALYSIS USED FOR THIS PROJECT
* Descriptive Analysis: Used to analyze and describe the main characteristics of the data set.
* Exploratory Data Analysis: Used for correlation matrix, churn by demographic
* Predictive Analysis: Used for churn prediction.

## KEY PERFORMANCE INDICATORS
* Total number of customers
* Average age of customers
* Percentage of frequent flyers vs non frequent flyers
* Proportion of income distribution of customers in different categories
* Average number of services opted for by customers
* Number of times customers opted for their services
* Percentage of customers with account synced to their social media
* Percentage of customers booking hotel through their services
* Percentage of customers who churned vs customers who did not churn
* Predictive model accuracy (accuracy, precision and recall)

## DATA CLEANING
These processes were carried out using power query
* Duplicates were not found
* Spelling errors were corrected
  
## DATA PROCESSING
* Predicted_churn column was created
* Churn_status column was created as well
  
## DATA ANALYSIS
### DESCRIPTIVE ANALYSIS
This is the first step in understanding the basic characteristics of the dataset. It provides a summary of the central tendencies, distributions, and proportions of different variables.

* Total Customers: 954
  
* Average Age: 32 years

* Average Number of Services Opted: 2 services
  
* Distribution of Services Opted:
 - Opted 1 service: 404 customers
 - Opted 2 services: 176 customers
 - Opted 3 services: 124 customers
 - Opted 4 services: 117 customers
 - Opted 5 services: 69 customers
 - Opted 6 services: 64 customers
   
* Frequent Flyer Status
 - Frequent Flyers: 30%
 - Non-Frequent Flyers: 64%
 - No Record: 6%
* Income Distribution
 - High Income: 17%
 - Middle Income: 40%
 - Low Income: 40%

* Social Media Synchronization
 - Accounts Synced to Social Media: 38%
 - Accounts Not Synced: 62%
   
* Hotel Booking Through Company Services
 - Booked Hotel: 40%
 - Not Booked: 60%

* Customer Churn
 - Churned: 23%
 - Did Not Churn: 77%

### EXPLORATORY DATA ANALYSIS
This helps to uncover patterns, correlations, and anomalies in the data.

* Correlation Matrix
The correlation matrix shows the relationship between customer churn and other variables. Here are the key findings:

* Age Correlation with Churn: -13%
Older customers tend to churn slightly less than younger customers.

* Service Usage Correlation with Churn: 4%
A slight positive correlation indicates that more service usage is associated with a marginal increase in churn likelihood.

* Frequent Flyer Correlation with Churn: -6%
Frequent flyers are slightly less likely to churn compared to non-frequent flyers.

* Income Level Correlation with Churn: 14%
Higher income is positively correlated with a higher likelihood of churn.

* Social Media Sync Correlation with Churn: 7%
Customers who have their accounts synced to social media have a slightly higher churn rate.

* Hotel Booking Correlation with Churn: -21%
Customers who booked hotels through the company's services are significantly less likely to churn.

### predictive analysis
was conducted to determine the accuracy of a churn prediction model using a confusion matrix.

* Model Performance Metrics
Accuracy: 27%
The model correctly predicted customer churn only 27% of the time, indicating a need for model improvement.

* Precision: 24%
Out of all customers predicted to churn, only 24% actually did, showing a high rate of false positives.

* Recall: 99%
The model identified 99% of actual churned customers, but this high recall is at the expense of precision.

## DATA VISUALIZATION


## INSIGHTS
 * High Churn Rate Among Higher Income Customers: Higher income customers tend to churn more, possibly due to their greater number of alternatives. This group may seek higher value or more personalized services.

* Significant Impact of Hotel Booking on Churn: Customers who book hotels through the company are less likely to churn, suggesting that these bookings enhance customer loyalty.

* Frequent Flyers Are Loyal: Frequent flyers are less likely to churn, indicating they value the services provided by the company.

* Service Usage and Churn: There is a slight increase in churn with more service usage, which could imply dissatisfaction with services or unmet expectations.

* Social Media Sync and Churn: Accounts synced to social media show a slightly higher churn rate, potentially indicating that these customers are more exposed to competitors’ promotions or reviews.

* Young Customers and Churn: Younger customers have a higher churn rate, possibly due to less brand loyalty and more flexibility in switching services.

## RECOMMENDATIONS
* Enhance Value for High Income Customers: Develop premium services or loyalty programs tailored to high-income customers to reduce their churn rate.

* Promote Hotel Booking Services: Strengthen and promote hotel booking services to increase customer retention. Consider offering exclusive deals or discounts for repeat customers.

* Focus on Frequent Flyers: Continue to nurture and reward frequent flyers with benefits and personalized experiences to maintain their loyalty.

* Improve Service Quality and Expectations Management: Investigate why customers using more services are slightly more likely to churn. Enhance service quality and set clear expectations to reduce churn.

* Leverage Social Media Engagement: Since customers with social media-synced accounts are more prone to churn, improve social media engagement by offering exclusive promotions and engaging content.

* Engage Younger Customers: Develop strategies to engage younger customers, such as offering trendy, budget-friendly packages or engaging them through social media campaigns.

* Model Improvement: The current churn prediction model is not very accurate. Enhance the model by including more relevant features, using different algorithms, and improving data quality.

By implementing these recommendations, the company can better understand its customer base, enhance customer satisfaction, and reduce churn rates, thereby driving growth and sustainability.
   


