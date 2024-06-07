# Overview

In the highly competitive telecommunications market, Syriatel faces the critical challenge of retaining its customer base while ensuring high levels of satisfaction. The company struggles with identifying at-risk customers who might churn and addressing their issues proactively. This problem is compounded by the need to offer personalized services and maintain optimal network performance, all while adapting to ever-evolving customer needs and preferences. Without effective data analytics and machine learning techniques, Syriatel risks losing market share and falling behind competitors who are more adept at leveraging these technologies to enhance customer experiences and loyalty.

## Introduction

Syriatel is a prominent mobile network provider in Syria. Alongside MTN Syria, it has been a key player in the country's telecommunications landscape. In 2022, the Syrian telecommunications authority awarded a third telecom license to Wafa Telecom, introducing new competition into the market. Syriatel offers LTE services with speeds up to 150 Mb/s under the brand name Super Surf. In this increasingly competitive environment, it is imperative for Syriatel to continuously adapt and enhance its services to remain competitive and provide outstanding customer experiences.

## Stakeholders**

The success of the project is intrinsically tied to the satisfaction of a diverse set of stakeholders:

*Syriatel Executives:* Leadership needs to maintain and expand their customer base, ensuring the long-term growth and sustainability of the company.

*Syriatel Marketing Team:* The marketing department aims to increase customer acquisition, engagement, and the delivery of targeted promotions.

*Syriatel Customer Support Team:* The customer support team seeks to provide efficient and effective customer service, resolving issues, and improving overall customer satisfaction.

*Syriatel Customers:* The end-users, who expect reliable, affordable, and innovative telecommunications services.

# Business and Data Understanding

Syriatel Mobile Telecom, amidst the challenges posed by competitive telecommunication markets, emphasizes the importance of improving customer satisfaction and retaining its significant clientele of 8 million subscribers. Acknowledging the potential threat of customer churn to its market standing, profitability, and overall growth, the company aims to undertake proactive measures. These include leveraging data analytics to identify customers with a higher propensity to churn. By understanding customer behavior, usage patterns, and preferences, Syriatel intends to implement tailored strategies to mitigate churn risk. Such initiatives are crucial not only for reducing costs associated with customer turnover but also for fostering long-term customer loyalty and driving sustainable business growth.

The proposed model presents significant benefits for all stakeholders involved. For the company, it offers the potential to reduce customer churn rates, leading to increased revenues, profits, and market sustainability. Customers stand to gain from improved telecommunication services and enhanced customer support. Shareholders can expect higher returns on their investments as the company grows in terms of revenues, profits, customer base, and market share. Additionally, employees are likely to benefit from improved remuneration packages and bonuses as the company thrives. Overall, the model fosters mutual growth and prosperity for all stakeholders.

The project aims to provide value to the different stakeholders by identifying predictable patterns related to customer churn, which can help SyriaTel take proactive measures to retain customers and minimize revenue loss.

## Data Understanding

The Churn in Telecom’s dataset from Kaggle contains information about customer activity and whether or not they canceled their subscription with the Telecom firm. The goal of this dataset is to develop predictive models that can help the telecom business reduce the amount of money lost due to customers who don’t stick around for very long.

The dataset contains 3333 entries and 21 columns, including information about the state, account length, area code, phone number, international plan, voice mail plan, number of voice mail messages, total day minutes, total day calls, total day charge, total evening minutes, total evening calls, total evening charge, total night minutes, total night calls, total night charge, total international minutes, total international calls, total international charge, customer service calls and churn.

In this phase of the project, we will focus on getting familiar with the data and identifying any potential data quality issues. We will also perform some initial exploratory data analysis to discover first insights into the data.

# Modeling

Modeling Summary and Evaluation
In this project, various machine learning models were employed to predict customer churn for Syriatel, including Logistic Regression, Decision Tree, Random Forest, and XGBoost.

Logistic Regression:

Initial accuracy was 86%, but recall was low (18% for churned customers).
Rebalancing improved recall to 77% but reduced accuracy to 78%.
ROC AUC: 0.83.
Decision Tree:

Initial accuracy: 86%.
Improved with SMOTE: accuracy 76%, precision 35%, recall 73%, F1-score 47%.
ROC AUC: 0.81.
Random Forest:

Accuracy: 95%, precision: 96%, recall: 67%, F1-score: 80%.
Cross-validation accuracy: 95.05%.
ROC AUC: 0.94.
XGBoost:

Accuracy: 96.1%, precision: 96.3%, recall: 77.23%, F1-score: 85.71%.
ROC AUC: 0.93.

# Evaluation

Evaluation:
The Random Forest model demonstrated the best overall performance with a high ROC AUC of 0.94, making it the recommended model for predicting customer churn at Syriatel. This model effectively balances accuracy, precision, recall, and F1-score, ensuring reliable identification of churned customers while maintaining high performance on unseen data.

# Conclusion

The analysis concludes that customer churn can be accurately predicted using machine learning models, with the Random Forest Classifier emerging as the recommended model due to its superior overall performance. This model demonstrates the highest Area Under the Curve (AUC) in the ROC curve, indicating its strong classification capabilities and reliability in predicting churn.