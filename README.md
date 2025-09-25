# Geo-semantic-analysis

Service Quality of Hospitals in Nigeria: Geo-Semantic Analysis of Citizens' Social Media Posts

Author: Morolari Boluwatife
Organization: Data Science Nigeria, Lagos, Nigeria
Email: morolaribolu@gmail.com

Overview

This project investigates the service quality of hospitals in Nigeria by analyzing citizens’ opinions expressed on social media platforms, primarily Twitter. The study combines geo-semantic analysis, natural language processing (NLP), and sentiment analysis to assess public perception of healthcare services, highlight critical service gaps, and provide actionable insights for policymakers and healthcare providers.

Social media provides a valuable platform for citizens to voice their healthcare experiences. Using geo-tagged posts and topic modeling, this study profiles hospital performance across different regions in Nigeria.

Objectives

To assess citizen sentiment towards hospital services in Nigeria.

To identify key factors affecting hospital service quality (e.g., infrastructure, waiting times, staff behavior).

To map geographical variations in hospital service perception across Nigeria.

To provide insights for healthcare policy and hospital management improvements.

Methods
Data Collection

Platform: Twitter (most widely used for healthcare opinions in Nigeria).

Tool: Twint
 Python scraper (no API required).

Keywords: Names of hospitals across Nigeria.

Collected Data: Tweet ID, timestamp, content, author handle, etc.

Data Preprocessing

Removal of irrelevant tweets (less than 3 words, unrelated mentions).

Cleaning: hyperlinks, hashtags, usernames, emojis, numbers, and punctuation removed.

Tokenization & Lemmatization: Using NLTK library.

Stop-word Removal to retain meaningful words.

Final dataset: ~250 curated tweets.

Data Analysis

Topic Modeling

Short Text Topic Modeling (STTM) using Gibbs Sampling Dirichlet Mixture Model (GSDMM).

Identified hospital-related topics like:

Infrastructure & Facilities

Staff Behavior & Professionalism

Waiting Times & Appointment Management

Accessibility & Availability

Overall Patient Experience

Sentiment Analysis

Conducted with TextBlob to determine positive, negative, or neutral sentiment.

Sentiment polarity range: -1 (negative) to 1 (positive).

Geo-Semantic Analysis

Geocoding: Used OpenCage API to convert hospital names to latitude/longitude.

Mapped sentiment distribution across regions to identify areas of high dissatisfaction.

Key Findings

Sentiment Distribution:

~80% negative posts

~10% positive posts

Remaining neutral

Common Keywords in Negative Posts:

“Poor service delivery”

“Inadequate facilities”

“Long waiting times”

“Lack of equipment”

Geographical Insights:

Major cities (Lagos, Abuja, Oyo) had the highest concentration of negative sentiment.

Lagos Island Maternity Hospital showed significant negative feedback related to staff and equipment.

Implications:

Highlights urgent need for improvements in infrastructure, staffing, funding, and hospital accessibility.

Suggests hospitals should maintain an active social media presence for better communication and service feedback.

Conclusion

This study demonstrates the power of geo-semantic analysis and social media data in evaluating hospital service quality. Despite limitations (e.g., small tweet sample, potential bias), the results provide actionable insights for healthcare providers and policymakers aiming to improve service delivery in Nigeria.

References

Greaves F, Laverty AA, Cano DR, et al. Tweets about hospital quality: a mixed methods study. BMJ Quality & Safety 2014;23:838-846.

Hawkins JB, Brownstein JS, Tuli G, et al. Measuring patient-perceived quality of care in US hospitals using Twitter. BMJ Quality & Safety 2016;25:404-413.

Greaves F, Ramirez-Cano D, et al. Use of sentiment analysis for capturing patient experience from free-text comments posted online. J Med Internet Res. 2013;15(11):e239.

Nghiem, Son & Mehta, Pratik & Tao, Liang. (2013). Twitter for Public Health: An Open-source Data Solution.

Huang JH, Floyd MF, et al. Exploring public values through Twitter data associated with urban parks pre- and post-COVID-19. Landsc Urban Plan. 2022;227:104517.
