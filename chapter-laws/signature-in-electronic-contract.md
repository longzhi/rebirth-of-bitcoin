# 电子合同与签名

比特币一个至关重要的问题是如何提高网络的可扩展性，从而提高交易速度和使用率。比特币 Core 开发团队提出的扩容解决方案为隔离见证，即将签名数据（见证）与交易数据分离开来。比特币社区关于隔离见证的争论多数集中在技术影响和风险的问题上。事实上，这同样存在法律风险：由于分离和丢弃了签名数据，隔离见证，以及像 Schnorr 这类改变了签名格式的做法，将使得电子合同和交易的法律证明和认证变得更加困难。

这一法律问题可能会在商界造成严重的实际问题。如果企业和个人在比特币网络使用电子合同和交易，发生了法律纠纷或应监管要求，他们却无法轻易证明和验证这些交易，那会发生什么情况呢？本文将研究这一问题在美国法律以及其他司法管辖区中的情况。

## 隔离见证如何分离签名数据

一个正常的比特币交易记录了交易和签名（见证）数据，其中签名约占数据体积的 60%。交易数据传递了在比特币交易中发送的值或记录的信息。签名数据很重要，因为它核实了交易所涉及的人员，并验证他们确实发送或接受了该交易。但是，隔离见证假设只有验证交易时才需要签名数据，并将其视为不重要的数据而丢弃。

隔离见证不是直接提高 1MB 的区块体积，而是通过将签名（见证）数据从交易数据中分离出来，从而间接地增加区块存储更多交易的能力。然后，它创建了两个哈希值：（1）一个交易数据的 “常规” 哈希值；（2）一个 “见证哈希值” 由交易数据和见证数据所组成。

