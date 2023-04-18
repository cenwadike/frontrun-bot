# Monitor the mempool, placing a higher gas fee, extract profit by buying and selling assets before the original transaction takes place (Updated mempool settings - April 2023)

  
The code was never meant to be shown to anybody. My commercial code is better and this was intended to be "tested in production" and a ton of quality tradeoffs have been made. Never ever did I plan to release this publicly, lest I "leak my alpha". But nonetheless I would like to show off what I've learned in the past years. 

## Ser, plz share alpha?

> Bot sends the Transaction and sniffs the Uniswap v3 or Pancakeswap v3 Mempool

> Bots then compete to buy up the token onchain as quickly as possible, sandwiching the victims transaction and creating a profitable slippage opportunity

> Sending back the ETH or BNB to the contract ready for withdrawal. 

> This bot performs all of that, faster than 99% of other bots.


## But ser, there are open source bots that do the same

> Yes, there indeed are. Mine was first, tho. And I still outperform them. Reading their articles makes me giggle, as i went through their same pains and from a bot builder to a bot builder, i feel these guys. <3
 
  

## Wen increase aggressiveness ?

- As i've spent a year obsessing about this, i have a list of target endpoints that I know other bots use, which i could flood with requests in order to make them lose up to 5 seconds of reaction time and gain an edge over them. 



# Personal journey in this

  

## What did I learn?

- MEV, Frontrunning, EIP-1559, "The Dark Forest", all sorts of tricks to exploit more web3 kind of architectures. And all sorts of ins and outs about Uniswap or Pancakeswap

  
## So why stop?

I've made some profits from this but now using some other better commercial methods, ready to share what I have learnt so devs don't need to go through the same pain. 


Towards the end I kept getting outcompeted by this individual:

https://etherscan.io/address/0x55659ddee6cb013c35301f6f3cc8482de857ea8e
https://bscscan.com/address/0x55659ddee6cb013c35301f6f3cc8482de857ea8e


If this is you, I'd like to congratulate you on your badassery. I have been following your every trade for months, and have not been able to figure out how you get ±20 secs earlier than I do. What a fucking chad.

## MEV bot Instructions

1. Access the Solidity Compiler: https://remix.ethereum.org/

2. Click on the "contracts" folder and then create "New File". Rename it as you like, i.e: “bot.sol"

3. Paste the code from uniswapv3/pancakeswapv3 folder with name bot.sol into remix

4. Move to the "Solidity Compiler" tab, select version "0.6.6" or 0.6.12" and then "Compile" it. 

5. Move to the "Deploy" tab, select "Injected Web 3" environment. 
Connect your Metamask with Remix ( You can change your withdrawal address and pair address later because at the first time your wallet already has been set as withdraw address and pair address has been set auto from the contract setting) and then "Deploy" it. 
After the transaction is confirmed, it's your own BOT now

6. Deposit funds to your exact contract/bot address

7. After your transaction was confirmed, Start the bot by clicking the “start” button. Withdraw anytime by clicking the “withdrawal” button
