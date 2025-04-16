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

![Monthly Topic Proportion of topics in the Themes (a)](images/Monthly%20posts%20proportion%20of%20topics%20in%20the%20Themes%20%28a%29.png)

![Monthly posts proportion of topics in the Themes (b)](images/Monthly%20posts%20proportion%20of%20topics%20in%20the%20Themes%20%28b%29.png)

![Number of posts of sentiments (positive, negative, netural) trends over time](images/Number%20of%20posts%20of%20sentiments%20%28positive%2C%20negative%2C%20netural%29%20trends%20over%20time.png)

![Proportions of sentiments polarity (positive, negative, netual) by topics across two time periods](images/Proportions%20of%20sentiments%20polarity%20%28positive%2C%20negative%2C%20netual%29%20by%20topics%20across%20two%20time%20periods.png)

![Proportion of words associated with eight emotions by topics before the pandemic](images/Proportion%20of%20words%20associated%20with%20eight%20emotions%20by%20topics%20before%20the%20pandemic.png)

![Proportion of words associated with eight emotions by topics before the pandemic](images/Proportion%20of%20words%20associated%20with%20eight%20emotions%20by%20topics%20during%20the%20pandemic.png)

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
