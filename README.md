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
### DESCRIPTIVE ANALYSIS
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

### EXPLORATORY DATA ANALYSIS
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

![travel pics](https://github.com/debbhie/COGNORISE-INTERNSHIP-TRAVEL-AND-TOUR-ANALYSIS/assets/161854079/be610710-7b2a-454e-80b2-e0af867a34ec)

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
   


