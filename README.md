# Geo-semantic-analysis

Service Quality of Hospitals in Nigeria: Geo-Semantic Analysis of Citizens' Social Media Posts

Author: Morolari Boluwatife
Organization: Data Science Nigeria, Lagos, Nigeria
Email: morolaribolu@gmail.com

📖 Overview

This project evaluates the service quality of hospitals in Nigeria by analyzing citizens’ opinions expressed on social media. Using Twitter data, combined with geo-semantic analysis, natural language processing (NLP), and sentiment analysis, this study provides insights into:

Public perception of hospital services

Geographic variations in hospital satisfaction

Key factors contributing to service quality issues

The results can inform policymakers, healthcare providers, and stakeholders to improve service delivery.

🎯 Objectives

Assess citizens' sentiment towards hospital services in Nigeria.

Identify critical factors affecting service quality (e.g., infrastructure, waiting times, staff professionalism).

Map geographical variations in hospital service perception.

Provide actionable insights for healthcare policy and hospital management.

🛠 Methods
1. Data Collection

Platform: Twitter

Tool: Twint
 (Python-based scraper, no API required)

Keywords: Names of hospitals across Nigeria

Data Collected: Tweet ID, timestamp, content, author handle

2. Data Preprocessing

Removed irrelevant tweets (e.g., <3 words, unrelated mentions)

Cleaned text (hyperlinks, hashtags, mentions, emojis, numbers, punctuation)

Tokenization & Lemmatization: Using NLTK

Removed stop words for meaningful analysis

Final Dataset: 250 curated tweets

3. Data Analysis
Topic Modeling

Used Short Text Topic Modeling (STTM) with GSDMM (Gibbs Sampling Dirichlet Mixture Model)

Identified key topics:

Infrastructure & Facilities

Staff Behavior & Professionalism

Waiting Times & Appointment Management

Accessibility & Availability

Overall Patient Experience

Sentiment Analysis

Library: TextBlob

Sentiment polarity: -1 (negative) to +1 (positive)

Geo-Semantic Analysis

Geocoding via OpenCage to convert hospital names to latitude/longitude

Mapped tweets to visualize geographic sentiment distribution

📊 Key Findings
Sentiment Analysis

Negative Sentiment: ~80% of tweets

Positive Sentiment: ~10% of tweets

Neutral: ~10%

Common Keywords (Negative Sentiment)

Poor service delivery

Inadequate facilities

Long waiting times

Lack of equipment

Geographic Insights

Major cities with highest negative sentiment: Lagos, Abuja, Oyo

Example: Lagos Island Maternity Hospital showed strong negative feedback related to staff and equipment

Implications

Urgent need to improve infrastructure, staffing, and hospital accessibility

Hospitals should maintain an active social media presence for better communication with citizens

💡 Conclusion

Geo-semantic analysis of social media posts provides valuable insights into public perception of hospital services.

Despite the dataset being limited, trends indicate widespread dissatisfaction with Nigerian hospitals.

Findings highlight areas requiring urgent attention and can guide policy reforms and healthcare improvements.
