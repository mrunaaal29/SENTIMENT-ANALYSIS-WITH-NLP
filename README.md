# SENTIMENT-ANALYSIS-WITH-NLP

*COMPANY *: CODTECH IT SOLUTIONS

*NAME *: MRUNAL TAYDE

*INTERN ID *: CTIS7006

*DOMAIN *: MACHINE LEARNING

*DURATION *: 4 WEEEKS

*MENTOR *: NEELA SANTOSH

SENTIMENT ANALYSIS WITH NLP

1. Introduction

This project focuses on performing sentiment analysis on customer reviews using Natural Language Processing (NLP) techniques. Sentiment analysis is an important task in text mining and machine learning, where the objective is to determine whether a given text expresses a positive or negative sentiment. In this project, the dataset used contains customer reviews of the Uber mobile application collected from the Google Play Store. These reviews reflect real user experiences, complaints, and satisfaction levels, making the dataset suitable for training a sentiment classification model.

The primary goal of this project is to preprocess the review text, convert it into numerical features using the TF-IDF vectorization method, and then build a Logistic Regression model to classify sentiments as either positive or negative. The entire implementation is carried out in a Jupyter Notebook environment.

2. Dataset Description

The dataset used is the "Uber Customer Reviews Dataset 2024" sourced from Kaggle. It contains over twelve thousand customer reviews in textual format, along with a numerical rating score ranging from 1 to 5. These scores represent the user’s rating for the Uber application on the Play Store.

In this project, the review text is extracted from the "content" column, while the rating score is taken from the "score" column. To convert these numerical ratings into sentiment labels:

Ratings 4 and 5 are classified as positive sentiment (label 1).
Ratings 1 and 2 are classified as negative sentiment (label 0).
Rating 3 is considered neutral and removed from training for binary classification.

This conversion allows us to build a clear binary sentiment analysis model.

3. Project Workflow Overview

The project consists of three major phases: preprocessing, modeling, and evaluation. Each step is implemented carefully to ensure data quality and accurate predictions.

4. Preprocessing

Preprocessing is a crucial stage in any NLP task. The following steps are performed:

The dataset is loaded into a Pandas DataFrame.
Only the relevant columns (review text and score) are selected.
Missing values, if any, are detected and removed.
Rating values are mapped to sentiment labels based on the defined rules.
Rows with neutral ratings are excluded from further processing.
The dataset is split into training and testing sets using an 80:20 ratio.
Text data is transformed into numerical vectors using TF-IDF (Term Frequency–Inverse Document Frequency). This method converts words into weighted numerical features based on their importance in a document.

These preprocessing steps convert raw text into a clean, structured, and machine-understandable form.

5. Modeling

For sentiment classification, Logistic Regression is used as the machine learning model. Logistic Regression is a simple yet effective linear model widely used in binary classification tasks. The TF-IDF vectors obtained during preprocessing serve as input features for training the model.

The model is trained on the training set using the transformed text data, learning patterns and relationships between the words in a review and its corresponding sentiment label. After training, the model is tested on unseen data to evaluate its generalization capability.

6. Evaluation

To assess the model's performance, multiple evaluation metrics are used:

Accuracy score, which measures the percentage of correctly predicted labels.
Classification report, which includes precision, recall, F1-score, and support for each class.
Confusion matrix, which shows the number of correctly and incorrectly classified instances for each category.

These evaluation measures help determine how well the model performs on real-world sentiment classification. A higher accuracy and balanced performance across metrics indicate an effective sentiment analysis model.

7. Custom Prediction

The project also includes a section that allows users to test the model with custom sentences. Test sentences are passed through the TF-IDF vectorizer and then classified by the model. The predicted output indicates whether a sentence is positive or negative using labels 1 and 0.

8. Tools and Technologies Used

The following tools, libraries, and technologies were used to complete this sentiment analysis project:

Python-
Python is used as the primary programming language due to its rich ecosystem of data science, NLP, and machine learning libraries.

