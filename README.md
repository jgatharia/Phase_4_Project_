# Twitter Sentiment Analysis for Apple and Google Products

![Visualizations](attachment:Project_Image.jpg)

# Project Overview

NiaTech has embarked on a project to enhance customer engagement and refine marketing strategies through sentiment analysis of tweets related to Apple and Google products. Over the past year, the company has actively marketed and sold products from these tech giants, and with a significant portion of customer interactions occurring on Twitter, understanding public sentiment has become crucial.

This project aims to develop a machine learning model capable of classifying sentiments expressed in tweets as positive, negative, or neutral. By accurately categorizing these sentiments, NiaTech will gain valuable insights into customer perceptions, identify potential issues, and uncover opportunities for improvement.

# Objectives

>- Develop a machine learning model to correctly classify sentiments in tweets as positive, negative, or neutral regarding Apple and Google products.
>- Identify and analyze which product has the highest and lowest sentiment scores, highlighting areas for potential improvement.
>- Assess the overall sentiment trends towards Apple and Google to inform NiaTech’s strategic decision on continuing partnerships with these companies.

# Data Understanding

The dataset used is sourced from https://data.world/crowdflower/brands-and-product-emotions consisting of 3 columns and 9093 rows. The columns include; Tweet, Sentiment and Product.

# Data Preparation

The data cleaning process involved several key steps to enhance clarity and eliminate redundancy. Column names were renamed for better understanding, and duplicate entries were removed. To ensure uniformity, all text was converted to lowercase, while imputing missing values helped maintain data integrity. During the NLP pre-processing phase, URLs, unnecessary terms, punctuation, and stopwords were removed to refine the text, resulting in a cleaner and more focused dataset that is well-suited for accurate emotion and sentiment extraction. The cleaning and manipulation tasks were efficiently handled using the Pandas and NLTK libraries, which provided specialized tools for text processing in NLP.

# Exploratory Data Analysis (EDA)

This phase provided valuable insights into the dataset, uncovering issues such as class imbalance in the target variable. These findings guided the subsequent analysis and model development for the project.

![Sentiment Count For Each Product](Sentiment_Count_For_Each_Product.png)
![Word Cloud For Visualization](Word_Cloud_For_Visualization.png)

# Modeling

In this section, I develop machine learning models to predict customer churn using the following algorithms:

* Logistic Regression
* Support Vector Machine (SVM)
* Random Forest
* Naive Bayes

In our sentiment analysis project, we investigated the effectiveness of different machine learning models for classifying text into sentiment categories. We utilized a variety of models to capture the subtleties of sentiment conveyed in the textual data. We evaluate and compare the performance of all the models, selecting the top performers for more in-depth analysis.

# Model Evaluation

The NLP model with Grid Search CV performed well, achieving an accuracy of 85.9% across all classes. The model's performance for negative sentiments, neutral sentiments, and positive sentiments was improved after hyperparameter tuning, leading to better overall classification results. The tuning process further enhanced the model's performance, making it more reliable for sentiment analysis tasks. The model's robustness and ability to handle diverse sentiments make it a valuable tool

# Summary Findings

1. The larger share ofsentiments were directed to the Apple Products, pointing to the fact that the brand was more dominant compared to google products
2. Neutral sentiments towards the products was higher compared to the positive and negative sentiments

# Conclusion

Google and Apple products enjoy widespread usage worldwide. This study successfully achieved its objectives by analyzing the sentiment dynamics surrounding these products on Twitter. The NLP model, optimized using Grid Search CV, performed impressively, attaining an accuracy of 85.9% across all sentiment categories. Hyperparameter tuning significantly improved the model's performance for negative, neutral, and positive sentiments, resulting in enhanced overall classification results. This tuning process not only bolstered the model’s reliability for sentiment analysis tasks but also showcased its robustness and capacity to handle diverse sentiments, making it a valuable tool for deriving insights from customer feedback.

# Future Work

* Extend Time Frame for Analysis: Analyze sentiment over a longer period to identify trends and impacts of product launches and events.
* Segment Analysis by Demographics: Analyze sentiment based on age, gender, and location to tailor marketing strategies effectively. 
* Develop Predictive Models: Create models to anticipate shifts in sentiment, allowing clients to adjust strategies proactively.
* Integrate Insights with Clients: Collaborate with clients to weave sentiment insights into marketing strategies, content creation, and social media campaigns.

# For More Information
See the full analysis in the [Juptyer Notebook](robert.ipynb) or review the[Presentation](Presentation.pdf)