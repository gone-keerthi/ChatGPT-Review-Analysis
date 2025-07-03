# 📊 ChatGPT Review Sentiment Analysis

This project performs **sentiment analysis and feature extraction** on customer reviews of ChatGPT. It uses Python, NLP techniques, and data visualization to uncover what users love, criticize, or feel neutral about. This end-to-end analysis helps showcase practical skills in data cleaning, natural language processing, and storytelling with data—ideal for showcasing in a data analyst portfolio or resume.

## 🧠 Objectives
- Analyze overall **user sentiment**: Positive, Neutral, or Negative.
- Understand the **subjectivity** of reviews (emotional vs factual).
- Link **star ratings** with emotional tone.
- Extract and visualize commonly praised features.

## 📁 Dataset
- 📄 Source: [ChatGPT Reviews CSV](https://statso.io/wp-content/uploads/2024/08/chatgpt_reviews.csv)
- 📌 196,727 reviews with text, rating (1 to 5 stars), and timestamps.

## 🔧 Tools & Technologies
- Python
- pandas, numpy
- seaborn, matplotlib
- TextBlob (sentiment analysis)
- WordCloud
- Jupyter Notebook
- Google Colab (for runtime)
- 
## 📊 Project Workflow
### 📌 1. Data Preparation
- Load and inspect dataset
- Clean missing values
- Standardize column names
- Convert review dates to datetime
- Ensure correct data types

### 📌 2. Sentiment Analysis
- Apply `TextBlob` to calculate:
  - **Polarity** (from -1 to +1)
  - **Subjectivity** (from 0 to 1)
- Categorize into:
  - Positive (polarity > 0.1)
  - Neutral (between -0.1 and 0.1)
  - Negative (polarity < -0.1)

### 📌 3. Visualization
- **Bar Plot** for sentiment distribution  
- **Histogram + KDE** for subjectivity  
- **Heatmap** of sentiment vs. ratings  

### 📌 4. Keyword Extraction
- Focused on **positive reviews**
- Cleaned text and generated a **Word Cloud**
- Keywords: `love`, `helpful`, `useful`, `student`, `good`, `accurate`
- 
## 📈 Key Insights
| Metric              | Insight                                      |
|---------------------|----------------------------------------------|
| Total Reviews       | ~196,000                                     |
| Positive Sentiment  | ~74% of users were satisfied                 |
| Negative Sentiment  | ~3% only                                     |
| Subjectivity Peaks  | At 0.0, 0.6, and 1.0 – objective to emotional|
| Rating-Sentiment    | 5-star ratings strongly aligned with positivity |

## 🚀 How to Run
1. Clone the repo:
```bash
git clone https://github.com/your-username/chatgpt-review-analysis.git
