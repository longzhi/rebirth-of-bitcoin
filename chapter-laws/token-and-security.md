# 通证与合约

1696 年，英王任命牛顿为铸币大臣，以解决货币重铸（银币）中的假冒伪劣、短斤少两。1717 年，天才的牛顿提出放弃白银，实施 “金本位” 的思想，以纸币英镑作为货币，同时将纸币币值直接挂钩黄金，即每英镑含黄金 7.32238 克或每盎司黄金对应 3 英镑 17 先令 10.5 便士。而更早的 1600 年左右，英国的东印度公司和荷兰的东印度公司则分别发明了股票制，解决了大规模商业下以货币进行投、融资的问题。自此，股票 + 纸币成为金融双翼，成就了英镑的世界货币地位，也成就了日不落帝国的商业王朝。英镑领先世界 300 年后，20 世纪初，美元取代英镑，而华尔街则取代伦敦。美元先是锚定黄金，1971 年布雷顿森林体系后，美元放弃金本位，而华尔街则发明了除股票外更多的足以眼花缭乱的金融衍生品，帮助实现以美元为本位币的投融资。同样，证券 + 美钞之金融双翼，成就了美元的世界货币地位，也成就着美国的商业王朝。但是，没有锚定黄金的美元时时冲击着世界金融市场，潜流暗涌。

2008 年，一个化名中本聪的人在电报群中公布了一种新的通过数学加密技术生产货币的方法，他将之命名为比特币 --- 一种点对点的电子现金系统。该方法采用分布式账本网络，全球任何人皆可自由加入或退出这个网络，当在算力竞赛中最先破解一道数学题时，即可获得在系统中添加一个账本和在账本中获得一定数额比特币即初始发行的权利，比特币可以在这个网络中点对点收付。比特币在许多方面都模拟了黄金，如计价单位，比特币的计价单位为数量，最小单位为 10-8 个比特币，而黄金的计价单位为重量 ---- 盎司或两，数量与重量均属物理属性，均是不变常量；再如可发行总量，二者都是预期衡定、不可增发的，比特币总量为 2100 万个。2009 年 1 月 3 日，中本聪利用自己发布的网络挖出了第一个账本及 50 个比特币。在这个创世账本里，中本聪写下了一段意味深长、永不修改的话 “The Times 03/Jan/2009 Chancellor on brink of second bailout for banks（2009 年 1 月 3 日，（英国）财政大臣正处于实施第二轮银行紧急援助的边缘）。” 中本聪在创世区块里嘲讽了法币，也回应着 400 年前的另一个天才 — 牛顿。

比特币自创世以来，得到越来越多的共识，也基本实现了白皮书中的几个特性：1、现金；2、电子现金；3、永不篡改的记账系统；4、点对点支付。

但是，现代商业社会下，仅仅具有现金功能，比特币是难以成为货币的，正如前文所述，英镑、美元只所以成为世界货币，除了挂钩黄金的现金属性外，更是因为发展出了一整套以英镑、美元为本位币的投融资制度，契合了商业，这个制度的核心工具便是证券。借助证券系统，英镑、美元才走向世界的各个角落。这里说的证券是一个广义概念，举凡一切权益价值凭证皆是证券，股票、期货、期权自不比说，提单、借据、债券、积分，购物卡，等等，皆可视为证券，甚至严格意义上，货币也是证券，是国家发行的对国民的债务凭证证券。比特币欲成为世界货币，亦必须建立以比特币为本位币的证券系统。有了证券系统，比特币才有大规模的商业化应用，才能走入寻常百姓家。

幸而中本聪足够伟大，其早已考虑到比特币的完整商业生态，在其设计的原代码中包含了发行 Token 的功能，而 Token (又译为通证)，可以成为比特币衍生的证券系统，且与传统证券相比，人人可自由发行，可点对点交易，可迅速传递价值。

我这里要特别说明的是，比特币原链在 2017 年 8 月 1 日因为账本（区块）扩容问题产生了分裂，分裂成 BTC（Bitcoin Core）与 BCH（Bitcoin Cash），BTC 删除了比特币的许多原有设计且区块大小锁定于 1M, 因此难以充分实现中本聪原本设计的完全商业生态包括无限发行各种复杂 Token 的功能。

一、Token 及 Token 的法律属性

