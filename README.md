# CS412 - Machine Learning Project

## Overview

With this project, we aimed to predict the first assignment grades of the CS-412 course by using students' ChatGPT conversation histories.

- Atahan Bozkuş - 28471
- Emir Ay - 28150


## Methodology

1) Data Preparation and Preprocessing

- a) Parsing HTML Files
  The data set used consists of HTML files. In this step, unnecessary data is eliminated and useful data is selected. This process is important to make the data set more manageable and suitable for analysis.

- b) Data Cleansing
  Data cleaning processes are carried out to ensure the quality of the data and make it suitable for analysis. At this stage, noisy and incomplete data are corrected, and formatting and standardization processes are applied.

- c) Incomplete Data Processing
  Handling of missing data is performed to maintain the integrity of the analysis and improve code performance. Missing data are carefully handled to avoid biases and improve the accuracy of the model.
  
2) Feature Engineering

- a) Tokenization
  Text data is broken down into smaller pieces (tokens) that can be analyzed. This process allows for more detailed examination and processing of texts.

- b) Request Analysis
  Request analysis is performed to understand user preferences and concepts. This process is important to better adapt to users' needs and preferences.

- c) Keyword Analysis
  Analysis of keywords in texts helps categorize data and better understand the content.

- d) Sentiment Analysis
  It is used to analyze emotional tones in texts and understand users' feelings and attitudes.
  
3) Vectorization and Similarity Measurement

- a) Cosine Similarity
  Cosine similarity is used to measure similarities between texts. This metric is especially important in situations such as prompt matching.

- b) Vectorization
  Texts are converted into numerical vectors into a format that machine learning algorithms can process.

4) Model Evaluation

- a) Training and Testing Divisions
  To test the generalization ability of the model, the data set is divided into training and test sets. This stage is critical to evaluate how the model performs on different data.

- b) Mean Square Error (MSE)
  MSE is a metric used to evaluate the performance of the model. A lower MSE value indicates a better fit of the model to the data, which is a factor that increases the success of the model.
  

## Code Representation

1) Library Imports
- Notebook starts by importing various Python libraries. These libraries include common data analysis and machine learning libraries such as matplotlib, seaborn, pandas, numpy, sklearn. This step ensures that the necessary tools are available for the data analysis and modeling process. In particular, the sklearn library offers various functions for model training and evaluation.
-------------------------------
2) Text Preprocessing
- The text preprocessing step is a key component of natural language processing (NLP) applications. The preprocess_text function defined here cleans up text, making it more suitable for machine learning models. The function performs operations such as converting text to lowercase, clearing non-alphanumeric characters, and removing stop words.
-------------------------------
3) Data Extraction and Cleansing Procedures
- This section includes extracting and cleaning dialog and code data from HTML files. The extract_and_clean_code function is used to extract and organize the necessary information from the HTML content. This process is critical to make the data ready for analysis.
-------------------------------
4) Clearing Non-ASCII Characters
- This step ensures that non-ASCII characters are removed from the text data. This process helps make text data more consistent and suitable for analysis. The clean_text function performs this operation and is applied to the texts.
-------------------------------
5) Data Analysis and Visualization
- Later sections of the notebook include data analysis and visualization steps. In these steps, various analyzes are performed on the data sets using matplotlib and seaborn libraries and the results are visualized. These visualizations make it easier to understand data and gain insights.
------------------------------
6) Model Training and Evaluation
- In the model training section, machine learning models are trained and evaluated using various functions of the sklearn library. This process includes the steps of separating the data set into training and test sets, training the model, and evaluating its performance. Model evaluation is typically done using error metrics and cross-validation methods.
------------------------------
7) Conclusion and Evaluation
- Importing Model Performance Metrics: 
At the beginning of the notebook, the metrics to be used for model evaluation are imported. In this section, the from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score line makes the Mean Absolute Error (MAE), Mean Squared Error (MSE) and R-Square (R²) metrics ready for use to evaluate the performance of the model. These metrics are standard tools for measuring how accurate the model's predictions are.
- Calculating and Displaying R-Square Value: 
In another code cell, the performance of the model on the test data set is evaluated. Here, the R-Square value was calculated using the r2_score function. R-Square is a metric that shows how much of the variance in the data set the model can explain. A high R-Square value indicates that the model explains the data well. It measures whether the model makes predictions on the test set and how compatible these predictions are with the real values. The resulting R-Square value reflects the overall success of the model and is used as an important indicator when evaluating the performance of the model.

---------------------------
Detailed graphics and anaylsis is in the Report.pdf file.
