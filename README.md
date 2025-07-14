#  Fake News Detection using Machine Learning

Detect whether a  news article is **real or fake** using a supervised machine learning model.
---

## Overview

With the rise of misinformation, being able to detect fake news has become a critical task. This project:
- Uses a Kaggle dataset containing labeled fake and real news articles. The dataset is given in zipped form just extract the dataset and use it.
- Applies text preprocessing and NLP techniques.
- Trains a Logistic Regression model using TF-IDF feature vectors.
- Evaluates the model’s accuracy and enables real-time prediction.

---

##  Tech Stack & Tools

| Category        | Tools/Libraries                                   |
|----------------|---------------------------------------------------|
| Language        | Python                                            |
| Notebook        | Google Colab                                      |
| Libraries       | Pandas, NumPy, NLTK, Sklearn, Matplotlib, Seaborn |
| NLP Techniques  | Stemming, Stopwords Removal, TF-IDF Vectorizer    |
| Model           | Logistic Regression                               |

---

## Dataset

Structure of dataset:
- **title**: Title of the article  
- **text**: Full text of the article  
- **subject**: he news is of which type
- **date**: contains the date of the news
- **label**: 0 for Real, 1 for Fake  

Also a modified dataset can be used where:
- Fake and Real articles are in separate folders or CSV files.
- Merging logic is applied to unify and label them.

---

## Visualizations

The project includes the following visualizations:
-  Distribution of Fake vs Real News  
-  Top 20 Most Frequent Words  

---

##  Model Workflow

1. **Data Loading**
2. **Handling Missing Values**
3. **Using Title Column Only** – Only the `title` column was used for predictions, as merging with other columns like `subject` or `text` increases processing time.
4. **Text Cleaning & Stemming**
5. **TF-IDF Vectorization**
6. **Splitting Dataset**
7. **Training Logistic Regression Model**
8. **Accuracy Evaluation**
9. **Prediction System**

---

##  Accuracy

| Dataset       | Accuracy  |
|---------------|-----------|
| Training Set  |   ~96%    |
| Testing Set   |   ~94%    |

---

## How to Run the Project

### Option 1: Using Google Colab

1. Open the `.ipynb` notebook in Google Colab.
2. Upload the dataset (CSV or merged version).
3. Run all cells in order.
4. You can test predictions by modifying the final input examples.

###  Option 2: Manual

1. Clone this repository  
   ```bash
   git clone https://github.com/<your-username>/fake-news-detection.git
