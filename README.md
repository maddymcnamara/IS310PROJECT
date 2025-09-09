# Reddit Community Analysis: UIUC vs. Michigan  

This project applies **Natural Language Processing (NLP)** techniques to analyze and compare discussions from two university communities on Reddit: [r/UIUC](https://www.reddit.com/r/UIUC) and [r/UMich](https://www.reddit.com/r/umich). The goal was to explore the themes, language patterns, and community dynamics within these subreddits using word frequency analysis, classification models, and topic modeling.  

---

## Project Overview  
- **Data**: Reddit comments/posts from UIUC and Michigan subreddits (`uiuc.csv`, `michigan.csv`)  
- **Objective**: Identify key discussion patterns, compare communities, and build models to classify posts and uncover latent themes  

---

## Methods & Tools  
- **Preprocessing**  
  - Tokenization, lemmatization, lowercasing  
  - Stopword removal  
- **Exploratory Analysis**  
  - Word frequency plots  
  - Cross-community word usage comparison  
- **Modeling**  
  - Logistic Regression → Predict subreddit (71% accuracy after train/test split)  
  - LDA Topic Modeling → Extracted 10 themes across posts  
- **Libraries**: `pandas`, `scikit-learn`, `gensim`, `matplotlib`, `seaborn`, `nltk`  

---

## Results  

### Word Frequency Insights  
- Raw top words were dominated by stopwords (*“the,” “to,” “you”*)  
- After cleaning, more meaningful words appeared: *class, year, time, good, think*  
- Comparing the same words across UIUC and Michigan revealed **community-specific usage patterns** (e.g., “year” spiking in UIUC due to semester discussions)  

### Classification (Logistic Regression)  
- **Accuracy**: ~71% with train/test split  
- **Observation**: Accuracy dropped compared to testing on full data (inflated) → shows importance of proper model evaluation  

### Topic Modeling (LDA)  
Grouped 10 discovered topics into 3 overarching **themes**:  
1. **Campus Life & Challenges** (housing, weather, Greek life, transportation)  
2. **Resources & Information Sharing** (financial aid, health services, policies, local businesses)  
3. **Social & Emotional Experience** (friendships, classes, socializing, isolation, mental health)  

*Takeaway*: Reddit communities serve both **informational** and **emotional support** roles for students.  

   git clone https://github.com/yourusername/reddit-community-analysis.git
   cd reddit-community-analysis