Token 的原义当然不是证券，它是一个计算机术语，意思是令牌或通行指令，通常是一串符号序列，持有 Token 者可以执行或操作特定计算机指令。在比特币或数字加密货币系统中，Token 与比特币类似，亦是一串符号，由区块链代码按加密技术生成，因而是不可复制的，Token 可以在区块链上点对点传送。Token 有时又称为币（coin）或代币 (alt coin)，不过我不喜欢用币或代币这两个词，我也不认为 Token 是币或是代币。Token 的法律经济意义由发行者或使用者赋予，按照传统证券的分类，运行于区块链上的 Token 可以有以下几种法律分类：

1、证券类 Token，此相当于传统证券中的股票、期权、债券等。发行人可以通过智能合约承诺，该 Token 相当于发行人所在公司的股份、预期股份或债权等，持有人可以凭 Token 的数量按比例享有公司的决策权、分红权、预期分红权或债权，因而这类 Token 实质上就是股票、期权、债券等。
2、现金类 Token, 此相当于传统证券中的票据如支票、汇票等，发行人通过智能合约承诺，持有该类 Token 者可以按指示获得比特币等加密货币。
3、证明类 Token，此相当于传统证券中的提单、仓单、购物卡、各种产权证书等，持有此等 Token 者享有 Token 所记录的各项权利，如货物所有权、房屋所有权、购买特定货物、享受特定服务的权利等；
4、身份类 Token，此相当于传统经济中的身份证、会员证、游戏卡等，持有此等 Token 者，具有某种特定身份或资格，这种身份或资格或与利益有关，或与利益无关。

区块链上的 Token 实际上可以涵盖社会生活的方方面面，当其可以点对点、迅速交换或传输时，意味着其代表的权利或价值可以在无中介、无审查的情形下瞬间转移，这是前所未有的，对人类生活必将产生深远的影响。

同时，我们也可以看到，Token 既不是币，也不是代币，当发行人不承诺 Token 可实现某种权利或利益，或者 Token 根本就不具有实现某种权利或利益的功能时，这样的 Token 不管称为币还是代币，事实上连幂币也不如，也不具有任何可交换的价值，目前市面上的经 ETH、经 ICO 而发行的各种代币，绝大多数属于此类。

二、Token 的发行

1、发行许可：与传统证券发行的注册制或审核制不同，Token 的发行是自由的、无需许可的。发行 Token 的程序自动运行于货币公链或某个可以发行 Token 的公链上，任何下载公链客户端的人，均可一键发行，发行 Token 的种类和数量，悉由用户自行决定。现已推出的能够发行 Token 的以太坊（ETH），刚刚面世的基于 BCH 的虫洞协议，以及即将问世的基于 BCH 的其他 Token 协议，都将遵守这样的原则。容易理解，Token 的本质是公民的个人权利证书，其发行规则应采最低门槛，即自由的、非许可的发行。

2、发行协议：发行 Token 的协议旨在实现通过用户的客户端即钱包地址输出一串加密符号，程序无法干预这个符号能作什么用途，Token 的功用或法律属性是由发行人决定的，本质上是发行人与拟交易对象（持有人）之间的一个契约，而现实生活千差万别，Token 的种类和功能亦不计其数，Token 协议不可能一一预见，也无需一一预见。因此，Token 协议应当具备高度灵活性，包括三种灵活性，对应于发行过程中的三个主体，一是 Token 协议制定者，应当允许 Token 协议与其他公链进行交互，比如一个房产权人拟通过 BCH 链发行并交易自己的产权证 Token，该交易的价值是巨大的，是交易房屋产权，发行人必须承诺这个 Token 对应真实房产，持有 Token 即持有房产，如果他的原始房屋产权以 Token 形式登记于另一公链，那么这两个公链必须能够实现价值交换；二是 Token 发行人，Token 协议应当允许发行人自由定义拟发 Token 的种类、功能、数量、发行对象以及对所发 Token 的承诺，发行承诺比如分红一旦确定，永久记录于区块链，在发行人与持有人之间产生法律效力，直接约束发行人与持有人；三是 Token 持有人，即发行人的交易对象，Token 协议应当允许持有人对发行人进行反约束，包括持有人查阅发行人账本的权利，投票的权利、建议更改协议的权利等，这些权利一旦经由 Token 协议运行，将是不可逆的，直接对发行人产生法律后果，比如持有人对发行人的锁仓比例发起投票，一旦票决通过，程序即自动执行对发行人的仓位锁定。

