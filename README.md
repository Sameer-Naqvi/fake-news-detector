<h1> Fake News Detection </h1>
This repository contains a Python script for detecting fake news using a Support Vector Machine (SVM) classifier. The model is trained on a dataset of news articles and predicts whether a given article is real or fake.

<h2> Overview </h2>
The script follows these main steps:

<b>Data Loading:</b> Loads a dataset of news articles from a CSV file. <br>
<b>Preprocessing:</b> Converts the labels to numerical values (0 for real news, 1 for fake news) and splits the dataset into training and testing sets. <br>
<b>Feature Extraction:</b> Transforms the text data into numerical features using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization. <br>
<b>Model Training:</b> Trains a Linear Support Vector Machine (SVM) classifier on the vectorized training data.<br>
<b>Evaluation:</b> Evaluates the model on the test data and prints the accuracy score.

<h2> Dataset </h2>
The dataset used in this script is assumed to be in CSV format with the following structure:<br>

<b>text:</b> The content of the news article.<br>
<b>label:</b> The label indicating whether the news is "REAL" or "FAKE".<br>

<h2> Requirements </h2>
To run this script, you need the following Python libraries:<br>
<b>numpy</b><br>
<b>pandas</b><br>
<b>scikit-learn</b><br>
You can install the required libraries using pip:<br>
<b>pip install numpy pandas scikit-learn</b>

<h2> Usage </h2>
<b>Prepare the Dataset:</b>
Ensure you have the dataset file named fake_or_real_news.csv in the same directory as the script. The CSV file should have two columns: text and label.<br>

<b>Run the Script:</b>
Execute the script in your terminal:
<b>python fake_news_detection.py</b><br>
<b>Output:</b>
The script will output the accuracy of the model on the test data, which indicates how well the model performs in predicting whether a news article is real or fake.
