# sms-spam-predictor

This code represents a complete pipeline for SMS spam detection using natural language processing (NLP) and machine learning models. Below is a breakdown of its structure:

# 1. Data Loading and Preprocessing:
   - Data Cleaning: Unnecessary columns are dropped, and missing and duplicate values are handled.
   - Text Preprocessing: The text data is transformed by lowercasing, tokenizing, removing special characters, stopwords, punctuation, and applying stemming.

# 2. Exploratory Data Analysis (EDA):
   - Various features such as number of characters, words, and sentences are extracted from the text.
   - Visualization of spam and ham distributions is performed using histograms and pie charts.

# 3. Feature Engineering:
   - TF-IDF (Term Frequency-Inverse Document Frequency) is used to vectorize the text into numerical features for model building.

# 4. Model Building:
   - Several machine learning models are trained, including Naive Bayes (Gaussian, Multinomial, Bernoulli), Logistic Regression, Support Vector Classifier (SVC), Random Forest, XGBoost, Gradient Boosting Classifier, Extra Trees Classifier, Bagging Classifier, Ada Boost Classifier.
   - Performance metrics like accuracy and precision are calculated for each model.

# 5. Model Evaluation and Comparison:
   - All models are compared based on their accuracy and precision scores, which are visualized using bar plots.
   
# 6. Model Improvement:
   - The TF-IDF `max_features` parameter is tweaked, and additional features like the number of characters are appended to the model to improve performance.
   - Voting Classifier is also introduced, which combines the predictions of different models for better results.

If you want to improve or modify the code, you can:
1. Adjust the `max_features` of TF-IDF to capture more or fewer words.
2. Try scaling the data using MinMaxScaler for different models.
3. Experiment with hyperparameter tuning for each classifier.
