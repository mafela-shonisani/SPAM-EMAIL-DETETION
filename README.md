# SPAM-EMAIL-DETETION

## Overview

Email has become one of the most widely used communication tools in the world. However, the increasing number of spam emails poses a significant challenge to individuals, businesses, educational institutions, and communities. Spam emails often contain advertisements, phishing attempts, fraudulent offers, and malicious links that can compromise users' security and privacy.

This project presents a Machine Learning-based Spam Email Detection System that automatically classifies email messages as either **Spam** or **Ham (Not Spam)**. The system aims to improve digital safety by helping users identify and filter unwanted emails before they cause harm.

## Problem Statement

Spam emails continue to affect millions of users worldwide. These messages can:

* Expose users to phishing attacks and online scams.
* Contain harmful links and malicious content.
* Waste time by cluttering inboxes with unwanted messages.
* Create cybersecurity risks for individuals and organizations.

Manually filtering spam emails is inefficient and often unreliable. An automated solution can help users manage their inboxes more effectively while reducing exposure to cyber threats.

## Project Objectives

* Develop a machine learning model capable of detecting spam emails.
* Automatically classify email messages as spam or ham.
* Improve email security and user experience.
* Demonstrate the practical application of Machine Learning and Natural Language Processing (NLP) in solving real-world problems.

## Dataset

The project uses a labeled email dataset containing two main features:

| Feature  | Description                                  |
| -------- | -------------------------------------------- |
| Category | Indicates whether the message is Spam or Ham |
| Message  | The text content of the email                |

## Methodology

### 1. Data Collection

The dataset was imported from a CSV file containing labeled email messages.

### 2. Data Cleaning

Data preprocessing included:

* Removing duplicate records.
* Removing missing values.
* Converting categorical labels into numerical values.
* Preparing the dataset for machine learning analysis.

### 3. Data Preparation

The dataset was divided into training and testing sets using an 80:20 ratio. TF-IDF (Term Frequency-Inverse Document Frequency) Vectorization was applied to transform text data into numerical features suitable for machine learning models.

### 4. Model Development

A **Multinomial Naive Bayes Classifier** was selected because it is widely used for text classification problems and performs efficiently on spam detection tasks.

### 5. Model Training

The model was trained using the processed training dataset to learn patterns associated with spam and legitimate emails.

### 6. Prediction

The trained model was used to classify unseen email messages as either spam or ham.

### 7. Model Evaluation

Model performance was evaluated using:

* Accuracy Score
* Confusion Matrix
* Precision
* Recall
* F1-Score

## Results

### Model Performance

| Metric         | Value  |
| -------------- | ------ |
| Accuracy       | 96.32% |
| Spam Precision | 100%   |
| Spam Recall    | 70%    |
| Spam F1-Score  | 83%    |

### Confusion Matrix

```text
[[904   0]
 [ 38  90]]
```

### Interpretation of Results

The model successfully classified the majority of email messages.

* Correctly identified **904 legitimate emails**.
* Correctly identified **90 spam emails**.
* Missed **38 spam emails**.
* Did not incorrectly classify any legitimate email as spam.

These results demonstrate that the model is highly effective at identifying spam emails while minimizing false alarms.

## Technologies Used

* Python
* Jupyter Notebook
* Anaconda
* Pandas
* Scikit-learn
* TF-IDF Vectorizer
* Multinomial Naive Bayes

## Example Predictions

| Email Message                                | Prediction |
| -------------------------------------------- | ---------- |
| Congratulations! You have won a free iPhone. | Spam       |
| Hi, are we still meeting tomorrow?           | Ham        |

## Community Impact

This project addresses a real-world problem by helping users protect themselves from spam, phishing attempts, and online scams. By automatically identifying suspicious emails, the system contributes to:

* Improved cybersecurity awareness.
* Safer digital communication.
* Reduced exposure to fraudulent emails.
* Better productivity through cleaner inboxes.

The project demonstrates how machine learning can be used to solve practical challenges faced by communities in the digital age.

## Future Improvements

Future enhancements may include:

* Comparing performance with Logistic Regression and Support Vector Machines (SVM).
* Increasing spam detection recall.
* Developing a web-based application for public use.
* Integrating real-time email filtering.
* Applying advanced Natural Language Processing techniques.

## Project Structure

```text
spam-email-detection/
│
├── spam.csv
├── spam_detection.ipynb
├── README.md

```

## Author

**Shonisani Mafela**

Final-Year BSc Mathematical Sciences Student (Computer Science & Statistics)

Aspiring Data Scientist with interests in Machine Learning, Data Analytics, Artificial Intelligence, and solving real-world problems through data-driven solutions.
