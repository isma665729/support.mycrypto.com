{
"title"       : "Running MyCrypto w/ your own, personal node",
"sort"        : "08",
"category"    : "Networks & Nodes",
"description" : "Networks & Nodes",
"date_published" : "2017-07-05T08:00:00+08:00",
"date_modified" : "2018-11-29T08:00:00+08:00"
}

---%


You can use MyCrypto to connect to your own node. This decouples the frontend and features that you love about MyCrypto from our backend infrastructure. This means more nodes send more transactions and is closer to the decentralized nature of Ethereum. It also means that you fully control the entire process and don't rely on us.

### Warning

When connecting to your own node, please do not have any accounts in that node. Meaning: do not do things like `geth account add` or store your private keys in the geth keystore folder.

You will be using MyCrypto to sign and then broadcast the TXs via your node. You will **not** be using your node to sign and send. [If you do not heed this warning, bad things *could* happen if another setting gets changed. Here's one.](https://www.reddit.com/r/ethereum/comments/3itz1f/insecurely_configured_geth_with_no_firewall_and/). Better safe than sorry.


### Specifics to Connect To Your Local Node

##### [First, download and run MyCrypto Desktop App.](https://download.mycrypto.com/)

#####  Run geth or parity with correct flags

  *   Geth: `geth --syncmode=light  --rpc --rpccorsdomain "null" --keystore "dont_put_secret_files_here_ever"`

  *   Parity: `parity --jsonrpc-cors "null" --keys-path "dont_put_secret_files_here_ever"`

##### Connect to your node

*  Open the MyCrypto desktop application.

*  At the bottom-left there is a node switcher. Here is where you can select which node / chain you are connected to.

*  Click it, scroll all the way down & choose `Add Custom Node`

*   Enter a `Node Name` for your node

*   URL: `http://127.0.0.1:8545`

*   Select the chain. This is for some frontend features, like default tokens and ENS addresses and more. See above for more details.

![](https://i.imgur.com/wx5vZbs.jpg)

* Click "Save & Use Custom Node".

* This should immediately connect or an error message will display.

* Go to the "View & Send" tab and unlock via "View Address".

* Verify balances are loading correctly.



### Hosted Node

* Make sure your node is SSL

#####  Run geth or parity with correct flags

* Geth: `geth --datadir eth-mainnet --syncmode=light --rpcaddr "localhost" --rpc  --rpccorsdomain="https://mycrypto.com/" --unlock 1 console`

##### Connect to your Node Hosted Somewhere

* Go to `https://mycrypto.com/` or your local MyCrypto application.

* In upper right corner (MyCrypto website) or bottom left (MyCrypto desktop application) there is a node switcher. Here is where you can select which node / chain you are connected to.

*  Click it & choose `Add Custom Node`

*   Enter a `name` for your node

*   Enter the `URL`

*   Select the chain. This is for some frontend features, like default tokens and ENS addresses and more.

    *   ETH: Shows default ETH tokens, EIP-155=true, chainid=1, uses etherscan.io for links to addresses and txs.

    *   ETC: Shows default ETC tokens (none...yet?), EIP-155=false, chainid=false, uses gastracker.io for links to addresses and txs.

    *   Ropsten / Kovan / Rinkeby: Shows default testnet tokens, EIP-155=true, chainid=3/?/?, uses testnet.etherscan.io for links to addresses and txs.

    *   Custom: Allows you to select whether EIP-155 is true or false, and provide a chainid if it's true.

* Click "Save & Use Custom Node"

* This should immediately connect or an error message will display.

* If no errors, go to [https://mycrypto.com/account](https://mycrypto.com/account) and unlock via "View Address".

* Verify balances are loading correctly.


### Requirements

The URL must have an SSL certificate (aka be https://). You can get a free SSL certificate via [LetsEncrypt](https://letsencrypt.org/) very quickly.

If you node is local, it's much easier to simply also run MyCrypto locally. [Download the latest version of MyCrypto here](https://github.com/MyCryptoHQ/MyCrypto/releases/latest).


If you wish to run MyCrypto locally + hardware wallet, you will need to have a self-signed certificate in order to connect to your hardware wallet via U2F. Browsers that support U2F require that these calls take place over SSL. This is not something we have control of.

- [One way to do this is detailed here](https://support.mycrypto.com/offline/using-ledger-wallet-offline.html)

#### Parity

* https://wiki.parity.io/FAQ

* https://github.com/paritytech/parity-ethereum/releases

#### Geth

* https://github.com/ethereum/go-ethereum/wiki/FAQ

* https://geth.ethereum.org/downloads/
