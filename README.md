
# 💬 Comment Categorization & Reply Assistant Tool

## 🎯 Objective
The goal of this project is to develop an intelligent system that automatically **analyzes, classifies, and responds** to user comments based on their **emotion or intent**.  
This tool can assist **brands, creators, and customer service teams** in engaging with their audience more efficiently and empathetically.

## 🧠 Project Description
This project leverages **Natural Language Processing (NLP)** and **Machine Learning** to classify user comments into various emotional and intent-based categories such as:

- ❤️ Praise – positive feedback or appreciation  
- 😡 Hate/Abuse – offensive or harmful content  
- 😢 Emotional – personal or emotional connections  
- 🚨 Threat – threatening statements or warnings  
- 💬 Support – encouraging or friendly comments  
- 🧩 Constructive Criticism – helpful suggestions or mild criticism  
- 🗑️ Irrelevant/Spam – spammy or unrelated content  
- ❓ Question/Suggestion – inquiries or topic requests  

Each detected category is paired with a **context-aware automatic reply**, enabling the system to engage with users instantly.

## 🧰 Technologies & Libraries Used
- **Python**
- **pandas**, **numpy** → data preprocessing and analysis  
- **scikit-learn** → model training and evaluation  
- **nltk / spaCy** → text cleaning and tokenization  
- **TF-IDF Vectorization** → text feature extraction  
- **Logistic Regression / Random Forest** → model classification  

## 📊 Dataset Overview
- **Initial dataset shape:** 20,004 rows × 3 columns  
- **Final dataset shape:** (20004, 3) after preprocessing  
- The dataset contained labeled comments for supervised learnin

##Category Distribution:

| Category | Count |
|-----------|-------|
| Praise | 7480 |
| Emotional | 5797 |
| Hate/Abuse | 2709 |
| Threat | 2373 |
| Support | 1641 |
| Constructive Criticism | 2 |
| Irrelevant/Spam | 1 |
| Question/Suggestion | 1 |



## 📈 Model Performance
- **Model Accuracy:** `0.888` (88.8%)  
- **Precision, Recall, and F1-Score** indicate strong model performance in detecting **Praise**, **Hate/Abuse**, and **Support**.

| Metric | Precision | Recall | F1-score |
|--------|------------|---------|-----------|
| Praise | 0.96 | 0.89 | 0.92 |
| Emotional | 0.92 | 0.87 | 0.89 |
| Hate/Abuse | 0.94 | 0.93 | 0.93 |
| Support | 0.89 | 0.90 | 0.89 |
| Threat | 0.89 | 0.78 | 0.83 |

✅ **Overall Weighted Avg F1-Score:** ~0.89



## 💡 Example Predictions and Auto-Replies
| Comment | Predicted Category | Suggested Reply |
|----------|-------------------|-----------------|
| Amazing work! Loved the animation. | Praise | Thank you for your kind words! We appreciate your support. |
| This is trash, quit now. | Emotional | We’re glad our content connected with you emotionally. |
| The video was good, but the sound was poor. | Praise | Thank you for your kind words! We appreciate your support. |
| Can you make one on topic X? | Praise | Thank you for your kind words! We appreciate your support. |


## ⚙️ Real-Time Comment Classifier
The project includes a **real-time classification tool**, allowing users to input comments dynamically and instantly receive predictions and replies.

### Example:
