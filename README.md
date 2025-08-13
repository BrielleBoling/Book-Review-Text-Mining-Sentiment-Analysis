# Book-Review-Text-Mining-Sentiment-Analysis

This project applies text mining techniques to analyze **1,000 Amazon book reviews**, exploring patterns in sentiment, common vocabulary, and underlying discussion topics using topic modeling.

## Project Overview
This project includes **text preprocessing**, **word cloud visualization**, **sentiment analysis**, and **topic modeling** with Python.  

The dataset (`book_ratings.csv`) contains:
- **Id** – Unique ID for the book  
- **Title** – Book title  
- **Price** – Book price  
- **User_id** – Unique user ID  
- **profileName** – Reviewer name  
- **review/helpfulness** – Helpfulness score (0–1)  
- **review/score** – Book rating (0–5)  
- **review/time** – Review timestamp  
- **review/summary** – Short review summary  
- **review/text** – Full review text  

## Tools & Libraries
- `pandas` – Data handling
- `numpy` – Numerical operations
- `matplotlib` / `seaborn` – Visualizations
- `wordcloud` – Word cloud generation
- `nltk` / `spaCy` – Text preprocessing
- `scikit-learn` – Vectorization
- `gensim` – Topic modeling (LDA)
- `pyLDAvis` – Topic visualization

## Methodology
1. **Preprocessing**
   - Tokenization
   - Lowercasing
   - Stop word removal
   - Stemming
   - Additional cleaning steps for punctuation and special characters

2. **Word Cloud Visualization**
   - Generated for both `review/summary` and `review/text`
   - Showed dominant words like **"book"**, **"great"**, **"love"**, and **"time"**

3. **Sentiment Analysis**
   - Classified reviews as **positive**, **neutral**, or **negative**
   - Most reviews were **neutral**, with a noticeable number of mild-to-moderate positives and fewer negatives
   - Polarity distribution indicated a balance between emotional and objective reviews

4. **Topic Modeling (LDA)**
   - **6-topic model**: Captured diverse themes like book enjoyment, reading habits, preferences, emotional themes, classics, and historical/adventure genres
   - **4-topic model**: Used for `pyLDAvis` visualization of intertopic distances
   - Detailed interpretation provided for selected topics

## Results Summary
**Sentiment Insights:**
- Majority of reviews are **neutral**
- Positive reviews often express enjoyment, storytelling quality, and usefulness
- Negative reviews are rare but tend to focus on disappointment or unmet expectations

**Topic Modeling Highlights:**
- **Topic 1:** General enjoyment & storytelling  
- **Topic 2:** Reading habits & expectations  
- **Topic 3:** Book preferences & usefulness  
- **Topic 4:** Emotions & themes in literature  
- **Topic 5:** Classic literature & intellectual engagement  
- **Topic 6:** Reviews of historical/adventure genres  
