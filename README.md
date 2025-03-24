# 🍕 Tucson Pizza Review Analyzer 🍕

## Overview
This project analyzes Yelp reviews of Tucson-based pizza restaurants using advanced Natural Language Processing (NLP) techniques to gain insights into customer sentiment, restaurant performance, and popular pizza-related aspects like taste, crust, cheese, and service. The project integrates several components including Exploratory Data Analysis (EDA), Aspect-Based Sentiment Analysis using BERT, and automated summary generation via Claude (Amazon Bedrock).

_"Pizza is not just food, it's an experience!"_ 🍕

## Pipeline and Approach

### 🔍 Exploratory Data Analysis (EDA)
- Cleaned raw review text and visualized dominant keywords like "crust," "cheese," and "service" through WordClouds. 🌬️🧀🍞
- Analyzed sentiment distribution and star ratings, identifying a bimodal distribution (1-star and 5-star reviews). ⭐️⭐️⭐️⭐️⭐️
- Computed key statistics on review interactions and rating trends. 📊

### 🤖 Aspect-Based Sentiment Analysis with BERT
- Applied the `nlptown/bert-base-multilingual-uncased-sentiment` model to analyze sentiment for 10 pizza-related aspects (e.g., taste, crust, sauce, hygiene). 🍅🧀
- Converted 1–5 star ratings into a sentiment score scale (0–10) for each aspect. 📈
- Produced charts showing average ratings for each aspect and classification heatmaps of sentiment across 10 businesses. 📊💡

### 📝 Summary Generation with Claude (Amazon Bedrock)
- Used Claude to generate concise summaries for each restaurant based on aspect ratings.
- Summaries included the restaurant’s overall impression, strengths, areas for improvement, value assessment, and best use case. 🗣️

## Key Outputs
- `sentiment_analysis_results.csv`: Contains review scores and sentiments for each aspect. 📅
- `pizza_restaurant_summaries.txt`: Generated summaries for each restaurant based on sentiment analysis results. 📝
- `styled_table_big.png`: A formatted table visualizing the results for presentation. 📸

## Insights & Impact
- Revealed which Tucson pizza restaurants excel in aspects like crust, cheese, or ambiance. 🌟
- Identified potential areas for improvement in restaurants, such as delivery speed. ⏱️🍕
- Provided potential customers with valuable, easy-to-digest summaries of each restaurant based on real customer feedback. 🤩

## Tools and Technologies
- **Python Libraries**: Pandas, Seaborn, Matplotlib, WordCloud 🐍📊
- **Sentiment Analysis**: BERT (`nlptown/bert-base-multilingual-uncased-sentiment`) 🧠
- **Summary Generation**: Amazon Bedrock (Claude) ☁️
- **Data Source**: Yelp Open Dataset (filtered for Tucson pizza restaurants) 🌍🍕

## Future Improvements
- Integration with OpenAI (ChatGPT) for summary comparisons. 🤖
- Deployment as an interactive Streamlit dashboard for real-time analysis. 📱💻
- Integration with Yelp’s real-time API for dynamic reviews and restaurant updates. 📲

## Collaborators
- Sarah Le 👩‍💻
- Delna Sophia Dsouza 👩‍💻
- Mary John 👩‍💻
- Tsai-Yun Hsieh 👨‍💻

## Contact
Email: your-email@example.com ✉️