Jupyter Notebook-
The entire code execution, analysis, visualization, and documentation are performed in Jupyter Notebook. It is suitable for interactive workflows and step-by-step experimentation.

Pandas-
Pandas is utilized for loading the dataset, handling missing data, selecting columns, filtering records, and performing data manipulation tasks.

NumPy-
NumPy provides numerical computation support, especially for operations required in machine learning and vector transformations.

Scikit-learn -
The core machine learning framework used in this project.

Modules included:
TfidfVectorizer for text vectorization

train_test_split for dataset splitting

LogisticRegression for modeling

accuracy_score, confusion_matrix, and classification_report for evaluation


Matplotlib and Seaborn-
These libraries are used for data visualization, specifically for generating plots such as class distribution and confusion matrix heatmap.

Kaggle Dataset-
The Uber Customer Reviews Dataset 2024 from Kaggle is used as the source of text data.

9. Development Environment / Editor Platform

This project is executed in the following development environment:

Anaconda Distribution-
Anaconda provides a stable Python environment, package management, and easy installation of required libraries. It includes Jupyter Notebook, which is used as the code editor.

Jupyter Notebook-
Jupyter Notebook is chosen because it allows step-by-step execution, inline visualizations, and combining code with explanations in a single document. This makes it ideal for data science and machine learning tasks.

Windows Operating System-
The project has been implemented on a Windows-based system. However, the code is platform-independent and can run on Linux or macOS as well.

Git and GitHub-
This project can be pushed to a GitHub repository for version control, sharing, and documentation.

10. Applications of Sentiment Analysis (Where This Task is Applicable)

Sentiment analysis is widely applied in multiple industries and domains. The model developed in this project demonstrates a practical use case of text-based opinion classification. The following are real-world applications:

Customer Feedback Analysis:
Companies can analyze product reviews, app reviews, or service feedback to understand customer satisfaction and areas needing improvement.

Brand Monitoring:
Organizations track online discussions and sentiments about their brand across platforms such as Google Play Store, App Store, Twitter, and other social media channels.

Product Improvement Decisions:
User reviews can be categorized to identify recurring issues, prioritize feature requests, or improve user experience.

Market Research:
Sentiment analysis helps businesses evaluate how customers perceive their competitors, products, or marketing campaigns.

Chatbot and Virtual Assistant Improvement:
Understanding sentiment in user messages allows chatbots to respond appropriately and improve customer interactions.

Customer Support Automation:
Support tickets can be auto-classified into positive or negative tone, allowing teams to prioritize urgent or dissatisfied users.

11. Conclusion

This project successfully demonstrates how Natural Language Processing and machine learning can be applied to classify customer reviews based on sentiment. By leveraging TF-IDF vectorization and Logistic Regression, the model can effectively distinguish between positive and negative feedback. This type of sentiment analysis is widely used in industry applications such as customer feedback monitoring, brand analysis, and automated review classification. The project provides a foundation that can be further improved using advanced NLP models or deep learning algorithms.

12. Output

1. First 5 rows of dataset
<img width="1938" height="390" alt="Image" src="https://github.com/user-attachments/assets/b5f139e8-cc1c-42e9-9e59-a770474a12e4" />


2.Converted scores into sentiment labels
<img width="966" height="418" alt="Image" src="https://github.com/user-attachments/assets/8c1db14c-b16b-41ce-b646-2163627e6f39" />


3.Distribution of sentiments
<img width="968" height="782" alt="Image" src="https://github.com/user-attachments/assets/c2af31d7-b9be-4715-95fa-ccb77ec5800a" />


4.Accuracy and classification report
<img width="812" height="588" alt="Image" src="https://github.com/user-attachments/assets/0bea2042-e5bc-410d-ba08-4f62bf91212a" />


5.Confusion matrix
<img width="1058" height="776" alt="Image" src="https://github.com/user-attachments/assets/64d2ef19-2245-4923-89de-4796b8cc601b" />


6.Custom example
<img width="920" height="1148" alt="Image" src="https://github.com/user-attachments/assets/64d396b1-e051-49a2-b9cf-b8e669e3c39f" />





