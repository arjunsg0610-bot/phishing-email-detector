# Phishing Email Detection Mini-Model

A supervised machine learning project that classifies emails as phishing or legitimate using text feature extraction and multiple classifiers.

## Tools & Libraries
- Python, scikit-learn, Pandas
- Matplotlib, Seaborn
- Jupyter Notebook

## What This Project Does
- Built a labeled dataset of 500 phishing and legitimate email samples
- Extracted hand-crafted features including URL presence, urgency keywords, caps ratio, and suspicious domains
- Applied TF-IDF vectorization with unigrams and bigrams to convert text into numerical features
- Trained and evaluated 5 classifiers: Logistic Regression, Naive Bayes, Linear SVM, Random Forest, and Gradient Boosting
- Achieved 82% accuracy on test data with 5-fold cross-validation
- Analyzed confusion matrix to assess false positives and false negatives

## Key Findings
- Urgency language and suspicious URLs were the strongest phishing indicators
- TF-IDF bigrams effectively captured multi-word phishing phrases
- False negatives (missed phishing) are more costly than false positives in real-world deployment
- Logistic Regression provided the best interpretability via feature coefficients

## Files
| File | Description |
|------|-------------|
| `phishing_detection.ipynb` | Full model notebook with feature extraction, training, evaluation, and predictions |

## How to Run
1. Clone the repo
2. Install dependencies: `pip install pandas numpy matplotlib seaborn scikit-learn`
3. Open `phishing_detection.ipynb` in Jupyter or VS Code
4. Run all cells top to bottom
