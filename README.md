# Cryptocurrency Wallet

A startup is building a new and disruptive platform called Fintech Finder. Fintech Finder is an application that its customers can use to find fintech professionals from among a list of candidates, hire them, and pay them. This code integrates the Ethereum blockchain network into the application in order to enable human resources stuff to instantly pay the fintech professionals whom they hire with cryptocurrency. 


## Technologies
The project uses the following technologies and libraries:

 **Bip44, Web3, Crypto Wallet, Streamlit, Hashlib, Dataclasses, Typing, OS, Requests.** To manage credentials we use **Dotenv.**

We used `Python 3.7` in the coding.


## Instalation Guide

If you don't have it already, you need to install Streamlit. To assure the program will run properly, we recommend version 0.84.2 for Streamlit. If you have other versions, you may want to run the following commands on your terminal:


`pip uninstall streamlit -y`

`pip install streamlit==0.84.2`


The main file is `fintech_finder.py`. You need to open your terminal or GitBash on the folder where this file is, and then run:

    `streamlite run fintech_finder.py`

A local host address will appear. You may be redirected to a page in your browser, but if not, you may copy and paste directly the address in yours.


### Usage

#### Interface
The following screenshot is a sample of the Fintech Finder screen. The candidates information is displayed in the right panel. On the left panel, the you can select a candidate to hire, and the amount of hours associated. The application automatically calculates the total wage to be paid. By hitting the Send Transaction button, the application executes the payment of that wage on Ethereum network.  


![StreamlitInterface](images/StreamlitInterface.png)


#### Integration with Ethereum

To verify the integration with the Ethereum network, we will do a transaction and then verify that the transaction was recorded in the Ethereum network.

We made a payment of 0.0019 ether to Joe. Below we verify a balance and transaction history screenshot of the company in Etherscan after 13 min. We can see:

    1) The company address starting in 0xB2 and ending in CA7
    2) A remaining balance is 0.001 ether
    3) A "transfer" transaction going "out" from the company account to Joe's account of 0.0019 ether (13 min ago)
    
![EmployerBalanceAndHistory](images/5_EmployerBalanceAndHistory.png)

A similar situation we can verify on Joe's account balance and transaction history screenshot on Etherscan below. We can see that the last transaction was a transfer in of 0.0019 ether coming from the employer account. The screenshot is from 1 minute after executing the transaction:

![BalanceHistory](images/1_AddressBalancerAndHistory.png)


##### Transaction details
On the Kovan Etherscan page, if you click on the Txn Hash number associated with the transaction that paid the Fintech Finder candidate you can see the details about the transaction, inclñuding status, gas used, gas limit, among many other characteristics:

![TransactionDetailsOnEtherscan2](images/3_TransactionDetailsOnEtherscan2.png)



## Contributors
This project was coded by Paola Carvajal Almeida, QuantitativePaola@gmail.com.

Contact email: QuantitativePaola@gmail.com
LinkedIn profile: https://www.linkedin.com/in/paolacarvajal/
GitHub: https://github.com/paocarvajal1912


## License
This project uses a MIT license. This license allows you to use the licensed material at your discretion, as long as the original copyright and license are included in your work files. This license does not contain a patent grant,  and liberate the authors of any liability from the use of this code.


