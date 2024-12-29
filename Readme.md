**简单记录一下链上发生的故事：**

**熊链**[Boyco](https://app.stakestone.io/u/vault/detail/bera)存款活动自27号开始，悄悄经历了一场非平常的事件，预存款平台@Stake_Stone上出现涉及安全的事件，涉及4w+钱包的归属问题。

这里是熊链BGT持币排行榜[https://bartio.beratrail.io/token/0xbDa130737BDd9618301681329bF2e46A016ff9Ad/balances](https://bartio.beratrail.io/token/0xbDa130737BDd9618301681329bF2e46A016ff9Ad/balances)

下载CSV表单出来后，通过Stake_Stone的官方查询接口，可以查到钱包的绑定关系(如下4张图)，第5w名是BGT持币55个，大于这个数的都可以查查


![未激活用户](https://github.com/yonghumeijj/Bera/blob/main/004.jpg)

![正常未绑定](https://github.com/yonghumeijj/Bera/blob/main/001.jpg)

![正常绑定](https://github.com/yonghumeijj/Bera/blob/main/002.jpg)

![恶意绑定](https://github.com/yonghumeijj/Bera/blob/main/003.jpg)


重回到CSV表格，前5w个钱包，除了北京时间27号早晨8点左右(时间戳1735259148)起，已经绑定了邀请码的账户外，均被绑定为随机邀请码且邀请时间为空(详见[stone持币排行榜.txt](https://github.com/yonghumeijj/Bera/blob/main/%E7%86%8A%E9%93%BE%E6%8E%92%E8%A1%8C%E6%A6%9Cstone.txt)

Stone有20%邀请奖励，可以获得几个大项目方的空投，且BGT排行榜真实用户占比或达9成以上，此次定点邀请的精准度可谓是高！

**预估此次综合涉及邀请资金可达9位数，无形中蒙受不公损失的是所有在Stone预存的用户（包括嘉年华活动、因stone未空投，或能影响到未来sto的空投分配是否公平。）**



下边记录事件原因分析：

从文档1(熊链BGT持币绑)里钱包的激活预存款账户时间(activeTime)来看，所有的钱包都是有序且以时间递增的速度写入数据库绑定邀请关系。

感觉有两种可能

**1.外部原因，被黑客使用某种bug在不需要私钥签名的情况下强制设置邀请关系，危害是可能会涉及项目与资金安全.**

**2.内部原因，直接或间接写入数据库，危害是老鼠仓与公平性.**

两权相害取其轻，结论显而易见.

此次事件侧面反映了区块链安全任重而道远.

仅此记录日常趣事以便日后翻阅.
