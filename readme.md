A mini simulation of the Stock Exchange
---
A WebApp that enables authenticated users to trade stocks using simulated funds, access real-time stock quotes from the **alphavantage API**, and view their portfolio’s transaction history.
Try it out [here](https://stockex.onrender.com/).

<!-- more -->

## Technologies
* Python
* Flask with session authentication
* SQL
* HTML
* Bootstrap

## Features
* **Register** - Allows a new user to register for an account, rendering an apology view if the form data is incomplete or if the username already exists in the database.

* **Index** - The homepage displays a table of the logged-in user's owned stocks, number of shares, current stock price, value of each holding. This view also shows the user's imaginary "cash" balance and the total of their "cash" plus stock value.

* **Quote** - Allows the user to submit a form to look up a stock's current price, retrieving real-time data from the Alphavantage API. An error message is rendered if the stock symbol is invalid.

* **Buy** - Allows the user to "buy" stocks by submitting a form with the stock's symbol and number of shares. Checks to ensure the stock symbol is valid and the user can afford the purchase at the stock's current market price with their available balance, and stores the transaction history in the database.

* **Sell** - Allows the user to "sell" shares of any stock currently owned in their portfolio.

* **History** - Displays a table summarizing the user's past transactions (all buys and sells). Each row in the table lists whether the stock was bought or sold, the stock's symbol, the buy/sell price, the number of shares, and the transaction's date/time.
