# Lambda钱包质押教程--pc版本
 


下载地址 ：  
[https://lambdastorage.com/walletpages](https://lambdastorage.com/walletpages)  


* [创建钱包并备份助词](#创建钱包)
* [确认备份助记词正确](#确认备份助记词正确)
* [质押到验证节点](#质押到验证节点)
* [提取收益](#提取收益)
* [配合使用浏览器查询余额](#配合使用浏览器查询余额)
* [发起交易设置gas](#发起交易设置gas)
* [转质押](#转质押)
* [取消质押](#取消质押)
## 创建钱包
下载钱包后，打开，将语言切换到中文
![avatar](img/home.png)

点击创建钱包，进入创建钱包的页面
![avatar](img/login.png)

输入钱包的名称、密码，进入查看助记词的页面

![avatar](img/word1.png)

这里需要抄写 下助记词，助记词用来导入和恢复钱包
点击下一步，进入确认助记词页面
![avatar](img/word2.png)

根据抄写的助记词，按照顺序，点击页面上的助记词，
如果抄写错误了，点击返回查看助记词语，如果顺序正确，页面会跳转到保存钱包配置文件夹，Wallet 目录下 生成的.keyinfo 文件就是创建钱包生成的配置文件，可以拷贝一份keyinfo文件用于恢复钱包

![avatar](img/key.png)

## 确认备份助记词正确

点击导入钱包，点击用助记词导入
![avatar](img/import.png)

再次输入刚才抄写的助记次，输入钱包的名称和密码，
如果提示地址已经存在，说明抄写的助记词是没有问题的，根据助记词导入的时候要特别注意单词拼写，防止出错
![avatar](img/exists.png)



## 质押到验证节点

点击订不到导航菜单中的验证节点，进入验证节点页面
![avatar](img/va.png)

选择要进行质押的验证节点，主要状态要选择打对勾的
![avatar](img/va2.png)
点击质押按钮，弹窗对话框
![avatar](img/va3.png)
输入质押的金额点击下一步
![avatar](img/va4.png)
确认质押金额，并吧手续费设置为0点击确认即可
![avatar](img/va5.png)
交易成功后，可以看到我指的质押金额了

## 提取收益
奖励为质押tbb的收益
![avatar](img/r1.png)
点击提取收益，弹出提取收益的对话框
![avatar](img/r2.png)
点击下一步，将手续费设置为0
![avatar](img/r3.png)
点击确定即可提取收益


## 配合使用浏览器查询余额
登陆钱包后，可以先转一点币到当前账户，一会钱包就有记录出现了，点击右上角的地址，复制地址
![avatar](img/account.png)
打开lamba 区块链浏览器 http://explorer.lambdastorage.com/#/
搜索地址，看看地址的余额和最新的交易记录是否和钱包相符
![avatar](img/ex.png)

## 发起交易设置gas
转账tbb 或lamb 点击交易按钮
![avatar](img/conlist.png)
弹出对话框输入接收方地址，点击下一步
![avatar](img/tbbtx1.png)
确认转账的金额和接收方地址
![avatar](img/tbbtx2.png)
并设置手续费的gas，这里设置为0，尤其是账户里只有tbb没有lamb的情况下，只有设置为0，交易才可以成功
![avatar](img/tbbtx3.png)
确认后输入钱包密码即可发送交易

## 转质押
点击转质押按钮，弹窗转质押对话框，
![avatar](img/rz1.png)
输入需要转质押的金额，并选择新的节点，
![avatar](img/rz2.png)
确认转质押的节点和金额，并吧手续费调整为0

注意：21.00天内只能转质押7笔,且不能从新节点再转出，转质押周期内，原节点被惩罚了，转质押的那部分币，仍会按照惩罚比例进行扣除

## 取消质押
点击取消质押按钮，弹出取消质押对话框
![avatar](img/rq1.png)
填写需要取消质押的金额
![avatar](img/rq2.png)
确认质押金额，将手续费设置为0，即可
注意：21.00天内只能取消质押7笔 ,取消质押后将不再发放奖励，解除质押周期内，节点被惩罚了，解除质押的币也会按照惩罚比例进行扣除