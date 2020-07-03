# Lambda wallet instructions
Version 0.5.53

One Lambda wallet supports creating and managing multiple accounts. At present, wallet only support Chinese and English.


Download here: 
[https://github.com/LambdaIM/launch/releases/tag/Wallet0.5.53](https://github.com/LambdaIM/launch/releases/tag/Wallet0.5.53)  
[http://download.lambdastorage.com/wallet/0.5.53/](http://download.lambdastorage.com/wallet/0.5.53/)


![avatar](img/wallethome@2x.png)

* [Create Account] (#Create Account)
* [Import mnemonic into the node package] (#Import mnemonic into the node package)
* [Import Account] (#Import Account)
* [Wallet homepage description] (#wallet homepage description)
* [Receive Testnet Test Coin] (#Receive Testnet Test Coin)
* [Transfer] (#transfer)
* [Export Account Configuration File] (#Export Account Configuration File)
* [Replace Pledge node of wallet link] (#Replace Pledge node of wallet link)
* [LAMB to TBB] (#LAMB to TBB)
* [View verification node and Pledge] (#View verification node and Pledge)
* [Transfer Pledge] (#Transfer Pledge)
* [Cancel Pledge] (#Cancel Pledge)
* [View partner and Pledge] (#View partner and Pledge)
* [Extraction Reward] (#Extraction Reward)
* [Extract Node Profit] (#Extract Node Profit)
* [View assets and trading assets] (#View assets and trading assets)
* [Proposal and Deposit and Voting] (#Proposal and Deposit and Voting)
* [Market and Trading Space] (#Market and Trading Space)
* [Open lambdaS3 console] (#Open lambdaS3 console)
* [Switching between mainnet and testnet] (#Switching between mainnet and testnet)
* [Create mining sub-account, export and import] (#Create mining sub-account, export and import)
* [Initialize Miner] (#Initialize Miner)
* [Select Use Wallet Identity Role] (#Select Use Wallet Identity Role)
* [Mining Guide] (#Mining Guide)
* [Set gas fee] (#Set gas fee)
* [Withdraw order commission] (#Withdraw order commission)
* [Order Renewal] (#Order Renewal)
* [Pledge Market] (#Pledge Market)
* [Withdraw Market Validated Income] (#Withdraw Market Validated Income)

## Switch language

![avatar](img/lang@2x.png)
## 账号创建和导入
### 创建账号
点击 Create Wallet  进入创建钱包的页面

输入钱包名称，密码，确认钱包密码，点击 Create 按钮，
## Create and import an account
### Create an account
Click Create Wallet to enter the page for creating a wallet

Enter the wallet name and password, confirm the wallet password, and click the Create button,
![avatar](img/create@2x.png)

After clicking the Create button, enter the mnemonic page


Save the mnemonic words in the right order for future restore purpose, click Next Step to enter the next page.
It is advised to write down the mnemonic words on paper. Mnemonic words are used to import into node programs. 

![avatar](img/word@2x.png)

In the mnemonic words confirmation page, fill in the words in the right order for restoring account.

![avatar](img/select@2x.png)

Click to complete

![avatar](img/selectall@2x.png)

Click Export Keystore File to backup the wallet.

![avatar](img/file@2x.png)

You can import the wallet again through lambda********.keyinfo

Create an account through the wallet


### Import Mnemonic words into the node's package

Verification nodes and miners can import the account in the wallet into the mining package (lambda chain) and run the mining program.

After creating an account, save the mnemonic words, which can be imported into the verification node and miner programs.

For example, the mnemonic is imported into the node's package

Use lambdacli to call the command line


```bash
./lambdacli keys add [name] --recover
```

Enter the password twice as prompted to confirm

```bash
Enter a passphrase to encrypt your key to disk:
Repeat the passphrase:
```
![avatar](img/zhujici.png)


If the address of the output account is the same as the wallet, the import is successful

**tips**
Note that the mnemonic combination in the example is just a test account


### Import Account

Click on the Import wallet to enter the account import page

![avatar](img/import@2x.png)

Click Choose Wallet Files to select the backup file of the account

The backup file suffix is ​​keyinfo, for example, the configuration file created by the wallet is lambda.keyinfo

Enter the password when creating the wallet, then enter the name of the new wallet, and click Import to import the wallet

## Wallet Home Description
The newly created account has a balance of 0 and no transaction history

![avatar](img/home2@2x.png)

At the top is the navigation menu, click the settings button to enter the settings page, click the account address to copy the account

At the bottom is the information of the Validator node connected to the wallet, including the node's public key address, block height, and block generation time

The account has a rendering of the transaction record

![avatar](img/home@2x.png)

## Receive testnet test coins

After logging in to your wallet account, click on the activity link on the homepage
![avatar](img/WXceshicoin1.png)
redirect to 
[http://faucet.lambda.im/](http://faucet.lambda.im/)
![avatar](img/WXceshicoinget.png)
Enter the created lambda main network address, for example lambda163q4m634nq8les4nuvdvz49tk6aeh926t0****

Now the account will receive LAMB and TBB of the testnet for storage mining testing

Receipt rules:
One IP can receive 50000 LAMB and 5 TBB every 24 hours;
For a Lambda main network address, you can receive LAMB and TBB capped 10 times.



## Transfer
Click the Transfer button on the home page, a transfer dialog box pops up, fill in the address and amount of the transfer

![avatar](img/send@2x.png)

Click Next, preview the transaction information, then modify the gas if needed
![avatar](img/send3@2x.png)
Click OK. A dialog box for entering the wallet password pops up, fill in the wallet password

![avatar](img/pasword@2x.png)

Click Submit and wait for the transfer to be completed in about 10s. Once sucessfully transferred, the display is as follow:

![avatar](img/ok@2x.png)

Click View Detail to view transaction details

![avatar](img/view@2x.png)

## Export account configuration file

Click Keystore File Backup on the settings page to view the account backup file

![avatar](img/set@2x.png)

## Change the Pledge node of the wallet link
Click Switch Pledgeon the settings page to enter the page for viewing Pledge information

![avatar](img/info@2x.png)

Change the IP address of the node in the input box, click Submit, the prompt message is as follows after the switch is successful

![avatar](img/ok2@2x.png)

## LAMB to TBB

TBB can be used for Pledge

![avatar](img/duihuan1@2x.png)

![avatar](img/duihuan2@2x.png)



## Pledge related operations
### View verification nodes and Pledge
![avatar](img/valist@2x.png)
The first column My Pledge list
Second column Verification node list
Click to verify node list
![avatar](img/valist2@2x.png)
Click to view verification node details
![avatar](img/vainfo@2x.png)
Click the Pledge button to validate
![avatar](img/zhiyainfo@2x.png)
### Transfer pledge
Click the transfer pledge button on the node's details page
![avatar](img/WXrv1@2x.png)
Click to open the pledge window

Fill in how many TBB needed to be transferred and select a new node

(If you want to transfer all TBB, it may fail. It is recommended that the total pledge -0.1 tbb be transferred to pledge is easier to succeed)

![avatar](img/WXr2@2x.png)
### Cancel pledge
Click the cancel pledge button on the node's details page
![avatar](img/cancel1@2x.png)
Click to open the cancel pledge window
![avatar](img/cancel2@2x.png)
Fill in how many TBBs need to be cancelled

(If you want to cancel all TBB, it may fail, it is recommended that the total pledge -0.1 tbb cancel pledge is easier to succeed)


### View partners and pledges
First column my pledge
Column 2 List of partners
![avatar](img/plist@2x.png)
Click on the partner list to view all partner information
![avatar](img/plist2@2x.png)
Click to view partner details
![avatar](img/pinfo@2x.png)
Click the pledge button to pledge
![avatar](img/zhiya2@2x.png)

## Extract reward-related operations
### Withdraw rewards
Click [Extract Rewards] in the [Extract Rewards] drop-down menu on the homepage
![avatar](img/wv3@2x.png)
![avatar](img/wi1@2x.png)


### Extract node revenue
Click [Extract Node Revenue] in the [Extract Reward] drop-down menu on the homepage
![avatar](img/wv1@2x.png)
You can open the window for extracting node revenue
![avatar](img/wv2@2x.png)


### View assets and trading assets
Click the Assets tab on the wallet homepage to view which assets are in the current account
![avatar](img/asset1@2x.png)
Click the trading button to open the window for trading assets
![avatar](img/asset2@2x.png)

## Proposal and deposit and voting
Click [Proposal] in the navigation menu at the top to enter the proposal list page
![avatar](img/t1@2x.png)
Click the text description part of the proposal to enter the proposal details page
![avatar](img/t2@2x.png)

When the status of the proposal is [deposit stage], a deposit can be deposited for the proposal
Click the Deposit Deposit button to open the Deposit Deposit dialog
![avatar](img/t3@2x.png)
When the total deposit is satisfied, the proposal will enter the [voting stage], click the voting button to open the voting dialog box

![avatar](img/t4@2x.png)
Vote can choose to agree, oppose, strongly oppose, abstain

If the first vote is wrong, it does not matter that the second vote will overwrite the result of the first vote

The weight of voting is equal to the amount of pledge. Both the pledge at the node and the partner pledge are effective pledges.

If there is no pledge, the vote is invalid

## Market and trading space

Click the market link in the navigation bar to enter the market page


### My order list
Order list contains buy and sell orders

![avatar](img/WXmk1@2x.png)

Purchase space

There are two ways to purchase space: one is to automatically match the purchase, and the other is to select a certain miner's high-quality sell order to buy.

The automatic matching purchase is an ordinary sell order with odds of 0.5 unit price and 5 lamb.

A high-quality sell order is a sell order with a odds of 1 unit price greater than 5lamb, and can be specified to buy.

![avatar](img/WXmk2@2x.png)

Automatic matching purchase space only needs to fill in the size and duration of the space, for example, purchase 3 months 2GB of space

![avatar](img/WXmk7@2x.png)

To purchase a high-quality purchase order from a miner, you need to select a miner first, and check whether the minimum purchase space size, minimum purchase duration, and maximum duration of the order meet your needs. If they are satisfied, fill in the space size and duration to purchase

![avatar](img/WXmk15@2x.png)


### Sell space
 If the current account is a miner's account, here will list the list of sell orders for this account in the market
 
![avatar](img/WXmk3@2x.png)
After completing the startup of miners and storage nodes in the miner management program, you can hang the sell order of the storage node in the wallet


Select the storage node in the pop-up dialog box and fill in the size of the space to be sold (one storage node can only hang one sell order, it is recommended to sell all the space at once)

, Odds, unit price and conditions that restrict users to purchase, the minimum purchase space size, the shortest duration, the longest duration can be

About odds
Odds = 0.5 The price cannot be specified, only 5LAMB/G/month

Odds = 1 need to specify the price, price >= 5LAMB/G/month

Odds = 0.5 for ordinary sell orders, odds> = 1 for high-quality sell orders

Only high-quality sell orders will appear in the market list for users to choose, ordinary sell orders can only be automatically matched

![avatar](img/marketd4.png)



 Click View details on the order list page to enter the order details page
 
 Details page of sell order
 
![avatar](img/WXmk4@2x.png)


## Open the lambdaS3 console
After the purchase order, you can upload and download files through the lambdaS3 console, using storage space

![avatar](img/markets2.png)
Here you can modify the username and password required to log in to s3

If you need to use the space of this order, you can upload files to the space in the lambda storage and delete the files in the space

On the order details page, click to view the order space, a pop-up authorization dialog box, you can complete the authorization of this order

![avatar](img/markets1.png)

Enter on the login page:

The login information of the lambda storage console prompted in the wallet: key: lambda, private key: 12345678

Complete login

![avatar](img/WXs32@2x.png)

You can upload the file, drag and drop the file to the file list area to upload the file

![avatar](img/WXs31@2x.png)

## Switch between mainnet and testnet
After logging into the wallet, click the network type on the left side of the footer to enter the node selection page

![avatar](img/WXqh@2x.png)

Click the default mainnet ip and click submit to switch to the mainnet

Click the default testnet ip and then click submit to switch to the testnet

## Mining sub-account creation, export and import

Click mining on the wallet homepage, wizard, click next, until you see the create sub-account module

![avatar](img/sonaccount.png)

You can see the create miner sub-account and import button

### Create Sub Account
Click the Create Sub Account button to open the Create Sub Account popup window

![avatar](img/sonaccountd1.png)

To create a miner sub-account, you need to enter the mnemonic words and password of the current wallet, and enter a note to remember

You can also import sub-accounts exported by wallets or blockchain programs

### Import sub-account
If you have a subaccount json file, you can import the subaccount through the wallet. If you have already done the above operation to create a sub-account, you can skip this step.

Click the Import button to open the import sub-account pop-up window

![avatar](img/sonaccountd2.png)

Importing a sub-account requires selecting the json file of the sub-account and the password of the current wallet

### Export subaccount
If you need to use the mining sub-account in the miner management program or blockchain program, you can export the sub-account

![avatar](img/sonaccountd3.png)

Exporting the sub-account requires entering the password of the current wallet

For example, select the sub-account exported by the wallet in the miner management program
![avatar](img/sonaccountd5.png)

## Initialize miner

Click the Mining Wizard in the navigation menu and click Next on the Mining Wizard page until you see the Initial Miner Module
Click the miner initialization button to open the create miner popup window
![avatar](img/minersetup.png)

To create a miner, you need to select the sub-account in the wallet and deploy the dhtid of the miner server
You can get the dhtid of a miner service in the miner management program
E.g

![avatar](img/marketd3.png)
## Choose to use the wallet identity role

The first time you install and use the wallet, it will automatically pop up. After that, you need to switch your identity. Click the edit button of the role on the settings page to open the popup
![avatar](img/role.png)

Choose different roles and use slightly different functions
#### Wallet users
View assets, transfer money, pledge mining, vote on proposals, withdraw pledge rewards

#### Users who buy space
View assets, transfer money, pledge mining, vote on proposals, buy space, use lambdas3, withdraw pledge rewards

#### Miner
View assets, transfer funds, pledge mining, vote for proposals, market trading space, mining wizard, extract pledge rewards, extract storage mining rewards

#### Verification node
View assets, transfer funds, pledge mining, vote on proposals, extract pledge rewards, and extract node revenue


## Mining Wizard
Select the role of miner to use the wallet, you can see the menu of the mining wizard in the navigation menu

![avatar](img/MiningGuide.png)
The mining guide shows the mining steps of the miners,
And collated the functions of the wallet that need to be used in the mining process, and the description of the miner management program

The features of the wallet included in the mining wizard are

1 Pledge mining

2 Create a miner sub-account

3 initialize miner

4 space for sale

## Set gas fee

Click Edit gas price on the setting page, open the pop-up window, you can set the gas fee
![avatar](img/Gasprice.png)

## Withdraw order commission

Click the transaction on the homepage of the wallet, click to withdraw order commission
![avatar](img/txlist2.png)

Open a pop-up window for withdrawing order revenue
![avatar](img/Orderrevenue.png)
Withdrawal order revenue is the revenue from the batch withdrawal order
Withdraw 100 orders at a time
If there are many orders, you can try to divide the area, for example, extract the first page, extract the second page,
The extraction rules are as follows

Each 100 orders is 1 page, the order quantity is relatively large, the page number can be filled in 1, 2, 3, 4, 5, 6 etc.

Can only withdraw 100 orders at a time

Extraction operation time limit is 1 hour extraction
The revenue in the order is calculated once every 24 hours. If the withdrawal is not initiated within 24 hours, the amount withdrawn is 0

## Order renewal

The usage time of the order needs to be increased, which can be achieved by order renewal. On the order details page, click the order demand button to open the dialog box
![avatar](img/ordertime.png)
The price of the renewal is the same as when the space was purchased,
Cannot be renewed after the order expires

## Market pledge
Click the market pledge button on the homepage to open the market pledge description page

![avatar](img/Marketpledge.png)


Only markets created by users can be pledged, and the default lambdamarket cannot be pledged

Market pledged minimum amount of 1,000 LAMB

Allow pledge in multiple markets

Users can participate in the operation of the market created by users by way of pledge.

The market income is composed of the order processing fee, the order processing fee and the renewal processing fee.

Each income in the market will be distributed according to the market pledge ratio.

Income distribution rules:

Market creator charges 10% of market revenue

The market pledger allocates the remaining 90% according to the pledge ratio (the market creator is also in the distribution set)

Click the market pledge button to open the market pledge dialog box, you can pledge
![avatar](img/MarketpledgeModel.png)

## Extract market pledge income

![avatar](img/Withdrawmarketrevenue.png)

Click on Extract Market Revenue from the drop-down list on the homepage transaction

Choose the pledged market, you can click the next step to extract the market pledged income

![avatar](img/Withdrawmarketrevenuemodel.png)










