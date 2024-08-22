# Online News Popularity Prediction Using Machine Learning

## Project Overview

This project focuses on predicting the popularity of online news articles for a media company. The primary objective was to automate the process of selecting or rejecting contributed articles based on their potential to generate revenue through shares. The media company faces the challenge of efficiently curating a large volume of daily articles, and this project seeks to address that by implementing machine learning models to predict article popularity, measured by the number of shares each article receives.

## Problem Definition

The media company needs a reliable system to predict which articles will become popular and generate significant revenue through shares. Each share contributes $0.75 for the first 1000 shares and $2 per share thereafter. Given the substantial volume of articles published daily, a mechanized prediction system could significantly impact the company's revenue. The goal was to develop models that could accurately predict article popularity, thereby automating the curation process and optimizing revenue.

## Data Description

The dataset used in this project consists of nearly 40,000 articles with various features related to article content, display characteristics, and performance metrics. Non-predictive variables, such as 'url' and 'timedelta,' along with repetitive and outlier-prone columns, were removed to streamline the analysis. Additionally, categorical factors were converted to numeric values to facilitate the modeling process. While the dataset was comprehensive, the inclusion of additional features, such as social media engagement metrics, author reputation, and sentiment analysis, could further enhance the predictive models.

## Data Preparation

Before applying the models, the following data preparation steps were taken:
- **Removal of Non-predictive and Repetitive Variables**: Columns like 'url,' 'timedelta,' and 'is_weekend' were removed.
- **Outlier Treatment**: Columns with extreme outliers were carefully cleaned.
- **Conversion to Numeric Values**: Factor columns were converted to numeric for better correlation analysis and model compatibility.

## Model Selection and Analysis

Several machine learning models were employed to predict article popularity:

### 1. Linear Regression
The Linear Regression model aimed to predict the exact number of shares an article would receive. However, the model's performance was suboptimal, with low R-squared values indicating it was not suitable for this task.

### 2. Logistic Regression
To improve accuracy, a Logistic Regression model was used with a binary outcome variable indicating whether an article surpassed a threshold of 1,400 shares. This model showed better performance, making it a more viable option for predicting article popularity.

### 3. Decision Tree
A Decision Tree model was also tested to predict the number of shares. While it performed better than Linear Regression, the accuracy was still inadequate, indicating that the model was making predictions no better than random chance.

### 4. Random Forest
The Random Forest model was employed for binary classification but yielded accuracy similar to that of the Decision Tree model, suggesting that this approach was also not ideal for the task.

## Conclusion

This project explored multiple machine learning models to predict the popularity of online news articles. Despite the varied performance of the models, Logistic Regression emerged as the most promising approach, although the overall results highlight the complexity of predicting online content popularity. Further refinement of models and inclusion of additional data features could enhance predictive accuracy, offering a valuable tool for automating article curation and maximizing revenue.

![image](https://github.com/user-attachments/assets/4477dd55-efbe-40d2-93f6-7e4aee988f9c)