这些数据是如何存储在区块里的呢？比特币协议已经使用了一个 Merkle 树（一种由信息哈希值组成的异端数据结构）来有效存储交易数据，并把 Merkle 的根放在每个被挖掘区块的块头上。隔离见证建议创建第二个 Merkle 树来单独存储见证哈希值，但不保留实际的签名数据。正如隔离见证发明者 [Pieter Wuille](https://diyhpl.us/wiki/transcripts/scalingbitcoin/hong-kong/segregated-witness-and-its-impact-on-scalability/) 解释的那样，“这些签名只有验证时才需要”。一旦给定交易被验证，隔离见证便只保留见证哈希值（在第二个 Merkle 树中），并且默认丢弃完整的数字签名。有些节点可以选择保留完整的数字签名，这就产生了三种可能的场景:

* 网络中有些节点维护数字签名
* 没有节点维护数字签名
* 最有可能的情况是：绝大多数数字签名将被丢弃。

考虑一下这在纸质合同世界中的运作情况。一旦双方签署了一份合同的硬拷贝，签名块就会被从合同主体（写有条款）切离。然后签名块被转换为索引的标识符，与数百个其他签名标识符放在一个文件柜中。在大多数情况下，物理签名块本身将会被丢弃。多年以后，如果想要证明你已经签署了（或没有签署）某个特定合同，你可以找到签名块标识符，但可能无法检索到物理签名块本身。隔离见证的最终结果将是不可靠的：你可以找到见证的哈希值，但不确定能找到数字签名本身。

## 为什么签名很重要

1996 年，美国律师协会审查了电子签名的必要性，以促进网上交易。在其数字签名指南中，美国律师协会规定了在数字环境中复制物理签名的两个关键属性：（1）签名者身份验证：数字签名应显示签署人且未经授权方很难复制；（2）文档 / 交易认证：数字签名应识别签署的内容，使其难以伪造或更改已签名的事项。大多数数字签名机制，包括美国的 NIST（国家标准与技术研究所）标准和欧盟的 eIDAS 条例，都遵循了类似的原则。

事实上，比特币使用公私密钥来签署交易的签名方法，满足了这些数字签名原则。[比特币白皮书](http://nakamotoinstitute.org/bitcoin/#selection-57.4-57.311)（在第二节）甚至将电子货币定义为“一条数字签名链”，并指出收款人可以“通过验证签名来验证所有权链”。因此，比特币系统依赖于验证数字签名的能力。相比之下，隔离见证倾向于验证交易而非签名者身份，并很少考虑这可能会导致以后的交易纠纷。

## 联邦电子签名法的含义

隔离见证可能会使交易或电子合同的当事人很难证明其真实性。在美国，企业和消费者之间的电子合同（和数字签名）通常在联邦电子签名法下是有效的。美国法典第 15 篇第 7001 节法律把“电子签名”——一个比比特币使用的数字签名更灵活的概念——定义为“与合同或其他记录有附属关系或者逻辑关联，并由有意签署记录的人执行或采用”。美国法典第 15 篇第 7006（5）节提供了验证合同已被各方签署和授权的基础，就像一个纸质的物理签名块可以用来显示当事人实际上已经签署了合同。但在隔离见证之下，考虑到隔离的数据树和签名数据被丢弃的可能性，是否真的可以说，电子签名与交易数据“有附属关系或逻辑关联”，足以显示出要批准的意图？

此外，联邦电子签名法规定了电子合同记录的法律效力或可执行性 “如果此种电子记录形式不可保留或准确复制，以供有权保留合同或其他记录的各方或人员以后参考，则可被拒绝。”美国法典第 17 篇第 7001（e）节的一项关键条款是——如果电子合同的保存形式不支持以后被准确复制，则可 **拒绝承认** 其效力或可执行性。然而，正如我们所看到的，隔离见证并不关心如何维护数字签名，只关心在交易发生时验证交易。隔离见证方法产生了很大的不确定性，即仅凭签名数据哈希是否能满足电子签名法对数字签名证明的要求。

因此，在隔离见证的情况下，想要明确证明交易的企业或消费者，最多能将见证哈希与相应的交易数据重新关联起来。但可能没办法恢复数字签名本身，这意味着电子签名法可能 **拒绝承认** 电子合同或记录的法律效力或可执行性。

只有当某个节点选择保留所有完整签名数据时，才能恢复数字签名。然而，如果一个节点被用来提供商业存档服务，对检索和验证完整的数字签名收取费用，那么它只具有经济上的动机。这将为数字签名创造一种新的中介形式，这与比特币的分散化性质是背道而驰的。

## 美国各州法律的影响

类似的问题也会在美国各州法律中出现。美国绝大多数州（加上哥伦比亚特区和美属维尔京群岛一共 47 个州）已经各自制定了统一电子交易法（UETA）的版本，承认电子交易的有效性。与联邦电子签名法类似，UETA 将电子签名定义为 “与记录 **有附属关系或逻辑关联** 的电子声音、符号或过程，由有意签署记录的人执行或采用。” 纽约的版本在 9 CRR-NY 540.4(b)中更进一步指出，如果电子签名“在传输和存储过程中与记录有联系”，则电子签名被认为“与电子记录有附属关系或逻辑关联”。但是，由于隔离见证不要求传输和存储签名数据，试图拒绝交易的一方可能会争辩说，隔离见证的签名总体无法满足纽约对电子签名的定义。

“电子声音、符号或过程”是否 “与记录有附属关系或逻辑关联” 往往是一个复杂的事实问题。例如，在 Young v. Rose, 286 P.3d 518 (Az. App. 2012)中，亚利桑那州上诉法院解释说，如果给附有协议的一封电子邮件回复了一封表示 “谢谢” 的电子邮件，并不确定这封表示 “谢谢” 的电子邮件是否属于 “电子签名”，需要对法院诉状和协议之外的事实进行审查。隔离见证会进一步复杂化这类“一个满足条件的电子签名由什么构成” 的事实调查。

当然，可以修正法律来解决这些比特币交易和合同的问题。例如，2017 年 3 月亚利桑那州通过了一项立法（HB 2417）来修改其 UETA 版本（亚利桑那州电子交易法），以确认通过区块链技术保护的电子签名、记录或合同在州法律下是有效的。它还承认智能合同是有效的。然而，法律规定符合条件的区块链技术是 “不可变的、可审核的、并提供未经审查的事实。” 在一个签名数据被剪除掉的隔离见证世界中，区块链记录真的可被审核并提供未经审查的事实吗？此外，亚利桑那州的法案并没有规定交易、智能合同或区块链签名是否必须完整地记录下来（将交易和签名数据放在一起），也没有规定如果签名数据被丢弃，它们是否还有效。如果隔离见证被激活，根据亚利桑那州的新法律和其他州法律，这些合同的有效性可能会变得不明确。

## 面临着法律风险

美国的法律体系能解决这些问题吗? 这是有可能的，但法律跟上变革性技术的速度非常缓慢。隔离见证剪除了合同或交易的一个关键元素，即当事人授权交易发生的内嵌证据，从而使挑战变得更加困难。它也没有提供任何简单机制，使得签名数据以后与交易数据 “有附属关系或逻辑关联”。这将违反美国的电子合同法律框架，可能会吓到企业使其不会在区块链上投入更多运营，并阻碍了比特币网络为未来的各种交易和智能合同提供动力的更大愿景。这种法律不确定性是隔离见证的一个重大风险。这也是 BSV(当时的 BCH) 为了避免这个风险而出现的原因。
