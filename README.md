# Data-Mining-on-Amazon-Product-Reviews

## 📂 Dataset
Amazon Review Polarity Dataset  
Contains 34,686,770 Amazon reviews from 6,643,669 users on 2,441,053 products.  
Used for sentiment analysis and text classification tasks.  

---

## 🧐 Approach  

### 📌 Phase 1: Data Preprocessing
**Step 1: Data Cleaning**  
- Handle missing values (if any).  
- Remove special characters, HTML tags, and URLs.  
- Normalize text (convert to lowercase, remove stop words, punctuation, and perform stemming/lemmatization).  

**Step 2: Text Parsing & Product Extraction**  
- Extract product names and categories using **Named Entity Recognition (NER)** with **SpaCy** or **BERT-based NER models**.  
- Store the product, review title, and review text in a structured format.  

---

### 📌 Phase 2: Sentiment Intensity Mapping
**Step 3: Sentiment Scoring**  
- Use **VADER** or **TextBlob** for basic sentiment scoring.  
- Fine-tune **DistilBERT**, **RoBERTa**, or **XLNet** for more accurate sentiment analysis.  
- Map sentiment intensity to a scale:  
    - Highly Negative (-2)  
    - Negative (-1)  
    - Neutral (0)  
    - Positive (+1)  
    - Highly Positive (+2)  

---

### 📌 Phase 3: Interclass Comparison
**Step 4: Interclass Analysis**  
- Compare sentiment distribution across different product categories.  
- Use statistical measures like **ANOVA**, **Chi-Square**, or **T-test** to identify significant differences between positive and negative reviews.  

---

### 📌 Phase 4: Semantic Pattern Analysis
**Step 5: Topic Modeling**  
- Use **Latent Dirichlet Allocation (LDA)** or **BERTopic** to identify hidden topics and patterns in reviews.  
- Visualize patterns using **t-SNE** or **UMAP clustering**.  

**Step 6: Word Embedding**  
- Use **Word2Vec**, **GloVe**, or **BERT embeddings** to capture the semantic meaning of reviews.  
- Cluster similar reviews and detect trends in customer feedback.  

---

### 📌 Phase 5: Keyword Frequency Distribution
**Step 7: Keyword Extraction**  
- Use **TF-IDF** to identify important keywords for positive and negative reviews.  
- Visualize using **word clouds** and **bar charts**.  

---

### 📌 Phase 6: Classification (Neutral, Positive, Negative)
**Step 8: Sentiment Classification**  
- Fine-tune **BERT**, **RoBERTa**, or **XLNet** for **3-class classification (Neutral, Positive, Negative)**.  
- Train the model on a balanced subset of the dataset.  

---

### 📌 Phase 7: Business Insights Extraction
**Step 9: Product and Feature Extraction**  
- Extract product-related information (e.g., product names, features, and brand names).  
- Perform **Aspect-Based Sentiment Analysis (ABSA)** to understand customer pain points and satisfaction factors.  

**Step 10: Predict Product Success**  
- Use **XGBoost**, **Random Forest**, or **LightGBM** to predict product success based on sentiment trends.  
- Identify which product features drive positive or negative customer experiences.  

---

## ✅ Expected Output  

| **Module**                  | **Output**                                      |
|--------------------|----------------------------------|
| Data Preprocessing      | Cleaned and structured dataset with product and review info |
| Sentiment Mapping      | Sentiment intensity score for each review |
| Interclass Comparison | Difference in sentiment trends across products |
| Semantic Patterns         | Hidden themes and customer behavior patterns |
| Keyword Distribution       | Top positive and negative keywords |
| Classification                  | Neutral, Positive, Negative |
| Business Insights              | Product success prediction, pain point identification |

---

## 📈 Business Impact  
- Analyzing customer sentiment towards specific products.  
- Identifying customer pain points and satisfaction drivers.  
- Predicting product performance and customer satisfaction trends.  
- Enhancing decision-making for product improvement and marketing strategies.  

---

## 🔧 Tech Stack  
- Python  
- SpaCy  
- NLTK  
- TensorFlow / PyTorch  
- Hugging Face Transformers  
- Sklearn  
- XGBoost / LightGBM  

---

## 🚀 Future Scope  
- Build a real-time sentiment analysis dashboard.  
- Integrate with e-commerce platforms for live product reviews monitoring.  
- Develop a recommendation system based on customer feedback.  

---

