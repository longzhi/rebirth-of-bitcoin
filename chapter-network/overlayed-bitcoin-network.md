# 双重的比特币网络

点对点网络是人们在没有中间人的情况下直接向彼此发送信息的时候。

比特币中有两层点对点网络。最著名的是矿工之间的点对点网络。但最重要的是用户之间的点对点网络。而这两层网络实际上是浑然一体，联系紧密。如果理解这一点，理解比特币的潜在能力会容易得多。

## 矿工

矿工们组成了一个点对点网络，它们互相传输区块和交易信息。它们被鼓励尽可能快地将每个区块传送给所有其它矿工，以便其它他矿工在他们的区块上建造，他们从而获得报酬。

为了做到这一点，每个矿工都因激励而彼此连接紧密。在理想情况下，这形成了一个完全图，每个矿工都与其他矿工相连。实际上，矿工与大多数其他矿工连接，但不是全部，形成了近完全图。

![miner-network](https://i2.wp.com/blog.moneybutton.com/wp-content/uploads/2019/08/Screen-Shot-2019-08-14-at-16.02.51.png?resize=1000%252C631&ssl=1)

矿工网络用于解决双重支出问题。[比特币白皮书](https://bitcoinsv.io/bitcoin.pdf)中描述了这一点：“在本文中，我们提出了使用对等分布式时间戳服务器生成双重花费问题的解决方案，以生成交易时间顺序的计算证明。”

矿工是点对点分布式时间戳服务器。它们与普通用户不同。

## 用户

用户具有不同的对等网络。用户不一定与矿工联系。但是用户确实需要相互联系才能进行交易。

用户与他们进行交易的其他用户相关联。用户不会被激励连接到所有其他用户。仅激励用户与他们想要交易的其他用户建立联系。

用户形成网状网络，就像现实的经济交易一样。

![user-network](https://i2.wp.com/blog.moneybutton.com/wp-content/uploads/2019/08/Screen-Shot-2019-08-14-at-16.02.59.png?resize=1000%252C561&ssl=1)

与现实一样，一个用户并不与其它的大多数其他用户直接关联，它们仅直接连接到他们关心的用户。

白皮书描述了这样的用户：“可以在不运行完整网络节点的情况下验证付款。用户只需要保留最长工作证明链的块头的副本，他可以通过查询网络节点获得它，直到他确信他拥有最长的链，并获得将交易链接到区块的 Merkle 分支它被加上时间戳。“

白皮书明确区分了运行节点的矿工和 “不需要运行完整网络节点” 的用户，SPV 是其中的关键。

## 结论

白皮书的标题是“比特币：点对点的电子现金系统”。标题中的点对点网络是用户，而不是矿工。这是因为数字现金是点对点交易的。

![two-different-networks](https://i2.wp.com/blog.moneybutton.com/wp-content/uploads/2019/08/Screen-Shot-2019-08-14-at-16.03.08.png?resize=1000%252C561&ssl=1)

根据白皮书，“我们需要的是一种基于加密证明而不是信任的电子支付系统，允许任何两个愿意的各方直接相互交易，而无需受信任的第三方。”在比特币中，两个人可以直接交换交易，点对点，没有可信任的第三方。交易是即时的，仅受光速的限制。当用户彼此之间没有完全信任时，可以查询矿工（“网络节点”）以确认交易的有效性。用户对等网络比矿工对等网络更重要，因为用户是矿工存在的根基，矿工为用户提供服务并获取收益，从而能让这整个系统持续下去。

中本聪最初的比特币源代码提供了 P2IP 的功能，这是一种交易点对点的方法。该代码因实现不完整而被 Core 禁用了。现在，我可以下通过 Paymail 再次实现比特币的点对点交易功能。我们建议所有钱包都采用这种方法。
