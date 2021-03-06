{
"title" : "How to Access Your Wallet with Mnemonic Phrase",
"sort" : "15",
"category" : "Accessing your Wallet",
"description" : "Accessing your Wallet",
"date_published" : "2017-06-20T08:00:00+08:00",
"date_modified"  : "2018-11-28T08:00:00+08:00"
}

---%

## Important Information

We do not recommend that you access your wallet via Mnemonic Phrase.

**Why?**

Mnemonic Phrases are vulnerable for two reasons:
1. Theft
    * To use a Mnemonic phrase means you need to either physically type it into the website or copy & paste to access the wallet. If you enter this information into a fake phishing website, your funds **WILL BE STOLEN**
2. Not recoverable if Lost or Forgotten
    * MyCrypto does not store any information. We only have access to information that is publicly available on the blockchain. Hardware wallets at least give you a chance to restore your wallet if you lose the device using the 12-word seed phrase if you have backed it up correctly.
    * If you forget the Mnemonic Phrase or lose the file where you saved it, there is almost no guarantee that you will ever gain access back to the wallet

### Accessing your Wallet

We no longer allow accessing your mnemonic phrase using the MyCrypto.com website, instead, you have to download the [MyCrypto desktop app](https://download.mycrypto.com/). A more detailed explanation on why we decided for this change can be found [here](https://medium.com/mycrypto/a-safer-mycrypto-79d65196e7d8).

1. Follow our guide on [running MyCrypto offline and locally](https://support.mycrypto.com/offline/running-mycrypto-locally.html).
2. Open the MyCrypto desktop application.
3. The "View & Send" tab will appear, click "Mnemonic Phrase".
4. Enter your 12-word phrase. If you entered a password when you created the wallet, enter that as well. Failure to do so can change the list of addresses that you can access. 
5. Click "Choose address" and your list of wallets will show up.


### Side Note
You can share your public wallet address with others so they can send you Ethereum or ERC-20 tokens. Your account will not be compromised, just make sure to send them your PUBLIC wallet address and not your private key.

**TIP**: If you are planning on sending a large amount of ETH to any wallet, we recommend that you first send a small amount to test first before depositing a large amount.

You only need your address in order to see your balance. **Do not** enter your private key anywhere if you just want to check the balance or see incoming and outgoing transactions.

Instead, search your address (or bookmark it) on [etherscan.io](https://etherscan.io) or [etherchain.org](https://www.etherchain.org/).

While you are at it, you should bookmark [https://mycrypto.com/account](https://mycrypto.com/account) as well.

MyCrypto is a client-side wallet, which means you hold your own keys. If someone gets your private key (keystore file, mnemonic, passwords), they have complete access to your funds. There are no stopping transactions, canceling transactions, or resetting passwords. Once a transaction is on the blockchain, it is final.

For this reason, it is very, very important to keep your private key a secret and use it as rarely as possible. Only enter it on sites after double-checking to be sure you are on the correct site.

### Related Reading

* [Backing up your wallet](https://support.mycrypto.com/getting-started/backing-up-your-new-wallet.html)

* [Sending & Receiving](https://support.mycrypto.com/send/)

* [Protecting Yourself and Your Funds](https://support.mycrypto.com/getting-started/protecting-yourself-and-your-funds.html)

* [Difference between an exchange and MyCrypto](https://support.mycrypto.com/getting-started/whats-the-difference-between-an-exchange-and-mycrypto.html)
