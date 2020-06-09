## The History of Blockchain Wallets

```
When talking about cryptocurrency , you have to talk about blockchain wallet. Bitcoin has been created for 10 years, and the blockchain also has gone through 3 periods. At that time,the wallet develops from single-chain wallet to multi-chain wallet,and it also develops from a transfer-receive wallet to a blockchain ecological service platform.
```


### Blockchain 1.0 

**(From 2009-2013)**

In the year of 2009, Bitcoin Mainnet was set up. The blockchain had just started in this period. As a huge distributed ledger, bitcoin just has transfer and accounting functions.

The main function of the earliest wallet was to store bitcoin. That is to say,**<font color=#2980fe>only one kind of coin could be stored by a wallet during this period.</font>**

> On June 29th,2011, launched by BitPay, a new bitcoin e-wallet claimed to use in smartphones. On July 6th of the same year, a free App of bitcoin wallet was appeared in the android app store, which is the first smartphone App connects to bitcoin.


### Blockchain 2.0

**(From 2014-2018)**

In the year of 2014, Ethereum launched. It declared that the blockchain entered the 2.0 period. Smart contracts began to be used for blockchain.

> A smart contract is a computer program that can guarantee the execution of a contract without the need of a third party. Anyone can perform calculations and develop application layers based on this.  
> 
> At this time, the wallet not only could receive and transfer funds, but also perform contract operations on the chain. However, due to the slow speed at this time, the wallet can only provid non-transient response contract services.


### Blockchain 3.0

**(From 2018-Today)**


In the year of 2018, the blockchain entered the 3.0 period.The issues such as slow transfer speed and high miner fees are optimized. At this time, The high transfer speed and high scalability of the blockchain are realized, and the most representative blockchain is EOS

In addition to the basic storage and transfer functions, the wallet can also interact with the on-chain contracts in real time.Wallet is no longer a simple asset management tool, It becomes a public blockchain ecological service platform. At the same time, the single-chain wallet can not meet the user’s needs, **<font color=#2980fe>more and more wallets begin to develop multi-chain wallets.</font>**For example, TokenPocket wallet, supports assets on EOS, Bitcoin, Ethereum, TRON and IOST.

Nowadays, the functions of the wallet are no longer limited to store the cryptocurrencies. Users can create an account, manage and trade their assets, play DApps, get market information through the wallet.

The wallet has gradually assumed its role as the portal to the world of blockchain .


## The Basic Knowledge of Blockchain Wallets

```
To learn how to use a blockchain wallet, you must understand the five nouns : public key, private key, mnemonic, keystore and password.
```

### Public key

+ The public key is equivalent to your bank card number. It can be made public without any risk.

### Private key

+ The private key consists of numbers and uppercase and lowercase letters, the length of which is the same as that of the block chain private key.
Private key = bank card + password = identity authentication. The public key can be derived from the private key. It should be noted that once your private key is lost or forgotten, it cannot be retrieved again.


### mnemonic

+ Since the private key cannot be memorized, mnemonic words appear. The private key can be calculated by mnemonic words. In general, mnemonic words consist of some words. As long as you remember these single words and enter them in the wallet in sequence, you can recover the wallet and enter any operation. If someone gets your mnemonic, it is equivalent to getting your private key, that’s very dangerous.

### Keystore

+ The essence of Keystore is the encrypted private key. Keystore must be used with your wallet password to be valid. keystore = private key / mnemonic + password. 
Keystore, private key, mnemonic are common to all wallets, wallet service providers may only provide one or more of them due to product design.


### Password

+ In order to enhance the security, most wallets will use the password to encrypt the private key. The encryption method and storage method of each wallet are different. In order to get your authorization, you need to enter your password for each transaction, logic behind that is to decrypt your private keys and use it to sign a transaction.

### Wallet security tips

> + The public key can be disclosed without affecting the security of your assets.

> + Once the mnemonic, private key, and keystore are disclosed, the ownership of your asset will be controlled by others immediately. At this time, you need to transfer the asset to another address at once, and the original account cannot be used.

> + Once the keystore is disclosed, whether the password is exposed or not, there is a risk that others will control the asset, so you need to transfer the asset to another address immediately.

> + If the private key of EOSIO (including EOS, BOS, etc.) and IOST is disclosed, you can replace the private key to prevent others from controlling your own assets.

> +  When storing the private key and mnemonic, we recommend that you’d better use offline form (manual copying, printing, etc.) for data backup, and keep the backed up content properly. Writing down keystore as a term of backup could easily cause an error. Users are suggested to store the keystore as a file and then store carefully it in a USB flash drive. The methods such as screenshots, network transmission (Instagram, WeChat, WhatsApp) and cloud storage are highly objected which will bring hack and loss of your assets.


## The Sorts of Blockchain Wallets

```
We will classify the wallets from two dimensions: The generation of private keys and the storage of private keys.
```

### Storage of the Key

According to the method of private key storage, we divide wallets into**<font color=#2980fe>“centralized wallets”</font>及<font color=#2980fe>“decentralized wallets”</font>**。


Among them, the decentralized wallets can be divided into **<font color=#2980fe>cold wallets </font>**and **<font color=#2980fe>hot wallets</font>** according to the private key connect to the internet or not.

Hot wallets can be divided into desktop wallets, mobile wallets and web wallets.
Cold wallets keep the private key can’t be accessed by the network. Like paper wallet, brain wallet, hardware wallet, etc.

