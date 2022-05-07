# Blockchain Wallet

I am building a new and disruptive platform called Fintech Finder. Fintech Finder is an application that its customers can use to find fintech professionals from among a list of candidates, hire them, and pay them. As Fintech Finder’s lead developer, I've been tasked with integrating the Ethereum blockchain network into the application in order to enable your customers to instantly pay the fintech professionals whom they hire with cryptocurrency.

### What we are Creating

We will use two Python files, both of which are contained in the starter folder.

The first file that you will use is called fintech_finder.py. It contains the code associated with the web interface of your application. The code included in this file is compatible with the Streamlit library. You will write all of your code for this Challenge in this file.

The second file that you will use is called crypto_wallet.py. This file contains the Ethereum transaction functions that you have created throughout this module’s lessons. By using import statements, you will integrate the crypto_wallet.py Python script into the Fintech Finder interface program that is found in the fintech_finder.py file.

Integrating these two files will allow you to automate the tasks associated with generating a digital wallet, accessing Ethereum account balances, and signing and sending transactions via a personal Ethereum blockchain called Ganache.

We will do the following task:

Generate a new Ethereum account instance by using the mnemonic seed phrase provided by Ganache.
Fetch and display the account balance associated with your Ethereum account address.
Calculate the total value of an Ethereum transaction, including the gas estimate, that pays a Fintech Finder candidate for their work.
Digitally sign a transaction that pays a Fintech Finder candidate, and send this transaction to the Ganache blockchain.
Review the transaction hash code associated with the validated blockchain transaction.

### Localhost 8501 Screenshot


![2022-05-07 (14)](https://user-images.githubusercontent.com/93211640/167274598-58cb2efc-3cc4-4e62-af6b-aabfb0b1975e.png)


### Address Balance Screenshot

![2022-05-07 (8)](https://user-images.githubusercontent.com/93211640/167274282-7f4e83de-dd91-4f3e-bae4-514961f3d294.png)


### Transaction Details' Screenshot

![2022-05-07 (3)](https://user-images.githubusercontent.com/93211640/167274310-3c6af6dd-91f1-42d7-9837-4923d3955a8e.png)

### Transactions To Address screenshot

![2022-05-07 (9)](https://user-images.githubusercontent.com/93211640/167274399-168ca70f-a02c-40ab-83f5-295859a1818b.png)

### ***Installation Guide***
Before running the application first install the following dependencies.

### Imports for crypto_wallet.py

import os

import requests

from dotenv import load_dotenv

load_dotenv()

from bip44 import Wallet

from web3 import Account

from web3 import middleware

from web3.gas_strategies.time_based import medium_gas_price_strategy

### Imports for fintech_finder.py

import streamlit as st

from dataclasses import dataclass

from typing import Any, List

from web3 import Web3

w3 = Web3(Web3.HTTPProvider('HTTP://127.0.0.1:7545'))


### Usage 

After cloning the repository, open the directory Module_19_Challenge/Starter_Code in Gitbash and run the program by typing ***streamlit run fintech_finder.py***

#### Contributors

James Tagapan

jtagapan@gmail.com

#### License

Licensed under the MIT License. Copyright 2020# Module_10_Challenge
