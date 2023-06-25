# cryptoreview.ai

Now a large archive of news and reddit signals is open to the public. News data from late-2019 till May-2023 and reddit data from early-2019 till March-2023.

**How to interpret the data?**
There are two files under **data/** - **news_signals.csv** and **reddit_signals.csv** (data compressed to reduce overhead)
1) **ticker**: self explanatory
	supported tickers:
	['BTC', 'ETH', 'DOGE', 'ADA', 'LTC', 'XRP', 'XMR', 'XLM', 'BSV', 'BCH', 'CRO', 'TRX', 'EOS', 'ATOM', 'NEO', 'LINK', 'XTZ', 'ETC', 'DASH', 'USDT', 'MKR', 'ZEC', 'BNB', 'LUNA', 'MIOTA', 'LEO', 'HT', 'USDC', 'MATIC', 'ZRX', 'MANA', 'ALGO', 'BUSD', 'HOT', 'WAVES', 'DAI', 'FTT', 'THETA', 'VET', 'NEXO', 'QNT']
2) **datetime_hour**: date rolled up to the hour level(ceiling)
3) **signal** - name of the signal
	***Supported news signals:***
		- **news_pos_avg**: average of positive news articles
		- **news_neg_avg**: average of negative news articles
		- **news_pos_count**: number of positive news articles
		- **news_neg_count**: number of negative news articles
		- **news_sentiment_avg**: average of news sentiment
		- **news_num_of_articles**: number of news articles
		- **news_sentiment_index**: index created by cryptoreview.ai summarizing the news sentiment

    ***Supported reddit signals***
		- **reddit_submission_num_posts**: number of posts
		- **reddit_submission_ups**: number of ups at post level
		- **reddit_submission_sentiment**: sentiment at post level
		- **reddit_comment_num_comments**: number of comments
		- **reddit_comment_ups**: number of ups at comments level
		- **reddit_comment_sentiment**: sentiment at comments level
		- **reddit_hype_volatility_index**: index created by cryptoreview.ai summarizing reddit signals

4. **value_1hr_interval**: data rolled up to the hour level

5. **value_day**: cumulative data for day up to the current hour level
*Note: to use day level data, use the max value for each day as the last value indicates cumulative value for that day.*

---
![Alt text](extras/btc.png?raw=true "Bitcoin data - 2021")


![Alt text](extras/eth.png?raw=true "Ethereum data - 2021")


![Alt text](extras/doge.png?raw=true "Dogecoin data - 2021")

