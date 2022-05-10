# Unit 21

## Martian Token Crowdsale

My name is Oscar Lopez, I’m a student at the University of Miami FinTech Bootcamp Program.

In this activity, I was tasked with creating a monetary system for the first human colony on Mars, this system will be blockchain technology based and will have a cryptocurrency coin named KaseiCion or KAI. (Kaise means Mars in Japanese).

I developed the Solidity started code file KaseiCoin.sol to create the Token Contract containing a fungible token that is ERC-20 compliant, starting with the pragma statement for Solidity version 0.5.0, then importing the contracts from the from the OpenZeppelin library (ERC20, ERC20Detailed and ERC20Mintable), next defining a contract for the “KAI” coin and inheriting the three contracts imported from OpenZeppelin. Inside the “KAI” contract, I added a constructor with the name, symbol, and initial supply parameters, then I added a call to the constructor of the ERC20Detailed contract, passing the name, symbol and 18 (Decimals values) as parameters. Finally, I compiled the contract.

Also, I developed the Solidity started code file KaseiCoinCrowdsale.sol to create the crwodsale contract that will manage the entire process that allows the users to send ether to the contract and receive KaseiCoin tokens / KAI in return, the contract automatically mints the tokens and distribute them to a buyer in one transaction. I started with the pragma statement for Solidity version 0.5.0, then imported the contracts from the from the OpenZeppelin library (Crowdsale and MintedCrowdsale), next I defined a constructor providing the rate, wallet, and token parameters. Finally, I compiled the contract.
Then, I created the  the KaseiCoin Deployer Contract, I added variables to store addresses of the KaseCoin and KaseiCoinCrowdsale contracts, then I created a public address variable which will store the KaseiCoin address, a public address variable which will store the KaseiCoinCrowdsale address, a constructor with a name, symbol, and wallet parameters, inside it holds a new instance of the KaseiCoinToken contract with an assign address of the KaseiCoin token variable to the kasei_token_address variable. It also holds a new instance of the KaseiCoinCrowdsale contract by using rate (1) wallet (from main constructor), and token parameters. Then, I set the KaseiCoinCrowdsale contract as a minter and the KaseiCoinCrowdsaleDeployer renounce its minter role and finally, I compiled the contract.

Ultimately, I deployed and tested the Crowdsale on a my local Blockchain, by using Remix, MetaMask and Ganache, then performed real-world preproduction test by using test accounts to buy new tokens and then checking the balances of those accounts. Finally, I review the total supply of minted tokens and the amount of wei that the crowdsale contract has raised.

-----------------------------------------------------------------------------------------------------------------------------------------------------------

## Solidity – KaseiCoin Contract Compiler
![Stocks Phot](
https://github.com/Maurolp15/Unit_21_Martian_Token_Crowdsale/blob/main/Evaluation%20Evidence/Screenshot_1.png?raw=true)


-----------------------------------------------------------------------------------------------------------------------------------------------------------

## Solidity – KaseiCoinCrowdsale Contract Compiler
![Stocks Phot]( https://github.com/Maurolp15/Unit_21_Martian_Token_Crowdsale/blob/main/Evaluation%20Evidence/Screenshot_2.png?raw=true)


-----------------------------------------------------------------------------------------------------------------------------------------------------------

## Solidity – KaseiCoinCrowdsaleDeployer Contract Compiler
![Stocks Phot]( https://github.com/Maurolp15/Unit_21_Martian_Token_Crowdsale/blob/main/Evaluation%20Evidence/Screenshot_3.png?raw=true)


-----------------------------------------------------------------------------------------------------------------------------------------------------------

## Solidity – KaseiCoin Contract Deploy
![Stocks Phot]( https://github.com/Maurolp15/Unit_21_Martian_Token_Crowdsale/blob/main/Evaluation%20Evidence/Screenshot_4.png?raw=true)


-----------------------------------------------------------------------------------------------------------------------------------------------------------

## Solidity – KaseiCoinCrowdsaleDeployer Contract Deploy
![Stocks Phot]( https://github.com/Maurolp15/Unit_21_Martian_Token_Crowdsale/blob/main/Evaluation%20Evidence/Screenshot_5.png?raw=true)


-----------------------------------------------------------------------------------------------------------------------------------------------------------

## Solidity – KaseiCoinCrowdsale Contract Deploy
![Stocks Phot]( https://github.com/Maurolp15/Unit_21_Martian_Token_Crowdsale/blob/main/Evaluation%20Evidence/Screenshot_6.png?raw=true)


-----------------------------------------------------------------------------------------------------------------------------------------------------------

## Solidity – kasei_crowdsale and kasei_token Addresses
![Stocks Phot]( https://github.com/Maurolp15/Unit_21_Martian_Token_Crowdsale/blob/main/Evaluation%20Evidence/Screenshot_7.png?raw=true)


-----------------------------------------------------------------------------------------------------------------------------------------------------------

## Solidity – KaseiCoinCrowdsale Contract Transaction
![Stocks Phot]( https://github.com/Maurolp15/Unit_21_Martian_Token_Crowdsale/blob/main/Evaluation%20Evidence/Screenshot_8.png?raw=true)


-----------------------------------------------------------------------------------------------------------------------------------------------------------

## Solidity – Ganache 8 Account Balance 
![Stocks Phot]( https://github.com/Maurolp15/Unit_21_Martian_Token_Crowdsale/blob/main/Evaluation%20Evidence/Screenshot_9.png?raw=true)

-----------------------------------------------------------------------------------------------------------------------------------------------------------

## Solidity – Ganache 9 Account Balance 
![Stocks Phot]( https://github.com/Maurolp15/Unit_21_Martian_Token_Crowdsale/blob/main/Evaluation%20Evidence/Screenshot_10.png?raw=true)
