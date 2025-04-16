# Reddit NLP Analysis: Weight Loss Discussions During the Pandemic

## Project Overview

This project explores how weight loss discussions and sentiments evolved on Reddit during the COVID-19 pandemic. It focuses on posts from the subreddit [r/loseit](https://www.reddit.com/r/loseit), analyzing 35,000+ submissions from March 2019 to March 2021.

Using topic modeling (LDA) and sentiment analysis (VADER and NRC-EIL), this project reveals:

- **5 main topic categories**: Weight Management, Diet, Physical Exercise, Emotions & Support, and Appearance.
- **16 topics** were detected, with notable changes over time in motivation, calorie tracking, and weight change discussions.
- **Sentiment dynamics**: Predominantly positive sentiment overall, but a slight increase in negative emotions was observed during the pandemic period.
- **Emotion analysis**: Common emotions expressed included *anticipation* and *fear*, with variation across topics.

---

## Key Results

![Monthly Post Count](images/Number%20of%20the%20posts%20posted%20per%20month%20from%20March%202019%20to%20March%202021.png)

![Sentiment Trend](images/sentiment_trend.png)

- **Topic Timeline:** Motivation-related discussions peaked mid-2020.
- **Sentiment Distribution:** Positive sentiment dominates, but negative sentiment grew slightly post-pandemic outbreak.
- **Emotion Breakdown:** Anticipation was the most frequent emotion, followed by fear and joy.
---

## Tools & Technologies

**Languages & Libraries:**

- Python (Pandas, NumPy, Scikit-learn, NLTK, SpaCy, Gensim)
- Topic Modeling: Latent Dirichlet Allocation (LDA)
- Sentiment Analysis: VADER, NRC Emotion Lexicon
- Data Visualization: Matplotlib, Seaborn, Plotly

**Other Tools:**
- Reddit API (PRAW)
- Data compression handling (`zstandard`)

---

## Data Structure

| File | Description |
|------|-------------|
| `loseit_submissions.zst` | Historical Reddit post data |
| `submissions.csv` | Raw content and metadata |
| `cleaned_submissions.csv` | Preprocessed dataset |
| `processed_lda.csv` | Cleaned data prepared for LDA |
| `processed_vader.csv` | Cleaned data for VADER sentiment |
| `processed_nrc.csv` | Cleaned data for NRC emotion analysis |
| `lda_submissions.csv` | Topic results |
| `vader_submissions.csv` | VADER sentiment results |
| `nrc_submissions.csv` | NRC emotion results |
