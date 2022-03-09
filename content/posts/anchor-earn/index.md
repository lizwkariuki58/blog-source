---
title: "Anchor Earn"
date: 2022-03-09T11:58:41+03:00
draft: false


description: "Earning a Guaranteed Return on Anchor"
---



# How To Deposit Funds into Anchor Earn

Anchor Earn on the Terra network is one of the safest way to park money in crypto and earn a guaranteed return. It is 'a decentralized savings protocol offering low-volatile yields on Terra stablecoin deposits'. At time of writing, there is $14 billion locked in Anchor earning an interest of 19.46% APY. In this guide I will show you how to go from Kenya shillings to UST in Anchor's Earn protocol; a process that requires a few steps that can be daunting for a beginner. TerraUSD (UST) is a stablecoin on Terra. This means that unlike other crypto tokens whose value is volatile, it's value is always pegged to one dollar. 

Before we get started, I would like to pass on a bit of wisdom I have learned during my short stint in the crypto ecosystem: always plan out your process in advance. Be sure there is a clear path from the time you on-board your fiat money to getting it on whichever blockchain you want. In this article, I will explain the straightforward way of doing things as well as some workarounds if that way does not work for you. But soon you will learn the importance of doing some research before moving your cryptocurrency. 



## Buy Cryptocurrency Using Kenyan Shillings

You will need to use a fiat on-ramp (typically a centralized exchange such as Binance, Coinbase, Kraken) to buy a crypto coin or token. Some tokens cannot be bought on these exchanges and good workaround for that is buying a stablecoin e.g. USDT, USDC, DAI and later swapping it for the token you want. 

I have used Binance so far and it is not possible to buy UST directly on the peer to peer platform using MPESA or a bank card. I have not tried it on the other exchanges. But if you want to use Binance, you can go ahead and buy any stablecoin e.g. Tether, BUSD, DAI etc on the peer to peer platform and pay via MPESA or card. There is however, a minimum of Ksh.2000 and a maximum of Ksh.280,000 when using Binance. 

## Create a Crypto Wallet

Congratulations on your first purchase of cryptocurrency! However, there is a saying in the crypto world that says:

> Not your keys, not your coins.

What this means is that even though you just bought and paid for this cryptocurrency, it is still under the control of the exchange. To truly own and control your crypto you need to create a crypto wallet to hold it. Controlling your money does not come without it's disadvantages. Crypto wallets are recovered/opened using a unique recovery phrase that only you have. If you lose this phrase, you lose access to your cryptocurrency forever and if anyone else gets a hold of it, they can transfer your coins elsewhere. There is no recourse for such an action. [These](https://cryptopotato.com/9-must-tips-securing-crypto-wallet/) are some tips on how to secure your wallet. There are different crypto wallets used by different blockchains but in this guide, I will show you how to create two of them:

### i. Metamask

[Metamask](https://metamask.io/)  is one of the most popular wallets since it is compatible with many popular blockchains and it is easy to use. You can get it as a browser extension or an Android/iOS app. 

### ii. Terra Station Wallet

You need a Terra Station Wallet to interact with the Terra ecosystem. You can get it [here](https://docs.terra.money/docs/learn/terra-station/download/README.html) as a desktop app, a browser extension or a mobile app.

## Withdraw Coins From Exchange to Crypto Wallet

Now that you have your wallet set up, it is time to truly own your coins. Before sending any tokens to a wallet, you have make sure that the wallet is set up to hold them. This is done by:
a) Adding the network to metamask e.g. [Binance Smart Chain](https://academy.binance.com/en/articles/connecting-metamask-to-binance-smart-chain) or [Polygon](https://docs.polygon.technology/docs/develop/metamask/config-polygon-on-metamask).
b) Add the token contract address of the token you want to add to the wallet. You can get this from the token's official site or on [bitquery](https://explorer.bitquery.io/).

You should be very careful to get the above steps right because if you do not, you could lose your tokens. Make sure you are using the official documentation and go through the details again to ensure you did not make a mistake. 

Once this is done, you can withdraw your crypto from the custodial wallet on the exchange to your own hot crypto wallet. The different centralized crypto exchanges have their own minimum amounts to withdraw, chains to withdraw to and fees levied. 

On Binance, you have two options:

### i. Swap USDT for UST and withdraw it

You could [convert](https://www.binance.com/en/blog/otc/binance-convert-making-crypto-transactions-quick-and-easy-for-all-421499824684901797) the stablecoin that you bought -we will use Tether(USDT) for this example - to UST and withdraw it. To do this you need to withdraw a minimum of 50 UST. So you need to have bought slightly more than 50 USDT to cater for the conversion and withdrawal fee. 55 USDT would be more than enough for this option and you'd still have some USDT left on Binance to pay for other fees if you need to. At time of writing, you need roughly Ksh. 6500 to use this option. 

After performing the convertion, you can withdraw the UST on the following chains at time of writing: BSC, Ethereum, Terra and Polygon. I would suggest we withdraw the UST to Terra since that is the ecosystem we want it in. No need to add a contract address to Terra Station wallet since it is created and configured specifically to hold tokens in the Terra ecosytem. See [these](https://thefipharmacist.com/binance-to-terra-station/) instructions to withdraw UST from Binance into your Terra Station wallet. 

I like this option since it reduces the number of steps you take and thereby reduces the opportunities for mistakes to be made. It does require you to have quite a bit of money though but don't worry if you do not. You still have another option. 

### ii. Withdraw USDT to Metamask

If your funds are low, you could simply withdraw them to metamask. Currently, you can withdraw USDT on 6 chains including BSC, Solana and Tron which have a minimum withdrawal amount of 10 USDT and a fee of 1 USDT with the exception of BSC which has a fee of 0.8. Note that the lower the amount you withdraw, the higher the percentage taken up by fees. 

To withdraw USDT from Binance on the Binance Smart Chain (BSC) network on Metamask, you'll need to add the BSC network as explained above. You  also need to add the USDT contract address given [here](https://explorer.bitquery.io/bsc/token/0x69bab60997a2f5cbee668e5087dd9f91437206bb). After performing these steps, you are ready to receive the USDT from Binance into your Metamask wallet. See [these](https://www.binance.com/en/support/faq/115003670492) instructions on how to withdraw from Binance. 

Once you have received USDT into your Metamask wallet, you need to swap it for UST on a decentralized exchange such as [nerve.fi](https://nerve.fi/). Note that this incurs a tiny fee. Now you have UST but it still on the BSC network and in Metamask. We need it in your Terra Station Wallet and on the Terra network. This process is called bridging and you can use the official [Terra Bridge](https://bridge.terra.money/) to do this. Again, make sure to double check everything, especially your wallet address and note that this also incurs a small fee. 

## Deposit UST into Anchor

Now that you have UST in your Terra Station it is time to do what brought us here: Deposit it into Anchor Earn. The Anchor protocol [documentation](https://docs.anchorprotocol.com/user-guide/webapp/earn) is very clear on how to do this. You may note that the amount of UST you deposit is not what you see on Anchor's interface. This is because technically, what you are doing is using your UST to buy [aUST](https://docs.anchorprotocol.com/protocol/money-market#anchor-terra-aterra) (anchor TerraUSD) which is the asset that earns interest on Anchor. Do not worry though, when you withdraw your money and interest earned, it will be converted back to UST. Now sit back and enjoy your returns!



