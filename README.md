# Analyzing the Negative Effects of Social Media on Gen-Z via YouTube NLP

**Tools Used:** Python, Google Colab, YouTube API, TextBlob, VADER Sentiment Analysis, NLTK (Tokenization)

## Executive Summary
This project analyzes the negative impact of social media on Generation Z by examining YouTube comments. Utilizing the YouTube API, TextBlob, and VADER, we processed 1,621 comments. Findings reveal keywords like sad, fake, and depression dominate the results. This aims to encourage positive social media usage[cite: 2].

## ⚙️ Data Collection & NLP Pipeline
To understand universal social media issues beyond geographic-specific limitations, this project utilized a custom natural language processing pipeline:

*   **Data Scraping:** Extracted over 10,000 comments and metadata from YouTube videos (2014-2023) across categories like GenZ's Opinions, TED Talks, Short Films, and Research[cite: 2].
*   **Sentiment Filtering:** Applied the TextBlob Python library to isolate comments with negative sentiment scores (polarity < 0) containing more than 20 words[cite: 2].
*   **Sentiment Scoring:** Utilized VADER to perform a complete scan of each sentence, assigning numerical polarity scores from -1 to 1 to calculate average sentiments by video type[cite: 2].
*   **Tokenization & N-grams:** Deployed the Natural Language Toolkit (NLTK) to split comment texts into tokens, specifically extracting bigrams (e.g., "anti social") to preserve context that unigrams might miss[cite: 2].

## 📊 Key Findings & Visualizations
Following the data cleaning process, the dataset was refined to 1,621 highly negative comments with a mean sentiment score of -0.23[cite: 2]. 

*   **Primary Keywords:** Across both general and Gen-Z specific video types, "sad" possessed the highest frequency, approaching 100 mentions, followed closely by "fake" and "depression"[cite: 2].
*   **Contextual Bigrams:** Bigram analysis revealed "i hate", "the worst", and "anti social" as leading phrases, confirming that users were reflecting negative sentiments and supporting movements to stop using social media[cite: 2].
*   **Category Nuances:** When filtering by the "Research" video type, "destroying" and "stupid" emerged as highly common negative keywords[cite: 2].

---
*For the complete methodology, histograms, and sentiment distribution plots, please view the [Full SOSC 314 Project Document](link-to-your-uploaded-file).*
