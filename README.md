# Webscraping-Stocks-and-Prices
Program 1
The CNN Money’s Market Movers website (https://money.cnn.com/data/hotstocks/) tracks the most active stocks on a real-time basis. Specifically, the most active, the top gainers and the top losers are listed at any instance in time. This program collects the list of most actives, gainers, and losers from the above website. Next, this program takes the ticker symbols and names of these companies (and categories) to build a csv file (called something like 20191201-212519.csv in which the title of the csv is determined by the time created saving it as the output year/month/day-hour/minute/seconds.csv) with data about each stock from the website: https://finance.yahoo.com/quote/AMD?p=AMD&.tsrc=fin-srch-v1, which gives the quote for ticker symbol AMD as an example. The data to be collected from the Yahoo Finance site includes:

OPEN price
PREV CLOSE price
VOLUME
MARKET CAP
This program also lists the names of the companies in the order and categories listed in the website https://money.cnn.com/data/hotstocks/ and prompts the user to choose a company to get the data on. Once the user chooses the company of interest, this program displays its corresponding data (Open, Prev Close, Volume, and Market Cap).

If the web page or server no longer exist (this includes internet connection), the program will display an error message and end.
Sample Runs (user input in BOLD):
This is a program to scrape data from the https://money.cnn.com/data/hotstocks/ for a class project.
Which stock are you interested in:

Most Actives:
AMD Advanced Micro Devices Inc
GE General Electric Co
BAC Bank of America Corp
WBA Walgreens Boots Alliance Inc
AAPL Apple Inc
F Ford Motor Co
FCX Freeport-McMoRan Inc
CSCO Cisco Systems Inc
OXY Occidental Petroleum Corp
MU Micron Technology Inc

Gainers:
WBA Walgreens Boots Alliance Inc
MKTX Marketaxess Holdings Inc
NVR NVR Inc
ARNC Arconic Inc
GPS Gap Inc
EQIX Equinix Inc
ULTA Ulta Beauty Inc
TTWO Take-Two Interactive Software Inc
M Macy's Inc
NWSA News Corp

Losers:
FCX Freeport-McMoRan Inc
WYNN Wynn Resorts Ltd
COTY Coty Inc
CNP CenterPoint Energy Inc
ABC AmerisourceBergen Corp
MRO Marathon Oil Corp
ATVI Activision Blizzard Inc
COG Cabot Oil & Gas Corp
XRAY Dentsply Sirona Inc

User inputs: COTY

The data for COTY Coty Inc is the following:

COTY Coty Inc
OPEN: 12.78
PREV CLOSE: 12.84 VOLUME: 2,000,995
MARKET CAP: 9.580B

If the user enters something other than the listed company symbols, the program will display a message about the user's error and end.

The csv should look something like this for one entry:
Losers,COTY,Coty Inc,12.78,12.84, 2000995,9.580B
If the program cannot access the location to save a file with the stock data, the program will display an error message and end.
