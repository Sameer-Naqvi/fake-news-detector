Fake News Detection
This repository contains a Python script for detecting fake news using a Support Vector Machine (SVM) classifier. The model is trained on a dataset of news articles and predicts whether a given article is real or fake.

Overview
The script follows these main steps:

Data Loading: Loads a dataset of news articles from a CSV file.
Preprocessing: Converts the labels to numerical values (0 for real news, 1 for fake news) and splits the dataset into training and testing sets.
Feature Extraction: Transforms the text data into numerical features using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization.
Model Training: Trains a Linear Support Vector Machine (SVM) classifier on the vectorized training data.
Evaluation: Evaluates the model on the test data and prints the accuracy score.
Dataset
The dataset used in this script is assumed to be in CSV format with the following structure:

text: The content of the news article.
label: The label indicating whether the news is "REAL" or "FAKE".
Requirements
To run this script, you need the following Python libraries:

numpy
pandas
scikit-learn
You can install the required libraries using pip:

bash
Copy code
pip install numpy pandas scikit-learn
Usage
Prepare the Dataset:
Ensure you have the dataset file named fake_or_real_news.csv in the same directory as the script. The CSV file should have two columns: text and label.

Run the Script:
Execute the script in your terminal:

bash
Copy code
python fake_news_detection.py
Output:
The script will output the accuracy of the model on the test data, which indicates how well the model performs in predicting whether a news article is real or fake.