3、发行平台：Token 在什么样的公链上发行，是整个数字加密货币领域的一个重大战略问题。首先，是财产安全问题，Token 是价值载体，是可以变现为钱的，因此必须给予不低于货币的安全保护，目前看，只有基于 PoW 的货币公链可以提供如此强大的算力保护，而且加密货币的演化，只有集合了地球最强算力、最大能量的加密货币才会最终胜出，因此一个有远见的 Token 发行者，应当选择最有可能成为全球货币的那个公链发行 Token，将 Token 存储于货币地址上，并接受公链的密钥保护。其次，是交易迅速问题。一个能够成为全球货币的公链必是交易迅速的，因此选择了安全，实际是就是选择了速度。我不太看好目前的 ICO 或 Token 项目动不动就声称要做自己的公链，当货币链可以发行 Token 时，当 Token 可以成为证券、票据、提单、身份证明等权益价值载体时，这些所谓独立的公链难以有独立存在的价值。正如现在所有的证券、债券、票据......, 都依赖于一个中心，即中央银行，同样，在数字货币领域，所有的 Token 都依赖于货币公链，货币公链就是全球的中央银行。当然，不排除在公链的演进过程中，会形成诸如票据结算中心，证券结算中心等等具有清算特定功能 Token 的公链，但这些公链或是货币链的侧链，或基于货币链的二级链，均是依赖于货币结算层的，这些链说是票据、证据结算中心，但其运行是去中心化的。

三、Token 的交易

一个初始发行的 Token, 只是一串存储于公链地址上的符号，如需实现发行人承诺或赋予这个 Token 的价值，必须经过交易，比如融资型 Token，只有将 Token 卖出去了，才能获得资金。交易可以点对点，也可以在交易所集中交易。Token 的交易应当符合以下原则：

1、Token 应当以加密数字货币作为计价的本位币。假如 Token 在货币公链上发行，则应当以该公链货币为计价本位币。因为如以法币为本位币，则 Token 不可避免会被法律定义为证券，且将以现行证券法、银行法进行监管，带来极大不确定性；而以加密数字货币为本位币时，其法律地位和抗审查性，取决于加密货币，如加密货币是抗审查的，则 Token 亦是抗审查的，且此时加密货币与 Token 互为生态，互为支持；

2、Token 应当具有内在价值，该内在价值由发行人承诺或赋予，并永久、不可篡改地记入区块链，成为发行人与持有人之间的契约，具有法律约束力。比如融资型的 Token，发行人欲通过发行 Token 而获得融资时，必须承诺持有 Token 者有权获得发行人使用该筹资经营而产生的红利，该承诺不得反悔。无此承诺者，不得上线交易。

3、Token 应当赋予持有人制约发行人的权利，传统证券主要通过国家的法律监管实现这一目的的，比如发行人或私募人在证券上市后三年内不得交易，公募发行者需连续三年有利润才准发行、交易，投资人有查阅财务账簿的权利等等。Token 应当吸收国家的成功监管经验，并纳入 Token 协议中。在区块链下，通过智能合约更有可能实现国家法律所难以实现、难以覆盖的监管。比如可以通过智能合约直接锁定发行人的 Token 地址且向所有投资人公开；可以设定发行人公司的连续三年红利必须达到拟发行价格的多少才能触发首次交易；发行人募集的所有加密货币地址必须全部向公众公开，否则不得触发交易；私募者的价格和地址应当向所有持有人公开；发行人的账簿必须向所有投资人公开，等等。

关于发行人的账簿，如采比特币为本位币记账，则天然是透明的，因为所有现金（比如 BCH）的走向在区块链上是天然透明的。鉴于比特币交易的不可逆性和 UTXO（未花费交易支出）特性，任何公司的钱包地址余额都是已经结算了全部往来账后的余额，因而就是利润，所以投资人只要知道发行人的钱包地址，均可随时、自由查阅账簿，随时可知晓当下可分配红利，从而决定是否持有 Token。这便构成对发行人的最强有力反制。

