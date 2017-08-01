# Bittrex Command-Line Trader
## Andre V. Banks


A commandline application for Mac OS that enables coin tradring through Bittrex on the CLI. To run the application it needs to be granted execution permission this can be done by running the following command in the directory of the "cli_trader.py" file ```bash
chmod u+x cli_trader.py ```
.A secrets.py file needs to be created which will hold the API key and secrety generated from Bittrex. The cli_trader.py file contains a global variable 'LOT' this determines what dollar lots the coins should be traded.  The default value is 5 which means coins will be traded in $5 USD lots.  This functionality makes trading between coins a lot easier to deal with.  Due to the extremely volatile nature of Bitcoin I find pricing purchase size in USD a lot easier.   


## Commands

## Default Functionality
### ./cli_trader.py (no arguments)
The default functionality will cause all purchased coins to be displayed with each positions total value and the total value of the portfolio displayed.
The the coins rank, ticker, 1hr, 24hr, and 7day change will be displayed.

]==========================================  
Bitcoin $1050.0000  
Rank 1 | 1 HR %10 | 24HR %20 | 7D %50  
]==========================================  
Balance $90000

![Cli Defualt Functionality](https://media.giphy.com/media/l0EoBilWm7mOSksta/giphy.gif)

## Buy Order @ ASK Price
### ./cli_trader.py --b <ticker> <lots>




