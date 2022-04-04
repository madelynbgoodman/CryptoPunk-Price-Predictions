CryptoPunk Price Predictions Using Machine Learning   


Madelyn Goodman
madelyn.b.goodman@gmail.com
https://www.linkedin.com/in/madelyn-b-goodman/


The first ever NFT “Quantum” was minted in 2014, since, the market has taken off to unprecedented heights. NFTs, (non-fungible tokens)  are non-interchangeable units of data. Unlike a cryptocurrency like ether (ETH) where one ETH can be traded for another identical ETH, each NFT is distinct, kind of like a social security number. People can trade and exchange these unique hashes through smart contracts on the Ethereum blockchain.
  
Woah, that was a lot of jargon... what is a blockchain? And what is Ethereum?
  
A blockchain is essentially an immutable digital ledger that operates off of a consensus mechanism. This means at least 51% of all the servers maintaining this ledger have to agree that a transaction is valid. The birth of the blockchain was the birth of a trustless system of exchange. Ethereum is a blockchain where transactions are executed using something called smart contracts. These are programs on the Ethereum blockchain that get executed when a certain set of conditions are met, such as an exchange of ETH, or the consensus of 51% of servers that a transaction is valid. NFTs use a specific kind of smart contract called an ERC-721 which are programmed to handle the transferability of these tokens and verify ownership. These contracts manage the exchange of ETH for the transfer of ownership of an NFT.
  
What does this have to do with this Capstone project? As with any asset/investment, being able to predict or forecast the movement of price or value is what every smart investor hopes to do.
  
CryptoPunks are an early NFT project that launched as free tokens in 2017 by Larva Labs that have since accumulated a trading volume of $1.7 billion with the most valuable punk selling for $23.7 million. In March 2022, Yuga Labs (creators of the Bored Ape NFTs) acquired management of the CryptoPunk collection.


There are 5 different types of CryptoPunks, each with a unique set of characteristics contributing to varying levels of rarity of each punk. The unique sets of characteristics that contribute to value and the fixed number of NFTs in this project provide an excellent case study for movement of price of this type of digital asset.
  
In addition to types and characteristics, the number of attributes each punk has, the value of ETH at the time of sale, who is buying and selling the punk, the number of days since the launch of the punks, average bids, and previous sale prices are all relevant and accessible features to use when building models to predict sale prices.


My primary source of data for this project was from a Kaggle dataset of Cryptopunk transactions from when the punks were first released in June 2017 until October 2021. I also used data on the daily closing price of Ethereum from Tradingview. 


I wanted to look at if machine learning techniques could be utilized to predict the prices of CryptoPunks in order to be able to formulate smart trading strategies. Using machine learning to predict stock prices is a common problem space for data scientists, setting a precedent for using such techniques to make predictions on the NFT market. 


The following files are required to execute the code found in the attached Jupyter Notebooks:


Virtual environment
* mbg_capstone_env.yml
   * This is the virtual environment I built that is equipped will all necessary packages to perform the analyses and data manipulation in this project. 
   * To install, run the following code in the terminal:
      * conda env create -f mbg_capstone_env.yml
      * conda activate capstone


Data
* Txn_history-2021-10-07.jsonl
* COINBASE_ETHUSD_1D.csv
* punk_sales_data.csv


All the code used to clean, perform exploratory data analysis, and build and evaluate my models can be found in the following Juptyer Notebooks:


* 01-CryptoPunk Price Prediction Data Cleaning and Pre-Processing 
* 02-CryptoPunk Price Prediction EDA
* 03-CryptoPunk Price Prediction Model Construction 
* 04-CryptoPunk Price Prediction Model Selection and Implementation


The following notebooks are appendices to the project and are not required to reproduce my results: 


* 03.1-CryptoPunk Price Prediction Using Keras Tuner
* 04.1-CryptoPunk Price Prediction Compiling Data on Recent and Upcoming Sales


Extra files generated from these notebooks are outlined below and can be found in the “generated_files” folder: 


* 01-CryptoPunk Price Prediction Data Cleaning and Pre-Processing 
   * traits_count.csv
   * traits.csv
   * type.csv
   * punk_data.csv
* 03-CryptoPunk Price Prediction Model Construction 
   * RandomForest_model.pkl
* 04-CryptoPunk Price Prediction Model Selection and Implementation
   * Neural_Network_13.pkl
* 04.1-CryptoPunk Price Prediction Compiling Data on Recent and Upcoming Sales
   * recent_sales_test.csv
   * upcoming_sales_test.csv


Finally, a brief summary of my work can be found in the MBG_Price_Prediction_Report.pdf file.


Acknowledgements 


I would like to acknowledge the following people that made this project possible:


* The Brainstation Data Science education team - their meticulous teaching styles and undying patience helped me build my data science skills from the ground up
* My classmates in the Brainstation Data Science Winter 2022 Bootcamp - the amount of support and camaraderie in this cohort and help offered by my peers greatly impacted the success of this project
* Kathy Bradley and Sandy Goodman - only with their support was I able to take this opportunity to make this career transition 
* Julian Marshall - through endless conversation and questions helped build my knowledge of the cryptocurrency and NFT space and also provided me with the data on ETH closings