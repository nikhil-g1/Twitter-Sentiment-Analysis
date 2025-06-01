# Twitter-Sentiment-analysis
- ## **Dataset**
The dataset was collected from kaggle Sentiment140 dataset with 1.6 million rows.
This is a real-world data of 1.6 million rows having tweets from across the globe. The dataset contains wide range of topics from fashion, tech, sports, politics to ongoing trends.
- ## **NLP Technique**
In this project I used various nlp techniques like--
1. Text Cleaning- Using regular expression to clean username, url, special characters, digits.
2. Translation- Using Google Translator to transform Non-English words to English.
3. Tokenization- Splitting text by spaces or periods.
4. Abbreviation Expansion- Using NLTK to get expansion.
5. POS Tagging- Tagging pos in every tweet.
6. POS Count- Making features of pos by count.
7. Stemming- Using Porter Stemmer to reduce to root word.
8. Word Embedding- Used various techniques like BOW, TF-IDF & N-Grams to convert text data to numerical format.
9. Sentence Transformer- Used hugging face BERT sentence transformer model to make more good features out of it. Evaluated using three
                          different transformers.
11. Text-Length Based Features- Added features like char_count, word_count, unique_word_ratio, sentence_count & more.
- ## **Feature Engineering**
1. Selecting top 500 features by average value for Tf-IDF & N-Gram.
2. Evaluating feature importances using Random Forest Classifier and selecting top 100 features by average value.
- ## **Modelling**
  Splitted the data into into X & y and train & test split.
  Aplied different algorithms like-
1. Random Forest Classifier- Did hyperparameter tuning using randomizedsearchcv and evaluated precision & F1 Score. Plotted classificaton
                             report. Saving model object using joblib.dump.
2. Logistic Regression- Did hyperparameter tuning using randomizedsearchcv and evaluated precision & F1 Score. Plotted classificaton
                        report. Saving model object using joblib.dump.
3. XGBoost Model- Did hyperparameter tuning using randomizedsearchcv and evaluated precision & F1 Score. Plotted classificaton
                  report. Saving model object using joblib.dump.
- ## **Model Performance**
  XGBoost & Random Forest both achieved highest accuracy of 72.1% but XGBoost had a slightly better F1 SCore (73.15 vs 72.1%) than random    forest indicating slightly better precision-recall balance. Logistic REgression performed significantly worse, with 59.2% accuracy and     60.2% F1 Score, suggesting it couldn't capture complex patterns as well as the tree based models. Overall, XGBoost is the performed
  model due to it's strnger F1 score and accuracy.
- ## **SHAP**
  Plotted 10 features using shap for feature explainability. Explained it's Features, Impact & Business Implications. 
