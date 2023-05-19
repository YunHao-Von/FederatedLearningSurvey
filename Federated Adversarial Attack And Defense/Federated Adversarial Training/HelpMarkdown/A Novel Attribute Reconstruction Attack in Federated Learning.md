# A Novel Attribute Reconstruction Attack in Federated Learning  
# 联邦学习中一种新的属性重构攻击  
## Abstract 
Existing FL designs have been shown to exhibit vulnerabilities which can be exploited by adversaries both within and outside of the system to compromise data privacy.  
现有的FL设计已被证明存在漏洞，这些漏洞可以被系统内外的对手利用，以损害数据隐私。   

In this work, we consider a more practical and interesting scenario in which participants share their epoch-averaged gradients (share gradients after at least 1 epoch of local training) rather than per-example or small batch-averaged gradients as in previous works.   
在本文中，我们考虑了一个更加实际和有趣的场景，在这个场景中，参与者们分享他们的epoch-averaged梯度(在本地起码训练一个epoch后，才分享梯度)，而不是像以前的设定一样，分享每个样本或者batch-averaged梯度。  

We perform the first systematic evaluation of attribute reconstruction attack (ARA) launched by the malicious server in the FL system, and empirically demonstrate that the shared epoch-averaged local model gradients can reveal sensitive attributes of local training data of any victim participant.To achieve this goal, we develop a more effective and efficient gradient matching based method called cos-matching to reconstruct the training data attributes.   
本文首次对联邦学习系统中恶意服务器发起的属性重构攻击(ARA)进行了系统性的评估，并且实证证明了通过共享epoch-averaged本地模型梯度，可以揭示受攻击客户端的训练数据的敏感特征。为了实现这一目标，我们开发了一套更有效和高校的基于梯度匹配的算法，称为cos-matching，来重建训练数据的属性。   

## 1.Introduction  
本文的贡献如下:  
+ 本文提出了一种更加使用和有趣的对联邦学习的攻击方式，称之为属性重建攻击(ARA)，每个客户端在本地起码执行一个epoch的局部训练后，才会分享他们的epoch-averaged梯度，而非batch-averaged梯度。 
+ 本文提出了一个更加有效的基于梯度匹配的算法，称之为cos-matching，这种方法利用了受害客户端的真实更新和虚拟更新之间的余弦相似度。  
+ 我们进行了全面的分析和调查各种实际设置，大量的实验验证了我们方法的有效性。
