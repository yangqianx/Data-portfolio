# Reddit NLP Analysis: Weight Loss Discussions During the Pandemic

## 1.Project Overview

This project explores how weight loss discussions and sentiments evolved on Reddit during the COVID-19 pandemic. It focuses on posts from the subreddit [r/loseit](https://www.reddit.com/r/loseit), analyzing 35,000+ submissions from March 2019 to March 2021.

Using topic modeling (LDA) and sentiment analysis (VADER and NRC-EIL), this project reveals:

- **5 main topic categories**: Weight Management, Diet, Physical Exercise, Emotions & Support, and Appearance.
- **16 topics** were detected, with notable changes over time in motivation, calorie tracking, and weight change discussions.
- **Sentiment dynamics**: Predominantly positive sentiment overall, but a slight increase in negative emotions was observed during the pandemic period.
- **Emotion analysis**: Common emotions expressed included *anticipation* and *fear*, with variation across topics.

---

## 2.Key Results

![Monthly Post Count](images/Number%20of%20the%20posts%20posted%20per%20month%20from%20March%202019%20to%20March%202021.png)

I tracked and visualized monthly trends in the submissions posted. There was a significant increase in the number of posts in the loseit subreddit starting from March 2020, about 2 months after WHO officially declared the pandemic. This increase continued until August 2020, after that, it returned to more typical levels.

![Monthly Topic Proportion of topics in the Themes (a)](images/Monthly%20posts%20proportion%20of%20topics%20in%20the%20Themes%20%28a%29.png)

![Monthly posts proportion of topics in the Themes (b)](images/Monthly%20posts%20proportion%20of%20topics%20in%20the%20Themes%20%28b%29.png)

16 topics were generated from the LDA model in the loseit subreddit. These topics have been manually named into Clothe fit (T0), Daily updates (T1), Weight change (T2), Calorie tracker (T3), Motivation (T4), Fitness App (T5), Exercise routine (T6), Body image (T7), Seeking advice (T8), Medication (T9), Emotional eating (T10), Weight loss goal (T11), Food choice (T12), Negative feeelings (T13), Diet control (T14) and Workout plan (T15).

I found several topics change significantly throughout the study period in the loseit subreddit. In the Weight Management theme (Figure 11), there was an increased focus on Weight
change (T2) starting at the end of 2019 and continuing untill the pandemic outbreak. In the Diet theme (Figure 12), Calorie tracker (T3) showed a significant increase over time, especially in the months following the outbreak. Emotional eating (T10) fluctuated slightly, with a small increase during the early month of the outbreak. In the Physical Exercise theme (Figure 13), both Motivation (T4) and Workout Plan (T15) showed some fluctuations with increasing trends during the outbreak and then stayed stable. In the Emotions and Support theme (Figure 14), Negative feelings (T13) showed a clear fluctuation and declining trend over time. In the Appearance theme (Figure 15), Body image (T7) increased while Clothe fit (T0) declined before the outbreak, and then both topics maintained relatively stable trends during the pandemic. Other topics, such as Weight loss goal (T11), Medication (T9), Daily updates (T1), Food choice (T12) and Diet control (T14), Fitness App (T5), Exercise routine (T6) and Seeking acvice (T8) remained relatively stable and slight fluctuations over time.

![Number of posts of sentiments (positive, negative, netural) trends over time](images/Number%20of%20posts%20of%20sentiments%20%28positive%2C%20negative%2C%20netural%29%20trends%20over%20time.png)

I visualized how sentiment evolved from March 2019 to March 2021 by VADER. However, from March 2020 to May 2020, during the early time of the pandemic outbreak, we saw increasing trends in both positive and negative posts about weight loss. Moreover, May 2020 was marked as a distinct peak during the pandemic. It was sustained through August before declining again. This suggests that the users discussed more weight loss-related topics during this period. Notably, two notable peaks were also observed in January 2020 and January 2021, which reflects a seasonal pattern of increased activity. This could potentially relate to the New Year resolutions, that people might be more motivated to set weight loss goals at the beginning of the year. Additionally, in this subreddit, neutral posts remained stable, with only slight changes over time.

![Proportions of sentiments polarity (positive, negative, netual) by topics across two time periods](images/Proportions%20of%20sentiments%20polarity%20%28positive%2C%20negative%2C%20netual%29%20by%20topics%20across%20two%20time%20periods.png)

After analyzing the overall sentiment polarity trends, I also examined the sentiment proportions at the topic level to explore how positive, negative, and neutral sentiments shifted in specific topics over time. I observed several significant sentiment changes in topics during the pandemic. In the Weight Management theme (T2, T11, T9, T1), positive posts in Daily updates (T1) increased (+5.42%), while negative posts decreased during the pandemic (-4.93%). In the Diet theme (T10, T12, T3, T14), posts about Emotional eating (T10) saw an increase in positive sentiment (+2.28%) with a decrease in negative sentiment during the pandemic (-2.04%). Furthermore, positive posts in Diet control (T14) also saw an increase (+4.30%), while negative posts decreased (-4.55%). In the Physical Exercise theme (T4, T15, T5, T6), positive posts (-2.70%) in Fitness App (T4) also decreased while negative posts increased (-3.99%). Conversely, positive posts (+3.99%) in Motivation (T4) also rose while negative posts decreased (-3.63%). In the Emotions and Support theme (T13, T8), positive posts in Negative feelings (T13) decreased slightly (-3.00%) while negative sentiments increased (+2.47%). Moreover, positive posts in Seeking advice (T8) decreased (-3.11%) during the pandemic, with an increase in negative posts (+2.90%). Additionally, in the Appearance theme (T7, T0), positive posts in Clothe fit (T0) declined slightly (-2.65%), and negative posts saw a corresponding increase (+3.56%) during the pandemic.

![Proportion of words associated with eight emotions by topics before the pandemic](images/Proportion%20of%20words%20associated%20with%20eight%20emotions%20by%20topics%20before%20the%20pandemic.png)

![Proportion of words associated with eight emotions by topics before the pandemic](images/Proportion%20of%20words%20associated%20with%20eight%20emotions%20by%20topics%20during%20the%20pandemic.png)

In the Weight management theme (T2, T11, T9, T1), the emotional changes in Daily updates (T1) were the most significant. Among them, positive words such as joy (+2.96%) and trust (+2.33%) increased significantly in the post, while negative words such as fear (-1.09%), sadness (-2.16%) and anger (-1.82%) decreased significantly in the post. Positive and negative words in Weight change (T2), Weight loss goal (T11), and Medication (T9) changed slightly, and the overall change was not noticeable.  

In the Diet theme (T10, T12, T3, T14), positive and negative words in the four topics, Emotional eating (T10), Food choice (T12), Calorie tracker (T3), and Diet control (T14) changed slightly, and the overall emotion was relatively stable. In the Physical Exercise theme (T4, T15, T5, T6), positive words in Motivation (T4) decreased, such as joy (-1.14%) and trust (-0.61%), decreased in the posts. Positive words in Workout plan (T15) decreased with joy words decreased significantly. Negative words changed slightly in the above topics. In addition, positive and negative words in Fitness App (T5) and Exercise routine (T6) were relatively balanced in the post, and the change was not significant.  

In the Emotions and Support theme (T13, T8), the emotional expression of Negative feelings (T13) decreased slightly, with positive words decreasing slightly. Negative emotional words in this topic also changed slightly, fear (+0.41%) and sadness (+0.29%) increased slightly. The emotions in Seeking advice (T8) changed slightly, and the overall emotional expression in this topic was relatively stable.  

In the Appearance theme (T7, T0), positive words in both topics decreased slightly, while negative words increased slightly.Positive words such as trust (-0.20%) in Body image (T7) decreased slightly. Negative words remained stable, with a slight increase, but the change was little. Positive words in Clothe fit (T0) also decreased with the joy (-0.18%) and trust (-0.29%) words decreased. Negative words increased slightly but there was little change.  

---

## 3.Tools & Technologies

**Languages & Libraries:**

- Python (Pandas, NumPy, Scikit-learn, NLTK, SpaCy, Gensim)
- Topic Modeling: Latent Dirichlet Allocation (LDA)
- Sentiment Analysis: VADER, NRC Emotion Lexicon
- Data Visualization: Matplotlib, Seaborn, Plotly

**Other Tools:**
- Reddit API (PRAW)
- Data compression handling (`zstandard`)

---

## 4.Data Structure

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
