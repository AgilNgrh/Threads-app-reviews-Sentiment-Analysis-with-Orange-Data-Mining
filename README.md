# Threads-app-reviews-Sentiment-Analysis-with-Orange-Data-Mining
# 📊 Sentiment Analysis on Meta's Threads App Reviews

A comprehensive sentiment analysis project examining user perceptions of Meta's Threads application through the analysis of 32,910 user reviews collected from Google Play Store and App Store platforms.

---

## 📌 Project Overview

Meta launched Threads, a Twitter-like social media platform, in July 2023 as part of the Instagram ecosystem. This research investigates public sentiment toward Threads using advanced Natural Language Processing (NLP) techniques to analyze user reviews. The application saw rapid adoption, reaching 100 million users within the first week.

The goal of this study is to:
- Understand user experiences and satisfaction levels.
- Explore how new platforms are received in competitive social media landscapes.
- Derive insights to guide product improvement and positioning.

---

## 📂 Dataset Information

- Dataset Name: Threads, an Instagram app Reviews  
- Source: [Kaggle Dataset](https://www.kaggle.com/datasets)
- Total Reviews: 32,910  
- Platforms: Google Play Store and App Store  
- File Format: CSV  

### Key Features:
- Review Source (Google Play / App Store)
- Review Text (User Feedback)
- Rating (1 to 5 stars)
- Timestamp (For temporal analysis)

---

## 🛠 Methodology

### 🔄 Data Preprocessing Pipeline

1. Text Transformation
   - Lowercasing
   - Removal of accents, HTML tags, URLs

2. Tokenization
   - Whitespace-based token splitting

3. Normalization
   - Snowball Stemmer applied to reduce words to root forms

4. Content Filtering
   - Stopword removal
   - Lexicon-based filtering (sentiment-bearing words)
   - Removal of numbers and special patterns using regex

---

### 📈 Sentiment Analysis Techniques

1. Liu Hu Lexicon Method
   - Uses a curated dictionary with pre-labeled positive/negative words
   - Simple, interpretable, suitable as a baseline method

2. VADER (Valence Aware Dictionary and sEntiment Reasoner)
   - Tailored for social media content
   - Detects emotional intensity, capitalization, punctuation, and emojis
   - Ideal for informal, user-generated reviews

---

## 🔍 Key Findings

### 📊 Sentiment Distribution
| Method      | Positive (%) | Negative (%) |
|-------------|--------------|---------------|
| Liu Hu      | 41.61%       | 15.70%        |
| VADER       | 51.61%       | 16.83%        |

- VADER captured more positive expressions, reflecting its optimization for digital informality.
- Negative sentiment detection showed high consistency across both methods.

### ☁️ Word Cloud Insights
- Frequently appearing words: "app", "twitter", "good", "like", "thread"
- Indicates comparison with Twitter is common and influences user expectations.

### 🧠 User Perception Patterns
- Overall sentiment is predominantly positive.
- Users evaluate Threads relative to existing platforms, notably Twitter.
- Highlights both challenges and opportunities for differentiation.

---

## ⚙️ Technical Implementation

- Tools: [Orange Data Mining Software](https://orangedatamining.com/)
- Workflow:
  - Data import
  - Preprocessing
  - Sentiment classification
  - Visualization

Orange enables visual programming with modular, reproducible workflows ideal for text mining tasks.

---

## 🧠 Insights and Implications

### 📌 Business Intelligence
- Positive reception suggests high adoption potential.
- Frequent Twitter comparisons offer areas for competitive feature development.

### 🎓 Academic Contributions
- Demonstrates the benefit of combining traditional lexicon-based and modern social media-optimized sentiment methods.
- Offers methodology comparison as a guide for future NLP research.

---

## 🔭 Future Research Directions

- 📅 Temporal Analysis: Utilize timestamps for longitudinal sentiment trends.
- 🔗 Cross-Platform Studies: Explore Instagram-Threads integration effects on user sentiment.
- 🧠 Deep Learning Expansion: Use cleaned dataset with models like transformers (BERT, RoBERTa) for nuanced emotion detection.

---
