# `British Airways Customer Reviews Sentiment Analysis: Insights from Skytrax`
### `Project Overview`

#### `1. Introduction`

British Airways (BA) is the flag carrier airline of the United Kingdom (UK). Every day, thousands of BA flights arrive to and depart from the UK, carrying customers across the world. Whether it’s for holidays, work or any other reason, the end-to-end process of scheduling, planning, boarding, fuelling, transporting, landing, and continuously running flights on time, efficiently and with top-class customer service is a huge task with many highly important responsibilities.

- **Objective:** The goal of this project is to analyze customer reviews of BA airline using data scraped from [Skytrax](https://www.airlinequality.com/), perform sentiment analysis, identify key factors affecting customer satisfaction, and present findings in a single page spread sheet.

- **Scope:** This project will involve data scraping, data cleaning, sentiment analysis, and presenting insights through visualizations and recommendations. For this project, we will be using python.

#### `2. Data Collection`
- **Source:** Skytrax website.
- **Method:** Python and libraries such as BeautifulSoup and Requests to scrape review data.
- **Data Collected:** Customer reviews, ratings for various aspects (e.g., cabin staff service, food and beverages), sentiment scores, and other relevant information.

#### `3. Data Cleaning and Preparation`
- **Handling Missing Values:** Deal with any missing or incomplete data and utilizing only verified customers.
- **Data Transformation:** Convert data types where necessary, tokenize text data, and prepare the data for analysis.

#### `4. Sentiment Analysis`
- **Method:** The Roberta sentiment analysis Pretrained Model from [HuggingFace](https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment) was used in analysising the sentiment of each review
- **Metrics:** The calculated sentiment scores of the positive, negative, neutral reviews was reviewed.

### 5. Data Analysis and Visualization
- **Descriptive Statistics:** We were able to scrape 3822 reviews from [Skytrax](https://www.airlinequality.com/), which includes verified customers and non-verified customers. For the purpose of this project, we will only be using the 2013 verified customers to be sure that the data we have are genuine. 

**Reviews from verified and non-verified customers.**
![Descriptive Statistics](img/df_describe_output.png)

**Reviews from verified customers only.**
![Descriptive Statistics](img/df_describe_verified_output.png)

**5-Star point ratings for verified customers**
Zero represents customers that did not provide a star review for each category
![Descriptive Statistics](img/point_review_BC.png)

**Recommendation from verified customers**
![Descriptive Statistics](img/recommendation_review_BC.png)

**Top 15 Countries with the Highest Number of "No Recommendations"**
![Descriptive Statistics](img/top_15_countries_with_no_in_recommendation.png)

**Top 15 Aircrafts with the Highest Number of "No Recommendations"**
![Descriptive Statistics](img/top_15_aircrafts_with_no_in_recommendation.png)

**MTop 20 most frequent words in Reviews**
![Descriptive Statistics](img/word_freq_result.png)


### `6. Insights`
- **Key Findings:** Sentiment analysis, performed using the RoBERTa pretrained model, classified the reviews as 28.6% positive, 8.6% neutral, and 62.7% negative

**Sentiment analysis result in percentage**
![Descriptive Statistics](img/sentiment_analysis_result.png)
- **Actionable Recommendations:**

**Positive World cloud**
![Descriptive Statistics](img/pos_wordcloud.png)

**Negative World cloud**
![Descriptive Statistics](img/neg_wordcloud.png)

### `Note:`
- To run the `ba_reviews_analysis.py`
- Run `pip install -r requirements.txt`, restart your jupyter notebook and then start running the cells.
