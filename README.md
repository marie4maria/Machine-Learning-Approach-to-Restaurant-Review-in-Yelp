# 🍕 Tucson Pizza Review Analyzer 🍕

## Overview
Welcome to the **Tucson Pizza Review Analyzer**! 🍕 This data science project dives deep into Yelp reviews of Tucson-based pizza restaurants to extract valuable insights on customer sentiment, restaurant performance, and key pizza-related aspects like taste, crust, cheese, and service. But that's not all! I've also built a recommendation model that suggests the **top 3 pizza restaurants** to customers based on specific keywords they provide. 🍽️✨

By combining **Exploratory Data Analysis (EDA)**, **Aspect-Based Sentiment Analysis** using **BERT**, and **Automated Summary Generation** via **Claude** (Amazon Bedrock), this project aims to offer both restaurant owners and customers actionable insights on restaurant performance.

_"Pizza is not just food, it's an experience!"_ 🍕

## Pipeline and Approach

### 🔍 Exploratory Data Analysis (EDA)
- Cleaned and preprocessed raw review text to identify key aspects, and visualized dominant keywords like **"crust," "cheese," and "service"** through **WordClouds**. 🌬️🧀🍞
- Analyzed sentiment distribution and star ratings, uncovering a **bimodal distribution** (with many 1-star and 5-star reviews). ⭐️⭐️⭐️⭐️⭐️
- Calculated key statistics on review interactions, average ratings, and review trends over time. 📊

### 🤖 Aspect-Based Sentiment Analysis with BERT
- Leveraged the **BERT model** (`nlptown/bert-base-multilingual-uncased-sentiment`) to perform **aspect-based sentiment analysis** across **10 pizza-related aspects** (e.g., taste, crust, sauce, hygiene). 🍅🧀
- Converted **1–5 star ratings** into a sentiment score scale (0–10) for more precise aspect-based analysis. 📈
- Produced easy-to-interpret charts showing **average ratings** for each aspect and **classification heatmaps** of sentiment across the top 10 businesses. 📊💡

### 📝 Summary Generation with Claude (Amazon Bedrock)
- Used **Claude** from Amazon Bedrock to generate **concise summaries** for each restaurant based on the sentiment analysis results.
- Summaries highlighted the restaurant’s **overall impression**, **strengths**, **areas for improvement**, **value assessment**, and the **best use case** for each restaurant. 🗣️

### 🤖 **Restaurant Recommendation Model** 
- Created a **LoRA-based model** to **recommend the top 3 pizza restaurants** based on **keywords** provided by customers (e.g., "best crust," "quick delivery," "family-friendly").
- The model matches the customer's preferred pizza aspects with reviews to suggest restaurants that best meet their criteria. 🍽️💡

## Key Outputs
- `sentiment_analysis_results.csv`: Contains review scores and sentiments for each aspect. 📅
- `pizza_restaurant_summaries.txt`: Generated summaries for each restaurant based on sentiment analysis results. 📝
- `styled_table_big.png`: A visually formatted table for easy presentation of results. 📸
- `restaurant_recommendations.txt`: A file with the top 3 pizza restaurant recommendations based on user-input keywords. 🍕

## Insights & Impact
- **Uncovered key insights** on which Tucson pizza restaurants excel in specific aspects, such as **crust**, **cheese**, or **ambiance**. 🌟
- **Identified potential areas** for improvement, such as **delivery speed** or **service quality**. ⏱️🍕
- Gave **customers valuable, easy-to-digest restaurant summaries**, helping them make informed dining decisions based on real customer feedback. 🤩
- The **recommendation system** takes customer preferences into account and makes personalized restaurant suggestions, improving the overall dining experience. 🍴

## Tools and Technologies
- **Python Libraries**: Pandas, Seaborn, Matplotlib, WordCloud, sklearn, nltk, NumPy, transformers, boto3 🐍📊
- **Sentiment Analysis**: BERT (`nlptown/bert-base-multilingual-uncased-sentiment`) 🧠
- **Summary Generation**: Amazon Bedrock (Claude) ☁️
- **Recommendation Model**: LoRA-based model for restaurant suggestions 🍴
- **Data Source**: Yelp Open Dataset (filtered for Tucson pizza restaurants) 🌍🍕

## Future Improvements
- **Integration with OpenAI (ChatGPT)** for deeper summary comparisons and additional personalization. 🤖
- Deployment as an **interactive Streamlit dashboard** for **real-time restaurant analysis** and recommendations. 📱💻
- Integration with **Yelp’s real-time API** for **dynamic reviews** and **restaurant updates**. 📲

## Collaborators
- **Sarah Le** 👩‍💻
- **Delna Sophia Dsouza** 👩‍💻
- **Mary John** 👩‍💻
- **Tsai-Yun Hsieh** 👨‍💻