从这里也可以看出，如采比特币为记账本位币，连会计都是多余的，因为比特币的 UTXO 设计天然地充当了会计，企业的一切往来账，均随时、随地在区块链由得到矿工的自动清算。

不由赞叹，比特币真是人类一项伟大的发明。当然我们也要看到，只有在数字加密货币已经成熟，企业已将数字加密货币作为记账的本位币时，Token 融资对投资人的保护才是空前强大的，对社会诚信的建立才是空前强大的，其强大远远胜过国家的法律监管。所以，Token 采数字加密货币为本位币极其重要，只有这样，Token 与加密货币才会相辅相成，犹如篇首提到股票 + 货币是金融双翼，Token + 比特币也是金融双翼，Token 成就数字加密货币，数字加密货币成就 Token, 二者共同成就人类新的商业文明。

四、Token 对现代投融资制度的影响

Token 可人人自由发行，可点对点无中介、无审查的交易与传输，可自我监管。仅凭这几点，相信有心的读者已经知道，以 Token 作为投融资工具，将对现代经济制度产生无法想象的深远影响。
不过，我在这里主要强调另一个影响，那就是 Token 投融资对人类更公正，可以消除法币的 “离法币越近、获利越大” 的根本性不公正。为什么？因为 Token 计价的本位币是比特币之类的数字加密货币，其发行是去中心化的，其总量是衡定的，不存在投融资时的信贷扩张，也就是不存在加印钞票，发行人借以融得的比特币是实打实的，投资人购买 Token 所花费的比特币也是实打实的，任何一个人如果用掉了手中的比特币，除非依靠价值劳动、依靠价值交换，将没有其他办法获得比特币，他将不能通过申请贷款以央行加印钞票的方式获得资金，也难以通过武力抢劫获得资金，从而，最大限度地的消除了法币发行与流通中的金融食利者、暴力暴利者，最大限度地实现人类公平。

五、Token 对现代法人制度的影响

  1、财务会计制度影响。前面已经提到，如采比特币为记帐本位币，由于比特币交易的不可逆性和 UTXO 设计，企业的任何一笔往来都是实时清账的，都在区块链的浏览器上有迹可寻，比特币的矿工节点实际就是会计，因而比特币消灭了会计。

  2、法律身份的影响。现代法人包括股份公司、有限公司、合伙企业等多种组织形式，但是，当一家企业采 Token 融资而组建并以比特币为记账本位币时，每一个 Token 持有人包括持有 Token 的企业管理层、企业员工和其他 Token 持有人都是企业的所有人，每个所有人都可借运行于区块链的智能合约对企业行使管理权、监督权，尤其是比特币本位制下，企业的财务对每一个 Token 持有人都是绝对透明的，因而 Token 持有人与传统公司制下非常分散且不参与公司管理的中、小股东不同，每个人都可能或深或浅、且非常方便地的参与企业经营，传统的法人界限模糊了，甚至很难说有哪个实体、哪个组织能够代表这个企业，所谓企业变成了全体 Token 持有人的一个社区，企业的比特币钱包地址才是这个企业的本质，地址的私钥拥有者才是企业的法人，这个地址包括了企业的全部资产，也是企业被法律执行时的资产账户。

六、Token 的抗审查性与法律监管

 虽然本文在前面反复提到 Token 的抗审查性、比特币的抗审查性，但这个抗审查性并非为了游离于法律之外，抗审查性只是为了让这个人类创新事物能够在早期生存下去，能够免遭不明智政府的戕害。因为人类历史表明，政府对于新生事物总是迟钝的、甚至反感的。所以，Token 和比特币不应排斥政府的法律监管、甚至应当欢迎、拥抱。

但也由于政府的迟钝与落后、更由于作为与人类财产利益攸关的伟大发明，所以，在政府的法律监管之前，作好自律监管极其重要。任何一个行业，只有能够自律、能够自我除恶时，才有可能得到政府承认，才有可能得到大多数人的承认。

几乎所有国家的民法都规定：处理法律纠纷时，法律有规定的，依照法律；法律没有规定的，适用习惯。什么是习惯？对 Token 而言，就是 Token 在发展过程中形成的行业惯例、国际共识，以及 Token 在发行、流通过程中形成的各种程序性协议、智能合约以及各法律主体签署的契约等等，这些事物在纠纷发生时，均具有法律效力。均有可能被司法系统直接采用。
