# TRAVEL AND TOUR CUSTOMER ANALYSIS

## TABLE OF CONTENT
- [TRAVEL AND TOUR CUSTOMER ANALYSIS OVERVIEW](#travel-and-tour-customer-analysis-overview)
- [LANDING PAGE](#landing-page)
- [DATA SOURCE](#data-source)
- [TOOLS](#tools)
- [TYPES OF ANALYSIS USED FOR THIS PROJECT](#types-of-analysis-used-for-this-project)
- [KEY PERFORMANCE INDICATORS](#key-performance-indicators)
- [DATA CLEANING](#data-cleaning)
- [DATA ANALYSIS](#data-analysis)
- [DATA VISUALIZATION](#data-visualization)
- [INSIGHTS](#insights)
- [RECOMMENDATIONS](#recommendations)


## TRAVEL AND TOUR CUSTOMER ANALYSIS OVERVIEW
The analysis of tour and travel customer dataset aimed to understand customer behavior, predict customer churn and identify key factors contributing to churn. Various analysis were used in carrying out this project such as descriptive, exploratory data and predictive data analysis techniques. Various aspect of this dataset were examined which consist of customer travel data and their interactions with the company's services. This primary focus was on understanding the characteristics of customers, their service usage patterns and the factord that influence customers to churn.

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
- Python - Jupyter notebook
- visualization - Jupyer notebook

## TYPES OF ANALYSIS USED FOR THIS PROJECT
* Descriptive Analysis: Used to analyze and describe the main characteristics of the data set.
* Exploratory Data Analysis: Used for correlation matrix, churn by demographic
* Predictive Analysis: Used for churn prediction.

## KEY PERFORMANCE INDICATORS
* Total number of customers
* Average age of customers
* Percentage of frequent flyers vs non frequent flyers
* Proportion of income distribution of customers in different categories
* Percentage of customers with account synced to their social media
* Percentage of customers booking hotel through their services
* Percentage of customers who churned vs customers who did not churn


## DATA CLEANING
These processes were carried out in jupyter notebook
* Duplicates were not found
* Spelling errors were corrected

## DATA ANALYSIS
## DESCRIPTIVE ANALYSIS
This is the first step in understanding the basic characteristics of the dataset. It provides a summary of the central tendencies, distributions, and proportions of different variables.

* Total number of customer: 954
  
* Average Age: 32 years, 11 months

* Average Number of Services Opted: 2.44 services
  
* Minimum age of customer: 27 years

* Maximum age of customer is: 38years
 
* Frequent Flyer Status
 - Frequent Flyers: 30%
 - Non-Frequent Flyers: 64%
 - No Record: 6%

* Income Distribution
 - High Income: 17%
 - Middle Income: 43%
 - Low Income: 40%

* Social Media Synchronization
 - Accounts Synced to Social Media: 38%
 - Accounts Not Synced: 62%
   
* Hotel Booking Through Company Services
 - Booked Hotel: 40%
 - Not Booked: 60%

* Customer Churn
 - Churned: 23.4%
 - Did Not Churn: 76.5%

## EXPLORATORY DATA ANALYSIS
In this aspect of exploratory data analysis, correlation matrix and churn rate segmented by age, income and frquent flyer were used to derived results from the analysis. This helps to uncover patterns, correlations, and anomalies in the data.

### CORRELATION MATRIX
The correlation matrix shows the relationship between customer churn and other variables. Here are the key findings:

* AGE 
 - Services opted: There is a slight negative correlation (-0.12), indicating that older customers tend to opt for fewer services.
 - Target: Age has slight negative correlation(-0.13) with churn, suggesting that younger customers may have a higher likelihood of churning.
 - Annual Income: There is virtually no correlation(-0.016) indicating age and income level are almost independent.

* SERVICES OPTED
  - Target: A very weak positive correlation(0.039), suggesting a slight increase in services opted could be associated with higher churn.
  - Annual Income: A weak positive correlation(0.09) indicating that customers with higher income level tend to opt for more services.
  - Frequent Flyer: slght negative correlation(-0.15) suggesting that customers who sync their account to social media tend to opt for fewer services.
  - Hotel Bokking: A moderate positive correlation (0.16) indicating customers who book hotels tend to opt for more services.
 
* ANNUAL INCOME
  - Frequent Flyer: A weak positve correlation(0.2) indication higher income customer are more likely to be frequent flyers.
  - Account Synced to socialmedia: A weak positive correlation(0.23) suggesting higher income customer are more likely to sync their account.
  - Hotel Booking: Virtually no correlation(-0.024).

* FREQUENT FLYER
  - Account synced: virtually no correlation(-0.04).
  - Hotel Booking: Aslight negative correlation(-0.13) indicating frequent flyers are less likely to book hortel through services.

* ACCOUNT SYNCED
  - Hotel booking: A slight negative correlation(-0.1), suggesting that customers who sync their account to social media are slightly less to book hotel through the company's services.

### CHURN RATE ANALYSIS
* AGE-BASED CHURN RATE: The churn rate analysis by age reveals the following patterns;
  - Age 27 and 28
    churn rate: Approximately 56%
    counts: 62 customers (age 27), 71 customer(age 28). Customers between age 27 and 28 exibit highest churn rate. This could indicate that younger customer may be more likely to switch providers, possibly due to lack of loyalty or dissatisfaction with the services offerd.
  - Age 29,30,31
    churn rate: 18.57% (age 29), 14.41% (age 30), 14.56% (age 31).
    counts: 70 customers (age 29), 236 customers (age 30), 103 customers (age 31). These age groups have moderate churn rates, suggesting that customers in their 20s to 30s may be more stable but there is still some churn. Age 30 has the highest count, so it may be key demographic to focus on for retention efforts.
  - Age 33, 34, 35
    churn rate: 27.59% (age 33), 18.69% (age 34), 25% (age 35)
    count: The churn rate for this ages are relatively high with 33 showing the highest rate. It suggests that customers in their early to mid 30s are also prone to churn, potentially due to changing life circumstances or shifting priorities.
  - Age 36, 37, 38
    churn rate: 23.88% (age 36), 21.43% (age 37), 9.68% (age 38)
    count: 67 customers(age 36), 126 customers(age 37), 31 customers (age 38). Older age groups show a decline churn rate, with age 38 having the lowest churn rate. This could suggest that older customers are more loyal or have established preferences that make them less likely to switch providers.

* ANNUAL INCOME -BASED CHURN RATE
  - High Income
    churn rate: 57.86%
    count: 159 customers. High income customers have the highest churn rate. This could br indicative of high expectations and a greater tendency to seek better alternative or more exclusive services. High income customers may also have more options and thus more opportunities to switch.
  - Low Income
    churn rate: 26.94%
    count: 386 customers. Low income customers have a moderate churn rate while they churn less than the high income customers, the churn rate is significant. This group might be more orice, sensitive and could benefit from targeted strategies.
  - Middle Income
    churn rate: 6.85%
    count: 409 customers. Middle income customers exibit the lowest churn rate. This suggest that customers in this income bracket are generally more stable and satisfied with the services. They might less likely to switch due to fewer financial resources or greater satisfaction with the current offerings.

* FREQUENT FLYER STATUS- BASED ON CHURN RATE
  - Non-frequent flyer
    churn rate: 11.35%
    count: 608 customers. Customers who do not frequently fly have the lowest churn rate. This suggest that less frequent travelers might have loyalty or satisfaction with the services possibly due to fewer competing options or lower expectations.
  - Frequent flyer
    churn rate: 51.40%
    count: 286 customers. Frequent flyers exibit the hughest churn rate. This indicate that customers who frquently use the company's services might be more likely to churn possibly due to high expectation or better offers from competitors.
  - No Record
    churn rate: 13.3%
    count: 60 customers. Customers with no record of frequent flying have a moderate churn rate. This group is likely a mixed bag with varied reasons for their status and churn behavior.
    
## PREDICTIVE ANALYSIS
* MODEL ACCURACY (89.20%): This represent the proportion of corrcetly predicted churn and non-churn instance out of thr total predictions made by the model. In this case, the model correctly predicted whether a customer churner or not 89.20% of the time. This metric indicates that the model performs reasonably well overall.

* CONFUSION MATRIX: This provides a detailed view of model's performance in predicting customer churn.
  - True Negative (TN): 206
  - False Positive (TP): 13
  - False Negative (FN): 18
  - True Positive (TP): 50

  - True Negative: The number of non-churning customers correctly predicted as not churning, there are 206 customers.
  - False Positive: The number of customers who were predicted to churn but did not churn. 13 non churning customers were incorretly label as churners.
  - False Negative: The number of churning customers incorrectly predicted as non-churners, 18 customers but they actually churned.
  - True Positive: The number of churning customers correctly predicted as churners, 50 customers and they actually churned.

* PERFORMANCE METRICS
  - Precision (0.7937 or 79.37%): Precision is the ratio of correctly predicted positive observation (true positive) to the total predicted positive (true positive + false positive). It measures how many predicted churner did actually churn.
    A precision of 0.7937 means 79.39% of the instance predicted churners did churn. Thia indicates that the modek is good at identifying true churners.

  - Recall (0.7353 or 73.53%): Recall is the ratio of correctly predicted positive observation (true positive) to the total actual positives (true positive + false negative). It measures how many of the actual churner were correctly identified by the model.
    A recall of 73.53% of actual churner means that the model successfully captures most of the churn cases.

  - F1 score (0.7634 or 76.34%): F1 score is the harmonic mean of precision and recall, providing a single metric that balances both. It is particularly useful when dealing with imbalance dataset.
    F1 score of 76.34% balances precision and recall providing a single metric tht captured both false positive and false negative. A score od 0.7634 suggests a good balance.

  The model correctly identified 206 customers who didnot churn and 50 customers who churn. There were 13 cases the model was incorrect.

## INSIGHTS FOR MODEL ACCURACY
* High overall accuracy: The model accuracy of 89.20% indicates the strong overall performance. It reliably distinguishes between customers who will churn and those who will not.
* Precision and recall balance: The precision of 79.37% and recall of 73.53% shows a reasonable balance. This means that while the model is good at predicting actual churners, it can still be iproved to reduce number of missed churn cases.
* Focus on reducing false negative: With 18 false negatives, the model misses a notable amount of actual churner.
* False positive impact: Although the rate is low, it is important to minimize these as they can lead to unnecessary retention effirts for customers who are not at risk of churning.

## RECOMMENDATION FOR MODEL ACCURACY
* Refine the model: Continously refine the model by incorporating more features or trying different algoriths to improve recall without significantly compromising precision.
* Target interventions: Use the model's predictions to implement targeted retention strategies for at-risk customers, especially those identified as likely churn.
* Monitor model performance: Regularly monitor the  model's performance and recalibrate as needed to adapt to changing customer behavior patterns.
* Customer feedback: Collect and analyze feedback from customers, particularlt those whochurn, to identify potential areas of improvement in service offerings and customer satisfaction.
  
## DATA VISUALIZATION

![travel pics](https://github.com/debbhie/COGNORISE-INTERNSHIP-TRAVEL-AND-TOUR-ANALYSIS/assets/161854079/be610710-7b2a-454e-80b2-e0af867a34ec)


## RECOMMENDATIONS


By implementing these recommendations, the company can better understand its customer base, enhance customer satisfaction, and reduce churn rates, thereby driving growth and sustainability.
   


