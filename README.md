# googleFinanceHistoryTracker
This scripts fills a spreadsheet with historical profit from another spreadsheet containing stock data.

The data obtained from the frist sheet have the following structure:
Date,	Operation,	Name,	Ticker,	Market,	Shares,	Price (in origin currency),	Currency, Investment (in origin currency),	Sotck price (Origin currency),	broker coststs 1 (€), Broker costs2 (€),	Broker cotsts 3 (€), 	Currency exchange when bought,  currency exchange charged by broker, current exchange price, current exchange applied by broker, profit, net profit,	buy (€)	sell (€)	benefit (€)	profit with dividends,  dividends,  broker, sold or not (1 - 0),  sold date, 	Sector

The data obtained from the dividends sheet have the following structure:
Date,	Name,	Ticker,	Market,	Type,	Value.


This file was created to generate the historical  from a european market, therefore all currencies are transformed to euros..
The starting date must be changed in more than one place. It generates a row for every 15 days, but that can also be changed.

Note: This will generate a lot of queries to googlefinance from the spreadsheet, and that may take a while to get the data, and probably it will also slow down the browser. But right now at 27/11/2017 I wasn't able to find another way to get values from a specific directly from a script, yahoo api and googlefinance api from the script are deprescated.
