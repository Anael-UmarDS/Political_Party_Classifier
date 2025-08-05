# Political Party Classifier Using Tweets  
**Author**: Anael Umar  
**GitHub:** [Anael-UmarDS](https://github.com/Anael-UmarDS)

---

# Description

This project classifies tweets written by US politicians as either **Democratic** or **Republican**, using a **supervised machine learning approach**. Tweets are processed with **TF-IDF vectorization**, and a **Logistic Regression classifier** is trained to predict the political party based solely on the tweet's content. This project demonstrates real-world **natural language processing (NLP)**, **feature engineering**, and **binary classification**, applied to political data.

---

# Objectives

- Use **supervised learning** to **classify** political tweets into Democratic or Republican categories  
- Understand how **political language differs by party affiliation** 
- Build a clean, interpretable **machine learning pipeline** using scikit-learn  
- **Apply NLP** techniques on real-world, publicly available tweet data  
- Develop skills in **preprocessing, feature extraction, and model evaluation**
- Explores how **data science** intersects with **government and civic technology**

---

# Source of Datasets

[Kaggle Dataset for **dataset.csv**](https://www.kaggle.com/datasets/mrmorj/us-politicians-twitter-dataset)

[Kaggle Dataset for **us_tweets.csv**](https://www.kaggle.com/datasets/jeevanbhoot/tweets-from-us-politicians)

---
# How It Works

### Data Preparation  
- Tweets were gathered from U.S. politicians, merged with a dataset containing each user's party affiliation  
- Only tweets from **Democratic Party** and **Republican Party** members were retained  
- Merged dataset included:  
  - `Name`, `Twitter_username`, `Political_party`, and `text`

### Text Preprocessing  
Each tweet undergoes data cleaning:
- Lowercasing  
- Removing URLs, mentions, hashtags, and punctuation  
- Removing common stopwords  
- Final cleaned text is stored for vectorization

### Feature Extraction (TF-IDF)  
- **TfidfVectorizer** converts each cleaned tweet into a **feature vector**
- Captures the **importance** of each word **relative** to the **entire dataset**

### Model Training (Logistic Regression)  
- Binary labels:
  - **Democratic Party** 
  - **Republican Party** 
- Model is trained using **LogisticRegression** from scikit-learn  

---

# Example Use Cases

- **Civic Tech**: Understand how politicians from different parties frame similar topics  
- **Political Science Research**: Study the linguistic differences in party messaging  
- **Media Literacy**: Recognize bias through language cues

---

# Visualizations

- **Confusion Matrix** for evaluating prediction accuracy  
- **Word importance** (TF-IDF weights) by class
- **Sample predictions** of tweet text with predicted party label  

---

# Limitations

- **Dataset Bias**: Only includes verified U.S. politicians; may not generalize to regular users  
- **Context Missing**: A single tweet may not represent a user's overall ideology  
- **Imbalanced Data**: Class imbalance can affect generalization (requires resampling if necessary)  
- **Linguistic Ambiguity**: Some tweets may appear neutral but still hold ideological undertones  

---

# Conclusions
- **TF-IDF + Logistic Regression** performs well in classifying political party from tweet content
- Simple **NLP methods** can reveal **deep political divisions** in language use
- **Machine learning** can support **political discourse analysis, civic education, and transparency**

# Implications
### Government & Civics
- Understand how **partisan messagin**g is framed
- Provide **transparency** in political communication

### Political Research
- **Track** evolving **language by party** over time
- Study **messaging strategy** and framing during election campaigns

### AI & ML Development
- Uses explainable **machine learning models** for interpretable results

# Machine Learning Concepts
- Supervised Learning
- Binary Classification
- Text Cleaning & Preprocessing
- TF-IDF Feature Engineering
- Logistic Regression
- Label Encoding
- Evaluation Metrics
