# Data-Mining-on-Amazon-Product-Reviews

## 📂 Dataset  
Amazon Review Polarity Dataset  
Contains 34,686,770 Amazon reviews from 6,643,669 users on 2,441,053 products.  
Used for **Sentiment Classification** and **Data Mining (Characterization & Discrimination)** tasks.  

---

## 🧐 Approach  

---

## Phase 1: **Data Preprocessing**
- Handle missing values (if any).  
- Remove special characters, HTML tags, and URLs.  
- Normalize text (convert to lowercase, remove stop words, punctuation, and perform stemming/lemmatization).  
- Extract product-related information using **Named Entity Recognition (NER)**.  

---

## Phase 2: **Classification (Neutral, Positive, Negative)**
- Fine-tune **BERT**, **RoBERTa**, or **XLNet** for **3-class sentiment classification**.  
- Classify reviews into:  
    - Negative (1)  
    - Neutral (0)  
    - Positive (2)  

---

## Phase 3: **Data Mining (Characterization & Discrimination)**  

### ✅ Step 1: Sentiment Intensity Mapping  
- Use **VADER** or **TextBlob** for basic scoring.  
- Map sentiment intensity to a scale:  
    - Highly Negative (-2)  
    - Negative (-1)  
    - Neutral (0)  
    - Positive (+1)  
    - Highly Positive (+2)  

---

### ✅ Step 2: Interclass Comparison  
- Compare sentiment trends across **different product categories**.  
- Statistical analysis (**ANOVA**, **Chi-Square**, **T-test**) to find **discrimination patterns** between positive and negative reviews.  

---

### ✅ Step 3: Semantic Pattern Analysis  
- **Topic Modeling (LDA or BERTopic)** to find hidden themes.  
- **Word Embedding (Word2Vec, GloVe, or BERT)** to understand customer behavior patterns.  

---

### ✅ Step 4: Keyword Frequency Distribution  
- Extract keywords using **TF-IDF**.  
- Visualize **frequent positive and negative terms** using **word clouds and bar charts**.  

---

## Phase 4: **Business Insights Extraction**  
- **Aspect-Based Sentiment Analysis (ABSA)** for customer pain point detection.  
- Predict **Product Success** using **XGBoost**, **Random Forest**, or **LightGBM**.  
- Identify product features that drive positive/negative customer experiences.  

---

## ✅ **Final Workflow Diagram**  

```
Raw Dataset
↓
Data Preprocessing
↓
Sentiment Classification (BERT/RoBERTa)
↓
Data Mining (Characterization & Discrimination)
↓
Business Insights Extraction

```

## 🎯 Expected Output  

| **Module**                  | **Output**                                      |
|--------------------|----------------------------------|
| Data Preprocessing      | Cleaned and structured dataset with product and review info |
| Classification             | Neutral, Positive, Negative |
| Sentiment Mapping      | Sentiment intensity score for each review |
| Interclass Comparison | Difference in sentiment trends across products |
| Semantic Patterns         | Hidden themes and customer behavior patterns |
| Keyword Distribution       | Top positive and negative keywords |
| Business Insights              | Product success prediction, pain point identification |

---

## 📈 Business Impact  

| Business Goal                | How Our Model Helps |
|----------------|----------------------------|
| Improve Product Quality       | Identify customer pain points |
| Enhance Customer Satisfaction | Detect positive product features |
| Predict Product Performance | Analyze sentiment trends |
| Market Analysis                | Track competitor product reviews |

---

## 🔧 Tech Stack  
- Python  
- SpaCy / NLTK  
- TensorFlow / PyTorch  
- Hugging Face Transformers  
- Sklearn  
- XGBoost / LightGBM  

---

## 🚀 Future Scope  
- Build a **real-time Sentiment Analysis Dashboard**  
- Integrate with **E-commerce platforms** for live product review monitoring  
- Develop a **Product Recommendation System**  
