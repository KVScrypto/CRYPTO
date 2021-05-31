## CRYPTO
Cryptocurrency is the Decentralized Digital Asset that acts as a store of value as well as a medium of exchange.
It is built on Blockchain Technology which  uses an online ledger with strong cryptography to secure online transactions.

## Team-KVS
#### Karan
#### Vicky
#### Shagun
 How do Bitcoin markets behave? What are the causes of the sudden spikes and dips in cryptocurrency values? Are the markets for different altcoins, such as Dogecoin and Ethereum, inseparably linked or largely independent? How can we predict what will happen next?

Articles on cryptocurrencies, such as Bitcoin and Ethereum, are rife with speculation these days, with hundreds of self-proclaimed experts advocating for the trends that they expect to emerge. What is lacking from many of these analyses is a strong data analysis foundation to backup the claims.

So we would be using Time series Modelling to forecast the cyptocurrency market trend(prices) and NLP for the sentiment analysis.
***
## key data fields

### Price related fields

- open: The opening price for the time range.
- close: The closing price for the time range.
- high: The highest price for the time range.
- low: The lowest price for the time range.
- volumeUSD: The trading volume in USD for the time range.
### Sentiment related fields

- source: The source of the community discussion data which the sentiments are computed upon.
- count: The number of discussions used to compute the sentiments. They can be posts, comments, or a chat message. Garbage discussions are excluded (e.g. a meme message with no text)
- average: The average sentiment value for all discussions in the time range, where each discussion's sentiment is predicted to be between 1-5 (with 3 as neutral)
- std: The standard deviation of the sentiments across all discussions in the time range.
- positive: Estimated percentage of relatively positive discussions in this time range.
- negative: Estimated percentage of relatively negative discussions in this time range.
- score: An adjusted sentiment score we computed for this time range. It is always between [0, 1]. We use a methodology that is designed to give higher scores when the proportion of positive discussions are high, and is less sensitive to overwhelming negative discussions. It shows many desirable statistical properties such as an empirical distribution with nicely spread and reasonable mean, among other things.