![Wallet category Sketch Map](https://tp-upload.cdn.bcebos.com/banner/tokenpocket-1591618729112.png "Wallet category")

Wallets can be divided into full-node wallets, light-node wallets and centralized wallets according to the maintenance mode of blockchain data and the level of decentralization of wallets.

Most of full-node wallets include desktop wallets, like Bitcoin-Core, Geth, Parity, etc. Such wallets need to synchronize all blockchain data, occupying a large storage space, but can be completely decentralized.
However, most mobile wallet and web wallet are light-node wallets. These wallets rely on other full-nodes in the blockchain network. They only synchronize their transaction data and can basically achieve decentralization.
The transaction data of the centralized wallet is stored in the blockchain, and all data is obtained from the server of the service provider. However, the transaction efficiency is very high and can be received in real time. For example, the account you registered in the exchanges is the centralized wallet.


![Node Wallet Sketch Map](https://tp-upload.cdn.bcebos.com/banner/tokenpocket-1591618876243.png "Node Wallet")


### Generation of the Key
**（The content of this section is slightly beyond the outline）**

From the generation of the private key, we can divide the wallet into "non-deterministic wallets", "deterministic wallets" and "hierarchical deterministic wallets", of which "hierarchy deterministic wallets" is an enhanced version of "deterministic wallets".


**<font color=#2980fe>Non-deterministic wallets:</font>**

The private keys generated in the wallet are independent of each other.

![Uncertainty Wallet Sketch Map](https://tp-statics.tokenpocket.pro/news/tokenpocket-1576070497680.png "Uncertainty Wallet")

**<font color=#2980fe>Deterministic wallets:</font>**

The private key is generated by a "seed" through algorithms, such as "mnemonic words". In this way, as long as the algorithm is consistent, the private key can be kept consistent, and one seed can derive unlimited private key addresses.

![Certainty Wallet Sketch Map](https://tp-statics.tokenpocket.pro/news/tokenpocket-1576070721576.png "Certainty Wallet")


**<font color=#2980fe>Hierarchy deterministic wallets:</font>**

It is an enhanced version of deterministic wallets, which introducing the concept of "master private key" for deterministic wallets, namely HD wallets. Its hierarchical structure is that the private key generated from the master private key can become a master private key, and then a deterministic wallet is generated by the above method.

![Layered deterministic Wallet Sketch Map](https://tp-statics.tokenpocket.pro/news/tokenpocket-1576070849616.png "Layered deterministic Wallet")


## The Functions of Blockchain Wallets

The wallet is the portal to the blockchain. It meets various needs of users with plenty of functions such as asset management.

### Create Accounts

Blockchain wallets are composed of addresses and account numbers, in order to make it easier, we call them as account. The account numbers of different blockchains are not the same, and their lengths may be different. The cost of creating a blockchain account is different, for example, creating an Ethereum or Bitcoin account is free, however, certain fee is asked to have an EOS account.

Since the creation of a blockchain account is generated by an algorithm, the process is very complicated. The existence of a wallet is to help users simplify these processes. For example, to register an ETH account in the TokenPocket wallet, you only need to set a password of not less than 8 digits, and perform a second confirmation to get an ETH account immediately. EOS accounts need to be created with EOS. In order to lower the threshold for users and allow newcomers without EOS to have EOS accounts quickly, TokenPocket uses an activation code to create an account. When users create an EOS account, they only need to purchase an activation code, then you can quickly have an EOS account.

For rookies, it may be too troublesome to master the private key. TokenPocket designed decentralized mobile phone number / email address for EOS account registration. This method supports users to retrieve private key through TP when they forget it, which greatly reduces the difficulty for users to use their wallets.

Of course, in order to meet the needs of users at different levels, TokenPocket also provides several methods such as “cold wallets, observation wallets, batch creation, contract creation and friend creation”to create an account.



### Assets Management

**<font color=#2980fe>Digital assets mainly refer to various tokens on the blockchain.</font>**The existence of wallets is extremely convenient for users to manage assets. It mainly includes transfers, receipts, viewing asset details, transaction details, etc. You can see the number and types of assets, and asset transfer operation.

> It should be noted that assets from different blockchains cannot be transferred directly. For example, Bitcoin to an Ethereum account is impossible.

### Assets Trading

The current wallet supports three types of digital asset transactions: token swap, token exchange, and OTC.

**<font color=#2980fe>Token Swap</font>**

Assets on different blockchains can be exchanged by Token Swap. For example, you can exchange your BTC (Bitcoin) into EOS.
> Usually trades happen on basic trading pair.
> like A to C,first is trade A to B by basic trading pair and then B to C.
> Token Swap can help to trade from A to C directly.  

**<font color=#2980fe>Token Exchange</font>**

Nowadays there are three types of exchanges :<font color=#2980fe>centralized exchanges, decentralized exchanges and mixed exchanges. </font> The centralized exchanges include Huobi, Binance, OKEX, etc. The decentralized exchanges include IDEX ( available on ETH), NewDex, Whale Exchange, and DEXEOS (available on EOS).

> First of all, we need to understand the process of trading. Generally speaking, users must first securely deposit assets in a certain place. Once there is a demand for trading, they will issue trading instructions. At this time, a place with sufficient liquidity is required for users to conduct match. After a suitable match is found, buyers and sellers enter into a transaction in a secure environment. At this time, certain restrictions need to be imposed objectively to prevent one party from cheating or bounced check. Finally, when the transaction is completed, the two parties settle the transaction.  
> The biggest difference between the two is that the centralized exchange requires us to deposit the currency in the exchange account, while the decentralized exchange deposits the currency to our own wallet. This greatly reduces the risk of loss of users’ assets due to theft or running of the exchange. 
> Through smart contracts, while improving transparency, it also greatly reduces the reliance on central media.


**<font color=#2980fe>Mixed Exchange</font>**

Mixed exchanges can aggregate all exchanges into a single exchange platform, which allowing users to cross-platform anytime without downloading many apps. Aggregation exchanges share the quoted depth and pair trading of other exchanges. For example, every time you buy or sell bitcoin in the mixed exchange, you can choose the best one with cost effective price from different exchanges.

> Decentralized wallets nowadays can support decentralized exchanges, and some of them support aggregated exchanges. TP wallet launched mixed exchange in December 2019.

**<font color=#2980fe>OTC</font>**

OTC (Over The Counter) is a peer-to-peer transaction which is guaranteed by a third party outside the exchange. OTC in the blockchain usually refers to the one-to-one transaction of fiat money and digital currency between OTC users.Currently,the largest OTC mainly based on exchanges, but some wallets also connected to the services of third-party channels.

> For example, TokenPocket wallet has connected to the OTC service of currency trading, when users use TP wallet, they can easily sell their digital currency into fiat money, or use fiat money to buy digital currency.

### Ecology Building

At present, in some public chain designs, users in the ecology are encouraged to participate in the public chain ecological construction. The main forms are **<font color=#2980fe>voting, referendum and staking.</font>**。

**<font color=#2980fe>voting</font>**  
Taking EOS as an example, EOS has 21 super nodes, and users can vote to 30 nodes(maximality) by staking EOS in their accounts. The purpose of voting is to allow users to choose nodes that can accelerate the development of the EOS ecosystem.

**<font color=#2980fe>referendum</font>**  
Referendum means that participants can initiate proposals that are good for the community. Holders of the entire blockchain can vote .When the number of votes exceeds a certain number, the proposal takes effect automatically. The referendum is beneficial to the participation of community users in blockchain governance.

**<font color=#2980fe>staking</font>**  
At present, some public chains encourage token holders to pledge token by staking,which will create stable nodes. For example, users can pledge COSMOS to obtain a certain amount of profit per year,it’s similar to the investment of a current account in a bank.

### Experience the DApp

At present, most wallets can support DApps . DApp is an abbreviation of Decentralized Application.

DApp is an application developed based on the underlying technology of the blockchain. Currently DApp is mainly concentrated on blockchains of Ethereum, EOS, TRON and IOST. The relationship between DApp and the underlying platform is similar to APP and IOS and Android systems.

That is to say, the DApp on EOS cannot run on ETH, just as APP on Android cannot run on IOS system. You can experience the decentralized integration of MakerDAO on ETH in your wallet, experience car driving in EOSRacing to get EOS in return. At present, some large-scale games are in the form of third-party APPs. When experiencing these DApps, you also need a wallet as a medium for logging in, operating, and authorization.

![DApp Store Sketch Map](https://tp-upload.cdn.bcebos.com/banner/tokenpocket-1591670818207.png "DApp Store")

> TokenPocket supports a number of popular games such as EOS Dynasty, EOSKnights, EOS Crypto Knights, Crypto Sword and Magic, XPET and so on. In order to avoid the tedious operation of users switching wallets, TP has developed the MiniWallet mode, which requires only one-time authorized operation and can always stay and have fun in the game.

### Ecology Claim Candy Rewards

The advantage of owning a wallet is that you can get candy from time to time (candy refers to the token obtained free on the blockchain). Common candy distribution methods are:**<font color=#2980fe>registration to get, free airdrop, advertising candy, Airgrab and mining airdrop etc.</font>**

> Candy refers to the token obtained free of charge on the blockchain

**<font color=#2980fe>registration to get：</font>**  
Registration to get: Usually at the early stage of the project, there are often free candy activities. As long as you register your blockchain address (such as ETH, EOS account, etc.) on the project's activity page, you can get it after waiting for the project to issue a reward of free candy.

**<font color=#2980fe>free airdrop：</font>**  
Airdrops for holding coins: There are two ways to hold airdrops for coins. One method is a forked coin. For example, BCH is forked from Bitcion, all users who held Bitcoin before the fork will receive the corresponding amount according to the qty of Bitcoin . Another is to directly issue another type of token to the holder, such as the first airdrop coin ADD on EOS. When the EOS mainnet is launched, a snapshot of the entire network account is taken, then distribute the candy to the account which is holding EOS.

**<font color=#2980fe>advertising candy：</font>**   
Advertising candy: At present, many projects will do small transactions to the holders for promoting their products. Their own advertisements can be seen in the transaction information.

> Ecology Claim Candy Rewards

![Airgrab Sketch Map](https://tp-upload.cdn.bcebos.com/banner/tokenpocket-1591671158041.png "Airgrab")

**<font color=#2980fe>Airgrab：</font>**  
 This is a way to distribute candy on EOS. Collecting tokens requires RAM of user’s account (each token needs about 0.25KB). You need to wait for the airdrop after executing.In TokenPocket wallet, an information integration page [Candy Airgrab] is specially created for Airgrab, and the candy currently available for collection is displayed in TokenPocket. Users only need to click the [AirGrab] button to complete the operation.

**<font color=#2980fe>Mining airdrop：</font>**  
Mining airdrop means that after the user sends a small amount of tokens to a contract account, the contract will return a certain amount of candy to the user at the same time as the original token is returned. The famous mining airdrop is EIDOS. Users only need to send 0.0001 EOS to the contract account, and the contract will return 0.0001 EOS while giving away 0.01% of the current remaining EIDOS of their contract account.

![Mining airdrop Sketch Map](https://tp-upload.cdn.bcebos.com/banner/tokenpocket-1591671277313.png "Mining airdrop")

Users can log in the decentralized exchange quickly in the wallet, you can exchange the receiving candy to ETH,EOS,USDT ect directly. That’s awesome.

### Assets Investment

Wallets naturally have features of financial properties. At present, wallets have integrated a variety of financial functions, including  **<font color=#2980fe>mining pools, financial management, DApp Mining, project investment, etc.</font>**These functions can meet the needs of users’ asset appreciation.

**<font color=#2980fe>Mining pool： </font>**  
At present, there are two main methods: POW mining and POS mining. 
Among them, POS can be subdivided into DPOS mining. POW is hashing power mining. The most famous POW mining we knew is BTC. 

> At present, the wallet pool is basically based on POS mining. POS (Proof of Stake) mining is to imitate POW to calculate mining. Holders can stake tokens to nodes to get reward dividends.

**<font color=#2980fe>Financial Management： </font>**  
Wallet's financial products are very similar with traditional financial products, the only difference is the way of settlement. Generally, an estimated rate of revenue will be agreed when users purchase this financial product with Token, regular settlements will happen per agreed date promised in advance,principal and profit can be retrieved or renewed at the expired time. TokenPocket will launch financial products of USDT soon. It is expected to an annual return of 12%. users with interests can follow our Twitter Official Account.

**<font color=#2980fe>DApp Mining： </font>**  
DApp mining products collected in wallets, which use the mining machine can quickly obtain Tokens. Taking EIDOS as an example, the EIDOS mining machine which developed by TokenPocket can help users transfer automatically. And the token from mining can be traded on exchanges to EOS.

**<font color=#2980fe>Project investment： </font>**  
Take HOO LABS as an example, you can use USDT to support the project on it, and according a certain ratio to get the token of the project based on the amount of USDT supported.

### Social


Some blockchain wallets have social functions. You can communicate with others in the wallet. In the chat interface of TokenPocket wallet, you can join different groups and talk freely with members. You can also hand out or receive digital currency red envelopes in chat groups.

Sense.Chat, which social function as the main function, allows users to chat freely with other members on the APP. All chat information is encrypted, and only you and the contact can decrypt the information. In addition, MIXIN is also a wallet with chat as its main function.

Trybe is a social network and media publishing community inspired by digital currency where users can create great content. Comment on others’ works or invite friends, you can get the digital currency sent by Trybe.


### Hardware wallet Tool kit

A hardware wallet is usually paired with a software wallet as a management tool. Hardware wallet companies such as Ledger, Trezor, ColdLar, YubiKey, etc., have developed their own software wallets.

Similarly, software wallet companies will also cooperate with hardware wallet companies to develop their own dedicated hardware wallets, such as imToken and imKey.

### Access the Blockchain News

Most of the wallet users have trading needs, so wallets usually add token price in it. In addition,modules such as newsletters, articles, and twitters will be added to the product.

Taking the TokenPocket wallet as an example, it builds a dedicated page for the information of decentralized exchanges. Users don’t need to enter the exchange, they can get token price conveniently. The wallet also has a special function to jump to the exchages quickly.

Unlike other blockchain media, the newsletters and articles in TokenPocket are mainly based on the currently blockchain of the wallet, which is more targeted.


## How to Choose a Blockchain Wallet

```
Firstly, we need to know the differences between centralized wallets and decentralized wallets,  then we can make a choice based on our own needs.
```


| **Centralized wallets**                                                                                                                 | **Decentralized wallets**                                         |
| --------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| The private key is held by the platform                                                                                                 | The private key is held by users                                  |
| Assets are stored in the wallet of the platform                                                                                         | Assets are stored in users' wallet                                |
| Password can be retrieved                                                                                                               | Password can NOT be retrieved                                     |
| The platform need audit the transfer                                                                                                    | The platform don’t need to audit the transfer                     |
| Centralized account is NOT available on the wallet platforms                                                                            | Decentralized account is available on all of the wallet platforms |
| No fees for internal platform transfers;                                                                                                | Asset transfer only pays for blockchain network                   |
| Fees for withdrawal of assets.                                                                                                          |
| The risks of the platform lost coins:                                                                                                   |
| The platform wallet was hacked, the service was attacked, the platform was closed (the wallet service was closed), the platform cheats. | The risks of the wallets lost coins:                              |
Private key leaks or being forgotten, private keys are not backed up, wallet-installed devices are lost (mobile phones, computers), and wallets are infected with viruses.

 

## The Directory of Blockchain Walle

### Decentralized wallets

<!-- 1 -->

<main class="tp-main">
<!-- TokenPocket -->
<a class="tp-custom" href="https://www.tokenpocket.pro" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/TokenPocket.png"/>
    <div class="tp-content">
        <h5>TokenPocket</h5>
        <p>https://www.tokenpocket.pro</p>
    </div>
</a>


<!-- Trust Wallet -->
<a class="tp-custom" href="https://www.trustwallet.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/TrustWallet.png"/>
    <div class="tp-content">
        <h5>Trust Wallet</h5>
        <p>https://www.trustwallet.com</p>
    </div>
</a>
</main>

</main>

<!-- 2 -->

<main class="tp-main">
<!-- Bitpie -->
<a class="tp-custom" href="https://bitpie.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Bitpie.png"/>
    <div class="tp-content">
        <h5>Bitpie</h5>
        <p>https://bitpie.com</p>
    </div>
</a>


<!-- imToken -->
<a class="tp-custom" href="https://token.im" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/ImToken.png"/>
    <div class="tp-content">
        <h5>imToken</h5>
        <p>https://token.im</p>
    </div>
</a>
</main>

<!-- 3 -->

<main class="tp-main">
<!-- Huobi -->
<a class="tp-custom" href="https://www.huobiwallet.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/HuobiWallet.png"/>
    <div class="tp-content">
        <h5>Huobi Wallet</h5>
        <p>https://www.huobiwallet.com</p>
    </div>
</a>


<!-- AToken -->
<a class="tp-custom" href="https://www.atoken.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/AToken.png"/>
    <div class="tp-content">
        <h5>AToken</h5>
        <p>https://www.atoken.com</p>
    </div>
</a>
</main>

<!-- 4 -->

<main class="tp-main">
<!-- BPEAL Wallet -->
<a class="tp-custom" href="https://www.bepal.pro" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/BPEALWallet.png"/>
    <div class="tp-content">
        <h5>BPEAL Wallet</h5>
        <p>https://www.bepal.pro</p>
    </div>
</a>


<!-- Starteos -->
<a class="tp-custom" href="https://www.starteos.io" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Starteos.png"/>
    <div class="tp-content">
        <h5>Starteos</h5>
        <p>https://www.starteos.io</p>
    </div>
</a>
</main>

<!-- 5 -->

<main class="tp-main">
<!-- BitKeep -->
<a class="tp-custom" href="https://www.bitkeep.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Bitkeep.png"/>
    <div class="tp-content">
        <h5>BitKeep</h5>
        <p>https://www.bitkeep.com</p>
    </div>
</a>


<!-- MEET.ONE -->
<a class="tp-custom" href="https://www.meet.one" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Meetone.png"/>
    <div class="tp-content">
        <h5>MEET.ONE</h5>
        <p>https://www.meet.one</p>
    </div>
</a>
</main>

<!-- 6 -->

<main class="tp-main">
<!-- Tronlink -->
<a class="tp-custom" href="https://www.tronlink.org" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Tronlink.png"/>
    <div class="tp-content">
        <h5>Tronlink</h5>
        <p>https://www.tronlink.org</p>
    </div>
</a>


<!-- Lynx -->
<a class="tp-custom" href="https://lynxwallet.io" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Lynx.png"/>
    <div class="tp-content">
        <h5>Lynx</h5>
        <p>https://lynxwallet.io</p>
    </div>
</a>
</main>

<!-- 7 -->

<main class="tp-main">
<!-- Scatter -->
<a class="tp-custom" href="https://get-scatter.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/scatter.png"/>
    <div class="tp-content">
        <h5>Scatter</h5>
        <p>https://get-scatter.com</p>
    </div>
</a>


<!-- MetaMask -->
<a class="tp-custom" href="https://metamask.io" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/MetaMask.png"/>
    <div class="tp-content">
        <h5>MetaMask</h5>
        <p>https://metamask.io</p>
    </div>
</a>
</main>

<!-- 8 -->

<main class="tp-main">
<!-- ENJIN Wallet -->
<a class="tp-custom" href="https://enjin.io/products/wallet" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/ENJINWallet.png"/>
    <div class="tp-content">
        <h5>ENJIN Wallet</h5>
        <p>https://enjin.io/products/wallet</p>
    </div>
</a>


<!-- jaxx wallet -->
<a class="tp-custom" href="https://jaxx.io" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/JaxxWallet.png"/>
    <div class="tp-content">
        <h5>jaxx wallet</h5>
        <p>https://jaxx.io</p>
    </div>
</a>
</main>

<!-- 9 -->
<main class="tp-main">
<!-- 块信 -->
<a class="tp-custom" href="https://chattle.vip/#/" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/dapp/tokenpocket-1576249499924.png"/ width=50>
    <div class="tp-content">
        <h5>块信</h5>
        <p>https://chattle.vip</p>
    </div>
</a>


<!-- KCASH -->
<a class="tp-custom" href="https://www.kcash.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/KCASH.png"/>
    <div class="tp-content">
        <h5>KCASH</h5>
        <p>https://www.kcash.com</p>
    </div>
</a>
</main>


<!-- 10 -->
<main class="tp-main">
<!-- Conibase Wallet -->
<a class="tp-custom" href="https://www.coinbase.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/ConibaseWallet.png"/>
    <div class="tp-content">
        <h5>Coinbase Wallet</h5>
        <p>https://www.coinbase.com</p>
    </div>
</a>

<!-- KCASH -->
<a class="tp-custom" style="border:none" target="_blank">
    <!-- <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/KCASH.png"/>
    <div class="tp-content">
        <h5>KCASH</h5>
        <p>https://www.kcash.com</p>
    </div> -->
</a>
</main>

### Centralized wallets

<!-- 1 -->

<main class="tp-main">
<!-- 币信 -->
<a class="tp-custom" href="https://bixin.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/bixin.png"/>
    <div class="tp-content">
        <h5>币信</h5>
        <p>https://bixin.com</p>
    </div>
</a>


<!-- Edge -->
<a class="tp-custom" href="https://edge.app" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Edge.png"/>
    <div class="tp-content">
        <h5>Edge</h5>
        <p>https://edge.app</p>
    </div>
</a>
</main>

<!-- 2 -->

<main class="tp-main">


<!-- Uphold -->
<a class="tp-custom" href="https://uphold.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Uphold.png"/>
    <div class="tp-content">
        <h5>Uphold</h5>
        <p>https://uphold.com</p>
    </div>
</a>

<!-- Conibase Wallet -->
<a class="tp-custom" style="border:none">
    <!-- <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/ConibaseWallet.png"/>
    <div class="tp-content">
        <h5>Conibase Wallet</h5>
        <p>https://www.coinbase.com</p> -->
    <!-- </div> -->
</a>

</main>

### Hardware wallets

<!-- 1 -->

<main class="tp-main">
<!-- Ledger -->
<a class="tp-custom" href="https://www.ledger.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Ledger.png"/>
    <div class="tp-content">
        <h5>Ledger</h5>
        <p>https://www.ledger.com</p>
    </div>
</a>


<!-- Trezor -->
<a class="tp-custom" href="https://www.trezor.io" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Trezor.png"/>
    <div class="tp-content">
        <h5>Trezor</h5>
        <p>https://www.trezor.io</p>
    </div>
</a>
</main>

<!-- 2 -->

<main class="tp-main">
<!-- keep key -->
<a class="tp-custom" href="https://shapeshift.io/keepkey" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/keepkey.png"/>
    <div class="tp-content">
        <h5>keep key</h5>
        <p>https://shapeshift.io/keepkey</p>
    </div>
</a>


<!-- 库神(ColdLar） -->
<a class="tp-custom" href="https://www.coldlar.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/ColdLar.png"/>
    <div class="tp-content">
        <h5>库神(ColdLar）</h5>
        <p>https://www.coldlar.com</p>
    </div>
</a>
</main>

<!-- 3 -->

<main class="tp-main">
<!-- 比特护盾（BITHD) -->
<a class="tp-custom" href="https://bithd.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/BITHD.png"/>
    <div class="tp-content">
        <h5>比特护盾（BITHD)</h5>
        <p>https://bithd.com</p>
    </div>
</a>


<!-- imKey -->
<a class="tp-custom" href="https://imkey.im" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/imKey.png"/>
    <div class="tp-content">
        <h5>imKey</h5>
        <p>https://imkey.im</p>
    </div>
</a>
</main>

<!-- 4 -->

<main class="tp-main">
<!-- Cobo金库 -->
<a class="tp-custom" href="https://cobo.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Cobo.png"/>
    <div class="tp-content">
        <h5>Cobo金库</h5>
        <p>https://cobo.com</p>
    </div>
</a>


<!-- BEPAL Pro S -->
<a class="tp-custom" href="https://www.bepal.pro/bepal-q" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/BEPALProS.png"/>
    <div class="tp-content">
        <h5>BEPAL Pro S</h5>
        <p>https://www.bepal.pro/bepal-q</p>
    </div>
</a>
</main>

<!-- 5 -->

<main class="tp-main">
<!-- 华特钱包 -->
<a class="tp-custom" href="https://www.orientwalt.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/orientwalt.png"/>
    <div class="tp-content">
        <h5>华特钱包</h5>
        <p>https://www.orientwalt.com</p>
    </div>
</a>


<!-- SafePal-->
<a class="tp-custom" href="https://safepal.io/" target="_blank">
    <img class="tp-logo" width=50 src="https://tp-statics.tokenpocket.pro/dapp/tokenpocket-1576591843263.png"/>
    <div class="tp-content">
        <h5>SafePal</h5>
        <p>https://safepal.io/</p>
    </div>
</a>
</main>



### Centralized wallets & Decentralized wallets

<!-- 1 -->

<main class="tp-main">
<!-- Cobo -->
<a class="tp-custom" href="https://cobo.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Cobo.png"/>
    <div class="tp-content">
        <h5>Cobo</h5>
        <p>https://cobo.com</p>
    </div>
</a>


<!-- 库神 -->
<a class="tp-custom" href="https://www.coldlar.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/ColdLar.png"/>
    <div class="tp-content">
        <h5>库神</h5>
        <p>https://www.coldlar.com</p>
    </div>
</a>
</main>

<!-- 2 -->

<main class="tp-main">
<!-- 虎符 -->
<a class="tp-custom" href="https://hoo.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Hoo.png"/>
    <div class="tp-content">
        <h5>虎符</h5>
        <p>https://hoo.com</p>
    </div>
</a>


<!-- RenrenBit -->
<a class="tp-custom" href="https://www.renrenbit.com" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Renrenbit.png"/>
    <div class="tp-content">
        <h5>RenrenBit</h5>
        <p>https://www.renrenbit.com</p>
    </div>
</a>
</main>

<!-- 3 -->

<main class="tp-main">
<!-- HyperPay -->
<a class="tp-custom" href="http://www.hyperpay.tech" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/Hyperpay.png"/>
    <div class="tp-content">
        <h5>HyperPay</h5>
        <p>http://www.hyperpay.tech</p>
    </div>
</a>


<!-- Math Wallet -->
<a class="tp-custom" href="http://www.mathwallet.org" target="_blank">
    <img class="tp-logo" src="https://tp-statics.tokenpocket.pro/logo/MathWallet.png"/>
    <div class="tp-content">
        <h5>Math Wallet</h5>
        <p>http://www.mathwallet.org</p>
    </div>
</a>
</main>

## The Guide of Blockchain Wallets

The following questions are posted on the official website help center in TokenPocket wallet.
URL:
https://help.mytokenpocket.vip/hc/zh-cn


<img src="https://gz.bcebos.com/v1/tp-statics/logo/QA-code.jpg" width="250">

### BTC (bitcoin) wallet problems

1.[How to create BTC bitcoin Wallet](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037208612-%E5%9C%A8TokenPocket%E5%A6%82%E4%BD%95%E5%88%9B%E5%BB%BABTC%E9%92%B1%E5%8C%85-)

2.[How to back up BTC bitcoin private key](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037208872-%E5%A6%82%E4%BD%95%E5%A4%87%E4%BB%BDBTC%E6%AF%94%E7%89%B9%E5%B8%81%E7%A7%81%E9%92%A5-)

3.[BTC比特币私钥丢了怎么办](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037208972-BTC%E7%A7%81%E9%92%A5%E4%B8%A2%E4%BA%86%E6%80%8E%E4%B9%88%E5%8A%9E-)

4.[What to do if the BTC bitcoin private key is lost](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037209032-%E5%A6%82%E4%BD%95%E9%87%8D%E7%BD%AEBTC%E9%92%B1%E5%8C%85%E5%AF%86%E7%A0%81-)

5.[How to import BTC bitcoin private key into Wallet](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037211032-%E5%A6%82%E4%BD%95%E5%B0%86btc%E7%A7%81%E9%92%A5%E5%AF%BC%E5%85%A5%E9%92%B1%E5%8C%85-)

6.[How to transfer BTC bitcoin to exchange with wallet](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037209852-%E5%A6%82%E4%BD%95%E7%94%A8%E9%92%B1%E5%8C%85%E6%8A%8Abtc%E8%BD%AC%E5%85%A5%E4%BA%A4%E6%98%93%E6%89%80-)

7.[How to set BTC bitcoin miner fee](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037576691-%E5%A6%82%E4%BD%95%E8%AE%BE%E7%BD%AEbtc%E7%9A%84%E7%9F%BF%E5%B7%A5%E8%B4%B9-)

8.[Can BTC bitcoin transfer speed up?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037211172-BTC%E6%AF%94%E7%89%B9%E5%B8%81%E8%BD%AC%E8%B4%A6%E6%85%A2%E5%8F%AF%E4%BB%A5%E5%8A%A0%E9%80%9F%E5%90%97)

9.[What is BTC isolation witness?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037362692-%E4%BB%80%E4%B9%88%E6%98%AFBTC%E9%9A%94%E7%A6%BB%E8%A7%81%E8%AF%81-)

10.[What is bitcoin proof of work (POW)?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037363992-BTC%E6%AF%94%E7%89%B9%E5%B8%81%E7%9A%84%E5%B7%A5%E4%BD%9C%E9%87%8F%E8%AF%81%E6%98%8E-POW-%E6%98%AF%E4%BB%80%E4%B9%88-)

[Click to see more](https://help.mytokenpocket.vip/hc/zh-cn/sections/360007340872-%E6%AF%94%E7%89%B9%E5%B8%81-BTC-%E9%92%B1%E5%8C%85%E5%B8%B8%E8%A7%81%E9%97%AE%E9%A2%98)

### Eth wallet problems

1.[How to create eth Wallet](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037514271-%E5%A6%82%E4%BD%95%E5%88%9B%E5%BB%BAETH%E9%92%B1%E5%8C%85-)

2.[How to retrieve the previous eth Wallet](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037151792-%E5%A6%82%E4%BD%95%E6%89%BE%E5%9B%9E%E4%B9%8B%E5%89%8D%E7%9A%84ETH%E9%92%B1%E5%8C%85-)

3.[How to purchase eth assets](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037152332-%E6%80%8E%E6%A0%B7%E8%B4%AD%E4%B9%B0ETH%E8%B5%84%E4%BA%A7-)

4.[How to recharge eth to Wallet](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037153092-%E6%80%8E%E6%A0%B7%E5%85%85%E5%80%BCETH%E5%88%B0%E9%92%B1%E5%8C%85-)

5.[How to sell eth in wallet for cash](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037153552-%E9%92%B1%E5%8C%85%E9%87%8C%E7%9A%84ETH%E5%A6%82%E4%BD%95%E5%8D%96%E5%87%BA%E5%8F%98%E7%8E%B0-)

6.[What about the ETH transfer record?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037153712-ETH%E8%BD%AC%E8%B4%A6%E8%AE%B0%E5%BD%95%E6%80%8E%E4%B9%88%E7%9C%8B-)

7.[How to transfer / collect eth from others?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037516471-%E6%80%8E%E4%B9%88%E5%90%91%E4%BB%96%E4%BA%BA%E8%BD%AC%E8%B4%A6-%E6%94%B6%E5%8F%96ETH-)

8.[What do you mean by the service charge and gas charge of eth transfer?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037516511-ETH%E8%BD%AC%E8%B4%A6%E7%9A%84%E6%89%8B%E7%BB%AD%E8%B4%B9%E5%92%8Cgas%E8%B4%B9%E6%98%AF%E4%BB%80%E4%B9%88%E6%84%8F%E6%80%9D-)

9.[Can eth wallets created from tokenpocket wallets be transferred to other wallets?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037516591-%E5%A6%82%E4%BD%95%E5%BE%80%E9%92%B1%E5%8C%85%E5%85%85%E5%80%BC%E5%9F%BA%E4%BA%8EETH%E5%85%AC%E9%93%BE%E7%9A%84%E5%85%B6%E4%BB%96Token-)

10.[How to recharge other currencies based on eth public chain?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037516591-%E5%A6%82%E4%BD%95%E5%BE%80%E9%92%B1%E5%8C%85%E5%85%85%E5%80%BC%E5%9F%BA%E4%BA%8EETH%E5%85%AC%E9%93%BE%E7%9A%84%E5%85%B6%E4%BB%96Token-)

[Click to see more](https://help.mytokenpocket.vip/hc/zh-cn/sections/360007354652-ETH-%E4%BB%A5%E5%A4%AA%E5%9D%8A-%E9%92%B1%E5%8C%85%E5%B8%B8%E8%A7%81%E9%97%AE%E9%A2%98)

### EOS (grapefruit) wallet problems

1.[How to get EOS grapefruit?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037250532-%E5%A6%82%E4%BD%95%E5%9C%A8TokenPocket%E9%92%B1%E5%8C%85%E8%B4%AD%E4%B9%B0EOS-)

2.[How to retrieve EOS from exchange to Wallet](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037250712-%E5%A6%82%E4%BD%95%E4%BB%8E%E4%BA%A4%E6%98%93%E6%89%80%E6%8F%90%E5%8F%96EOS%E5%88%B0TokenPocket%E9%92%B1%E5%8C%85-)

3.[How to register an EOS account](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037250892-%E5%A6%82%E4%BD%95%E6%B3%A8%E5%86%8CEOS%E8%B4%A6%E5%8F%B7)

4.[How to transfer and collect EOS](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037620971-%E5%A6%82%E4%BD%95%E8%BF%9B%E8%A1%8CEOS%E7%9A%84%E8%BD%AC%E8%B4%A6-%E6%94%B6%E6%AC%BE-)

5.[What are the resources of EOS? What does RAM (memory) CPU (network resource) net (computing resource) mean?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037623871-EOS%E7%9A%84%E8%B5%84%E6%BA%90%E5%8F%88%E5%93%AA%E4%BA%9B-RAM-%E5%86%85%E5%AD%98-cpu-%E7%BD%91%E7%BB%9C%E8%B5%84%E6%BA%90-net-%E8%AE%A1%E7%AE%97%E8%B5%84%E6%BA%90-%E6%98%AF%E4%BB%80%E4%B9%88%E6%84%8F%E6%80%9D-)

6.[Accidentally uninstalled the tokenpocketapp, and the private key was not saved. Can it be retrieved?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037254452-%E4%B8%8D%E5%B0%8F%E5%BF%83%E6%8A%8ATokenPocket-APP%E5%8D%B8%E8%BD%BD%E4%BA%86-%E7%A7%81%E9%92%A5%E4%B9%9F%E6%B2%A1%E4%BF%9D%E5%AD%98%E8%83%BD%E5%90%A6%E6%89%BE%E5%9B%9E-)

7.[Is there a service charge for EOS transfer?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037505611-EOS%E8%BD%AC%E8%B4%A6%E6%9C%89%E6%89%8B%E7%BB%AD%E8%B4%B9%E5%90%97-)

8.[How do I back up the EOS private key?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037505551-%E5%A6%82%E4%BD%95%E5%A4%87%E4%BB%BDEOS%E7%A7%81%E9%92%A5)

9.[How to use EOS observation mode?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037505191-TokenPocke%E9%92%B1%E5%8C%85%E4%B8%AD-%E5%A6%82%E4%BD%95%E4%BD%BF%E7%94%A8EOS%E8%A7%82%E5%AF%9F%E6%A8%A1%E5%BC%8F)

10.[What happens when there is no CPU? How to use the smooth mode of tokenpokcet?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037255072-%E6%B2%A1%E6%9C%89CPU%E7%9A%84%E6%97%B6%E5%80%99%E6%80%8E%E4%B9%88%E5%8A%9E-TokenPokcet%E7%9A%84%E9%A1%BA%E7%95%85%E6%A8%A1%E5%BC%8F%E5%A6%82%E4%BD%95%E4%BD%BF%E7%94%A8-)

[Click to see more](https://help.mytokenpocket.vip/hc/zh-cn/sections/360007442911-EOS%E9%92%B1%E5%8C%85%E5%B8%B8%E8%A7%81%E9%97%AE%E9%A2%98)

### Common problems of Tron Wallet

1.[How to obtain TRX wave field?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037354052-%E5%A6%82%E4%BD%95%E8%8E%B7%E5%BE%97TRX%E6%B3%A2%E5%9C%BA-)

2.[How to retrieve TRX from exchange to wallet?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037725931-%E5%A6%82%E4%BD%95%E4%BB%8E%E4%BA%A4%E6%98%93%E6%89%80%E6%8F%90%E5%8F%96TRX%E5%88%B0%E9%92%B1%E5%8C%85-)

3.[How to register and import TRX account?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037354672-%E5%A6%82%E4%BD%95%E6%B3%A8%E5%86%8C%E5%8F%8A%E5%AF%BC%E5%85%A5TRX%E8%B4%A6%E5%8F%B7-)

4.[How to transfer and collect TRX?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037726591-%E5%A6%82%E4%BD%95%E8%BF%9B%E8%A1%8CTRX%E7%9A%84%E8%BD%AC%E8%B4%A6-%E6%94%B6%E6%AC%BE-)

5.[What do you mean by broadband and energy in the wave field?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037730011-%E6%B3%A2%E5%9C%BA%E4%B8%8A%E7%9A%84%E5%AE%BD%E5%B8%A6-%E8%83%BD%E9%87%8F%E6%98%AF%E4%BB%80%E4%B9%88%E6%84%8F%E6%80%9D-)

6.[How to freeze and unfreeze resources in wave field?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037726871-%E6%B3%A2%E5%9C%BA%E4%B8%8A%E8%B5%84%E6%BA%90%E5%86%BB%E7%BB%93%E5%92%8C%E8%A7%A3%E5%86%BB%E5%A6%82%E4%BD%95%E6%93%8D%E4%BD%9C-)

7.[How to play DAPP on the wave field?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037355372-%E5%A6%82%E4%BD%95%E7%8E%A9%E6%B3%A2%E5%9C%BA%E4%B8%8A%E7%9A%84DApp-)

8.[How to backup the wave wallet?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037358892-%E6%B3%A2%E5%9C%BA%E9%92%B1%E5%8C%85%E5%A6%82%E4%BD%95%E8%BF%9B%E8%A1%8C%E5%A4%87%E4%BB%BD-)

9.[What to do when there is no energy?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037358952-%E6%B2%A1%E6%9C%89%E8%83%BD%E9%87%8F%E5%92%8C%E5%AE%BD%E5%B8%A6%E7%9A%84%E6%97%B6%E5%80%99%E6%80%8E%E4%B9%88%E5%8A%9E-)

10.[How to conduct wave voting?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037359032-%E5%A6%82%E4%BD%95%E8%BF%9B%E8%A1%8C%E6%B3%A2%E5%9C%BA%E6%8A%95%E7%A5%A8-)

[Click to see more](https://help.mytokenpocket.vip/hc/zh-cn/sections/360007395352-Tron-%E6%B3%A2%E5%9C%BA-%E9%92%B1%E5%8C%85%E5%B8%B8%E8%A7%81%E9%97%AE%E9%A2%98)


### IOST wallet problems

1.[How to create an Iost account?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037990432-%E5%A6%82%E4%BD%95%E5%88%9B%E5%BB%BAIOST%E8%B4%A6%E5%8F%B7-)

2.[How to transfer the Iost of the exchange to the wallet account?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037990332-%E5%A6%82%E4%BD%95%E6%8A%8A%E4%BA%A4%E6%98%93%E6%89%80%E7%9A%84IOST%E6%8F%90%E5%B8%81%E5%88%B0%E9%92%B1%E5%8C%85%E8%B4%A6%E6%88%B7-)

3.[How to import the previous Iost account?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360038358591-%E5%A6%82%E4%BD%95%E5%AF%BC%E5%85%A5%E4%B9%8B%E5%89%8D%E7%9A%84IOST%E8%B4%A6%E5%8F%B7-)

4.[How to collect Iost?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360040722751-IOST%E9%92%B1%E5%8C%85%E7%9A%84%E6%94%B6%E6%AC%BE)

5.[How to transfer the Iost Wallet](https://help.mytokenpocket.vip/hc/zh-cn/articles/360040721791-IOST%E9%92%B1%E5%8C%85%E5%A6%82%E4%BD%95%E8%BD%AC%E8%B4%A6)

6.[What are the resources of the Iost account?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360038358491-IOST%E8%B4%A6%E5%8F%B7%E7%9A%84%E8%B5%84%E6%BA%90%E6%98%AF%E4%BB%80%E4%B9%88-)

7.[How can Iost mortgage / redeem resources?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037990292-IOST%E6%80%8E%E4%B9%88%E6%8A%B5%E6%8A%BC-%E8%B5%8E%E5%9B%9E%E8%B5%84%E6%BA%90-)

8.[How to play DAPP app on Iost?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037990272-%E5%A6%82%E4%BD%95%E7%8E%A9IOST%E4%B8%8A%E7%9A%84Dapp%E5%BA%94%E7%94%A8-)

9.[How to vote for Iost?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360038358451-%E5%A6%82%E4%BD%95%E8%BF%9B%E8%A1%8CIOST%E6%8A%95%E7%A5%A8-)

10.[How to view the detailed block record of Iost transfer?](https://help.mytokenpocket.vip/hc/zh-cn/articles/360037990072-%E5%A6%82%E4%BD%95%E6%9F%A5%E7%9C%8BIOST%E8%BD%AC%E8%B4%A6%E7%9A%84%E8%AF%A6%E7%BB%86%E5%8C%BA%E5%9D%97%E8%AE%B0%E5%BD%95-)

[Click to see more](https://help.mytokenpocket.vip/hc/zh-cn/sections/360007631251-IOST-%E5%B8%B8%E8%A7%81%E9%97%AE%E9%A2%98)




## Blockchain wallet knowledge self test


```
It's time for self-test. Here are 100 Tips

Can you answer the question of blockchain wallet correctly?
```


<div class="ask-code">
<div>Scan code self test</div>
<img src="https://tp-statics.tokenpocket.pro/dapp/tokenpocket-1576248895145.jpeg" width="250">
</div>

<!-- <img src="https://tp-statics.tokenpocket.pro/news/tokenpocket-1576125777304.png" width="250"> -->
<!-- ![](https://tp-statics.tokenpocket.pro/news/tokenpocket-1576125777304.png) -->


**Business wechat：laurali0815**

**Official account:** TokenPocket wallet

**Telegram：** https://t.me/tokenPocket_en

**Twitter：** https://twitter.com/TokenPocket_TP

**Medium：** https://medium.com/@tokenpocket.gm

**Facebook：** [http://www.facebook.com/TokenPocket/](http://www.facebook.com/TokenPocket/)

**Github：** https://github.com/TP-Lab

**Email ：** service@tokenpocket.pro


### Copyright notice

#### "Blockchain wallet from introduction to Mastery", also known as wallet Xiaobai book. Edited by Marcus, the co-founder of tokenpocket wallet, it covers the development history, function and classification of wallet, and is one of the most detailed popular science materials of digital wallet on the market. Marcus, graduated from South China University of technology, co-founder and CMO of token Pocket Wallet, led the development of token pocket wallet from 0 to millions of users in one year. The former senior development engineer of Xunlei was employed as the market consultant of hashed labs, a well-known block chain investment institution in South Korea in 2019.

##### 1.This article is copyrighted by tokenpocket.

##### 2.With the consent of the author, the work is allowed to be quoted for non-profit, and the source and the author shall be indicated, so as to respect the work achievements of the author.

##### 3.出处：https://tp-lab.github.io/BlockchainGuideSeries/#/  作者：TokenPocket。

##### 4.No reprinting without permission. Tokenpocket and the author / translator reserve the right to pursue illegal reprints by legal means.

##### 5.For this article and this statement, as well as its modification right, renewal right and final interpretation right, all belong to tokenpocket.

##### 6."Tokenpocket" reserves the right to interpret the above statement.
