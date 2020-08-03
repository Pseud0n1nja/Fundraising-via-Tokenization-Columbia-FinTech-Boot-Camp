# Fundraising-via-Tokenization

## Project Description

Due to the large amount of capital and long investment horizons required in order to pursue their strategies, Private Equity funds have traditionally been exclusive investment opportunities offered to high net worth individuals, corporations, and asset managers. The average retail investor seeking to add private companies to their portfolio is generally unable to do so without connections in the space, resulting in a large capital pool left untapped or invested into more accessible investment vehicles. This project seeks to create an application that connects private equity fund managers and retail investors by using blockchain to tokenize investment into a fund into “shares” that can be bought and traded.

## Instructions

In order to run this code, you must have an active environment that has Python, Web3, ipywidgets, and Jupyter installed. You must also have set up Ethereum crypto-wallets on the Kovan test network (I recommend doing so via MetaMask and Ganache). 

Once you have this set up, you must open Remix (remix.ethereum.org), and deploy the following smart contract files in the following order:
* FundACoin.sol - this creates the token entity using ERC20 standards.
* CrowdsaleA.sol - this initiates the crowdsale. The FundACoin smart contract must be referenced, and an Ethereum wallet account into which to mint the tokens must be provided when deploying the contract.

Once the tokens have been minted, open up Jupyter and run the portfolio_dashboard.ipynb file. To buy tokens, enter in the account number and private key for a different Ethereum wallet (with enough test Ether to buy the tokens per the specified price when deploying the crowdsale contract) in the top half of the dashboard. Once tokens have been sold, they may be traded using the trading tool in the bottom half of the dashboard. 