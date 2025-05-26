# Hatespeech-Detection
HateSpeech Detection for beginers with a 87% accuracy rate using CountVectorizer and train_test_split methods to segregate data, then using confusion matrix and heatmap to visualize the following.


# Hate Speech Detection using Decision Tree Classifier

This project performs hate speech and offensive language classification on tweets using a **Decision Tree Classifier**. It involves preprocessing a labeled dataset, cleaning the text, transforming it into features, and then training/testing a model to classify the content of the tweets.

---

## Dataset

The dataset used is `labeled_data.csv` which includes:

* `tweet`: The actual tweet text.
* `class`: Category label (`0`: Hate Speech, `1`: Offensive Language, `2`: Neither).
* Additional columns like counts of hate speech, offensive language, and others.

---

## Features of the Project

* Loads and inspects the dataset.
* Cleans the text (lowercasing, punctuation removal, stopwords removal, stemming).
* Encodes the text using **CountVectorizer**.
* Splits the dataset into training and testing sets.
* Trains a **Decision Tree Classifier**.
* Evaluates the model with a **confusion matrix** and **accuracy score**.
* Predicts label for a custom input sample.

---

## Installation and Requirements

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

2. Install required packages:

   ```bash
   pip install pandas numpy nltk scikit-learn seaborn matplotlib
   ```

3. Download NLTK stopwords:

   ```python
   import nltk
   nltk.download("stopwords")
   ```

---

## How It Works

1. **Data Preprocessing**:

   * Lowercase conversion
   * Removal of URLs, special characters, digits
   * Stopword removal and stemming

2. **Feature Extraction**:

   * Uses `CountVectorizer` to convert text into numeric format

3. **Model Training**:

   * Applies a `DecisionTreeClassifier` from scikit-learn

4. **Evaluation**:

   * Uses accuracy and a heatmap of the confusion matrix to assess performance

5. **Prediction**:

   * Accepts new tweet text and classifies it as:

     * Hate Speech
     * Offensive Language
     * No hate nor offensive language

---

## Sample Output

```python
Sample: "Lets unite and Kill all the people who are protesting against the government"
Predicted Class: Hate Speech
```

---

## Results

* **Accuracy**: \~87.32%
* Confusion Matrix visualization included via seaborn

---

