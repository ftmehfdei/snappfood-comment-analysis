# Persian SnappFood Sentiment Analysis
An end-to-end NLP project for classifying Persian customer reviews from SnappFood (Iran's leading food delivery platform) into positive (HAPPY) and negative (SAD) sentiments.
# Dataset
Size: 70,000 labeled Persian comments
Classes: HAPPY (Positive) - 34,916 | SAD (Negative) - 34,564
Balance: Nearly perfect 50.3% / 49.7% split
Source: Real user reviews from SnappFood platform
# Model Performance
Best CV Accuracy	: 82.39%
Test Accuracy	: 82.02%
Cross-Validation : 3-Fold
Samples	: 70,000
#  Methodology
1. Persian Text Preprocessing
python
✅ Encoding fix (cp1256 → utf-8)
✅ Arabic-to-Persian normalization
✅ Hashtag/URL removal
✅ Persian stopword filtering
✅ Tokenization

3. Feature Extraction
TF-IDF Vectorization with:
Max features: 5,000
N-gram range: (1, 2) - unigrams + bigrams

3. Model Training
Algorithm: Logistic Regression
Hyperparameter Tuning: GridSearchCV (3-fold)
Regularization: C=1.0
Solver: liblinear

4. Evaluation
Train/Test split: 80/20
Cross-validation: 3-fold
Metrics: Accuracy, Precision, Recall, F1-Score
