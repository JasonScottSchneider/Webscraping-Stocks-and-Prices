# Webscraping-Stocks-and-Prices
## Program 1
The CNN Money’s Market Movers website (https://money.cnn.com/data/hotstocks/) tracks the most active stocks on a real-time basis. Specifically, the most active, the top gainers and the top losers are listed at any instance in time. This program collects the list of most actives, gainers, and losers from the above website. Next, this program takes the ticker symbols and names of these companies (and categories) to build a csv file (called something like <b>20191201-212519.csv</b> in which the title of the csv is determined by the time created saving it as the output year/month/day-hour/minute/seconds.csv) with data about each stock from the website: https://finance.yahoo.com/quote/AMD?p=AMD&.tsrc=fin-srch-v1, which gives the quote for ticker symbol AMD as an example. The data to be collected from the Yahoo Finance site includes:<br>
<blockquote>OPEN price<br>
PREV CLOSE price<br>
VOLUME<br>
MARKET CAP</blockquote>
This program also lists the names of the companies in the order and categories listed in the website https://money.cnn.com/data/hotstocks/ and prompts the user to choose a company to get the data on. Once the user chooses the company of interest, this program displays its corresponding data (Open, Prev Close, Volume, and Market Cap).<br>
<br>
If the web page or server no longer exist (this includes internet connection), the program will display an error message and end.
<br>
Sample Runs (user input in BOLD):<br>
<blockquote>This is a program to scrape data from the https://money.cnn.com/data/hotstocks/ for a class project.
<br>
Which stock are you interested in:<br>
<br>
Most Actives:<br>
AMD Advanced Micro Devices Inc<br>
GE General Electric Co<br>
BAC Bank of America Corp<br>
WBA Walgreens Boots Alliance Inc<br>
AAPL Apple Inc<br>
F Ford Motor Co<br>
FCX Freeport-McMoRan Inc<br>
CSCO Cisco Systems Inc<br>
OXY Occidental Petroleum Corp<br>
MU Micron Technology Inc<br>
<br>
Gainers:<br>
WBA Walgreens Boots Alliance Inc<br>
MKTX Marketaxess Holdings Inc<br>
NVR NVR Inc<br>
ARNC Arconic Inc<br>
GPS Gap Inc<br>
EQIX Equinix Inc<br>
ULTA Ulta Beauty Inc<br>
TTWO Take-Two Interactive Software Inc<br>
M Macy's Inc<br>
NWSA News Corp<br>
<br>
Losers:<br>
FCX Freeport-McMoRan Inc<br>
WYNN Wynn Resorts Ltd<br>
COTY Coty Inc<br>
CNP CenterPoint Energy Inc<br>
ABC AmerisourceBergen Corp<br>
MRO Marathon Oil Corp<br>
ATVI Activision Blizzard Inc<br>
COG Cabot Oil & Gas Corp<br>
XRAY Dentsply Sirona Inc<br>
<br>
User inputs: <b>COTY</b><br>
<br>
The data for COTY Coty Inc is the following:<br>
<br>
COTY Coty Inc<br>
OPEN: 12.78<br>
PREV CLOSE: 12.84 VOLUME: 2,000,995<br>
MARKET CAP: 9.580B<br>
<br></blockquote>
If the user enters something other than the listed company symbols, the program will display a message about the user's error and end.<br>
<br>
The csv should look something like this for one entry:<br>
<blockquote>Losers,COTY,Coty Inc,12.78,12.84, 2000995,9.580B</blockquote>
If the program cannot access the location to save a file with the stock data, the program will display an error message and end.
