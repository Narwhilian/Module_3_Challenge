# Crypto Arbitrage Application

This application takes in historical price data from the bitstamp and coinbase cypto currency exchanges and analyzes the difference in price shifts of Bitcoin (BTC) between the two exchanges to automatically identify arbitrage opportunites as well as note trends in the comparative pricing of BTC on each exchange over time.

---

## Technologies

This project uses the Python Programming language in a Jupyter Notebook as well as the following libraries
    
    - Pandas
    - Pathlib
    - matplotlib


---

## Installation Guide

To install you will want to pull the entire ARBITRAGE folder from github including its subfolder
    
    * Subfolder
        * Resources (data folder)
        * crypto_arbitrage (the jupyter notebook itseld)


---

## How it works

1) First the user will open the crypto_arbitrage.ipynb in the arbitrage folder
2) Then the user will simply run each cell in the notebook to get its output

    i) The app will collect the data from the bitstamp.csv and the coinbase.csv file in the Resources folder and read them each into a dataframe
    
    ii) Then it will check each dataframe for null values and drop any rows containing null values
    
    iii) Then it will process the data, removing the "$" from the close column in each dataframe and re type the data in that column as a float
    
    iv) Then it will drop duplicate data if there is any
    
    v) Then it will begin the analysis of the data frames by taking a slice of data (close column) from each data frame and provide the summary statistics for each dataframe
    
    vi) Then it will graph the historical close data both individually and together
    
    vii) Then it will examine the intra day data from three dates, by providing the summary stats as well as graphing it as both a line and box plot
    
    viii) Then it will identify all potential arbitrage opportunities buying from bitstamp and selling to coinbase
    
        a) It will then further refine the arbitrage opportunities by narrowing down the list to those that had a profit over 1% (the cost of buying and selling on the exchanges)
      
        b) Then it will find the summary stats for each days arbitrage as well as the cumulative profits for each day and analyze the trend in arbitrage profit as time progresses

---

## Usage

Overall it should be a very simple application to use, all you need to do is open the crypto_arbitrage.ipynb app in the arbitrage folder and run each cell in order


---

## Contributors

Colin Benjamin

Linkedin: [Colin Benjamin](https://www.linkedin.com/in/colinbenjamin/)
    
email: cbenjamin33@gmail.com

---

## License

MIT

