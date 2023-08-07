# A-Review-Of-Security-Issues-In-Federated-Learning

This is our first paper, which is called A Review Of Security Issues In Federated Learning.

```mermaid
graph LR
A1[Privacy and Robustness in Federated Learning: Attacks and Defences]  
B1[1.Introduction]  
A1 ---> B1  
B1A[A.Categorization of Federated Learning based on Distribution] 
B1B[B.Categorization of Federated Learning based on Architectures]  
B1 ---> B1A  
B1 ---> B1B  
B1A ---> B1A1[Horizontally Federated Learning]
B1A ---> B1A2[Vertically federated learning ]  
B1A ---> B1A3[Federated transfer learning]
B1B ---> B1B1[FL with Homogeneous Architectures]  
B1B ---> B1B2[FL with Heterogeneous Architectures]  
b1c[C.Threats to FL]  
b1d[D.Secure Fl] 
B1 ---> b1c  
B1 ---> b1d
b1c ---> pri[Privacy]   
pri ---> pri1[malicious server]  
pri ---> pri2[adversarial paricipant]
b1c ---> rus[Robustness] 
rus ---> pa[poisoning attacks]  
pa ---> ua[untargeted attacks]  
pa ---> ta[targeted attacks]  
b1d ---> sap[Secure Fl against privacy attacks]  
b1d ---> dfr[Defeding FL against various robustness attacks]  
A1 ---> B2[2.Threat Models]  
B2 ---> b2a[A. Insider and Outsider]  
B2 ---> b2b[B.Training Phase and Inference Phase]  
B2 ---> b2c[C.Privcy:Semi-honest and Malicious]  
B2 ---> b2d[D.Robustness: Untargeted and Targeted]   
A1 ---> B3[3.Privacy Attacks]  
B3 ---> b3a[A.Inferring Class Representatives]   
B3 ---> b3b[B. Inferring Membership]  
B3 ---> b3c[C. Inferring Properties]    
B3 ---> b3d[D. Inferring Training Inputs and Labels]  
A1 ---> B4[4.DEFENSES AGAINST PRIVACY ATTACKS]  
B4 --->b4a[A. Privacy Preservation through Homomorphic Encryption]
B4 --->b4b[B. Privacy-Preservation through SMC]
B4 --->b4c[C. Privacy-Preservation through Differential Privacy]
A1 ---> B5[5.Poisoning Attacks]  
B5 ---> b5a[A. Untargeted Attacks]
B5 ---> b5b[B. Targeted Attacks]
A1 ---> B6[6.Defences Against Poisoning Attacks]  
B6 ---> b6a[A. Defenses against Untargeted Attacks]
B6 ---> b6b[B. Defenses against Targeted Attacks]
```

```mermaid
graph LR
a2[Robust and Privacy-Preserving Collaborative Learning: A comprehensive Survey]  
a2 ---> a2b1[1.Introduction]  
a2 ---> a2b2[2.Stystem Overview:<br>We systematically introduce different types of collaborative <br>learning systems from various perspectives.]
a2 ---> a2b3[3.Threat In Collaborative Learning:<br> We summarize summarizes the privacy and <br> integrity threats in collaborative learning]
a2 ---> a2b4[4.Integrity Attacks]
a2 ---> a2b5[5.Integrity Defenses]
a2 ---> a2b6[6.Privacy Attacks]
a2 ---> a2b7[7.Privacy Defenses]
a2 ---> a2b8[8.Hybrid Defenses And Beyond]
a2 ---> a2b9[9.Open Problem]
a2 ---> a2b10[10.Conclusion]
a2b2 ---> a2b2a[A.Machine Learning Model]
a2b2 ---> a2b2b[B.Deimensions of Parallelism]
a2b2 ---> a2b2c[C.Parameter Distribution]
a2b2 ---> a2b2d[D.Model Consistency]
a2b2 ---> a2b2e[E.Federated Learning]
a2b2b ---> a2b2b1[Data Parallelism]
a2b2b ---> a2b2b2[Model Parallelism]
a2b2b ---> a2b2b3[Pipelining]
a2b2b ---> a2b2b4[Hybrid Parallelism]
a2b2c ---> a2b2c1[Centralized]  
a2b2c ---> a2b2c2[Decentralized]  
a2b2d ---> a2b2d1[Synchronous]
a2b2d ---> a2b2d2[Asynchronous]
a2b2d ---> a2b2d3[Stale-Synchronous]

a2b3 ---> a2b3a[A.Integrity Threats]
a2b3 ---> a2b3b[B.Privacy Threats]
a2b3a ---> a2b3a1[Compromise vs Backdorr]
a2b3a1 ---> a2b3a1a[Compromise attacks aims to reduce or destory <br> the trained model performance by changing model parameters, <br>which normally makes the shared model not converge <br> to a satisfactory one during the training phase.]
a2b3a1 ---> a2b3a1b[Backdoor attacks try to inject predefined malicious training samples, <br> backdoors, into a victim model while maintaining the performance of the primary task. <br> The backdoors would be activated if a input sample contains the injected triggers. <br> Because of the secrecy of triggers, it is difficult to identify backdoor attacks <br> as a backdoored model performs normally on normal samples.]

a2b3a ---> a2b3a2[Data Poisoning vs. Model Poisoning]
a2b3a2 ---> a2n3a2a[Attackers can poison the training datasets of some participants with <br>malicious samples with carefully crafted triggers]
a2b3a2 ---> a2n3a2b[Attackers compromise some participants and completely control their <br> behaviour during the training]

a2b3b ---> a2b3b1[Membership vs. Property vs. Sample]
a2b3b ---> a2b3b2[Passive vs. Active]
a2b3b1 ---> a2b3b1a[成员推理攻击确定记录是否在模型的训练数据集中]
a2b3b1 ---> a2b3b1b[属性推理攻击旨在推断参与者训练数据的属性]
a2b3b1 ---> a2b3b1c[攻击者在训练阶段获得模型更新时提取训练数据及其标签]

a2b3b2 ---> a2b3b2a[被动模式-不改变任何内容]
a2b3b2 ---> a2b3b2b[主动模式-攻击者可以在训练过程中做任何事情]


a2b4 ---> a2b4a[A.Byzantine Attacks]
a2b4 ---> a2b4b[B.Backdoor Attacks]
a2b4b ---> a2b4b1[Data Poisoning]
a2b4b ---> a2b4b2[Model Poisoning]  
a2b4b1 ---> a2b4b1a[Unclean label stand-alone backdoord<br>the adversary introduces a number of <br> miss-classified data samples into the training set. It<br> poisons the training examples and changes their labels.]
a2b4b1 ---> a2b4b1b[Clean label stand-alone backdoor<br>the adversary cannot change the label of any training sample<br> and preserves the labels of the poisoned samples<br>]  

a2b5 ---> a2b5a[Byzantine Defences]  
a2b5 ---> a2b5b[Backdoor Defences]  

a2b5a ---> a2b5a1[Statistic-based Inspection]  
a2b5a ---> a2b5a2[Learning-based Inspection]  

a2b5b ---> a2b5b1[Data Inspection]  
a2b5b ---> a2b5b2[Model Inspection]  
a2b6 ---> a2b6a[A.Threat Model]
a2b6 ---> a2b6b[B.Membership Inference]
a2b6 ---> a2b6c[C.Property Inference]
a2b6 ---> a2b6d[D.Sample Inference]

a2b7 ---> a2b7a[A. Differentially Private Collaborative Learning]
a2b7 ---> a2b7b[B. Cryptographic Privacy-preserving Collaborative Learning]
a2b7 ---> a2b7c[C. Practical Privacy-preserving Collaborative Learning]

a2b8 ---> a2b8a[A. Hybrid Defenses]
a2b8 ---> a2b8b[B. Collaborative Adversarial Training]

a2b9 ---> a2b9a[Non-IID or Noisy Scenarios in Byzantine Attacks and Defenses]
a2b9 ---> a2b9b[Certified Backdoor Defenses]
a2b9 ---> a2b9c[Privacy-performance Tradeoff in Differential Privacy]
a2b9 ---> a2b9d[Basis Datasets in Property Inference Attacks]
a2b9 ---> a2b9e[Performance Improvement in Sample Inference Defenses]

```

```mermaid
graph LR

a3[An overview of Federated Deep Learning Privacy Attacks and Defensive Strategies]

a3 ---> b1[1.Introduction]  
a3 ---> b2[2.Threat Model]  
b2 ---> b2a[A.Attack surface]
b2 ---> b2b[B.Client or server-side attacks]
b2 ---> b2c[C.Black-box or white-box attacks]
b2 ---> b2d[D.Active or passive attacks]
b2 ---> b2e[E.Attacker goal]
a3 ---> b3[3.Attack Methods]
b3 ---> b3a[A. Attacks targeting reconstruction]
b3 ---> b3b[B. Attacks targeting inference]
b3 ---> b3c[C. Attacks targeting misclassification]
b3 ---> b3d[D. Attacks targeting model corruption]


a3 ---> b4[4.Defensive Measures]   
b4 ---> b4a[A. Gradient subset]
b4 ---> b4b[B. Gradient compression]
b4 ---> b4c[C. Dropout]
b4 ---> b4d[D. Differential privacy]
b4 ---> b4e[E. Secure multiparty computation]
b4 ---> b4f[F. Homomorphic encryption]
b4 ---> b4g[G. Robust aggregation] 



a3 ---> b5[5.Relatd Work]
a3 ---> b6[6.Conclusion]

```

   ```mermaid
   graph LR
    a[Survey on federated learning threats:<br> Concepts, taxonomy on attacks and defences, <br>experimental study and challenges]
    a ---> b1[1.Introduction]
    a ---> b2[2.Background concepts on <br>Federated Learning Threats]
    b2 ---> b2a[2.1Federated Learning]
    b2 ---> b2b[2.2Differential Privacy]
    b2 ---> b2c[2.3Threat Model]
    b2c ---> b2c1[Insider vs Outsider]
    b2c ---> b2c2[Client vs Server]
    b2c ---> b2c3[Attacker knowledge]



    a ---> b3[3.Adversarial Attacks in <br>Federated Learning:Taxonomies]  
    b3 ---> b3a[First Categorisation]  
    b3a ---> b3a1[3.1 Adversarial attacks to the federated model ] 
    b3a1 --->b3a1a[3.1.1 Taxonomy according to the attack moment]  
    b3a1 --->b3a1b[3.1.2 Taxonomy according to the objective]  
    b3a1 --->b3a1c[3.1.3. Taxonomy according to the poisoned part of the FL scheme]
    b3a1 --->b3a1d[3.1.4. Taxonomy according to the frequency]

    b3a ---> b3a2[Privacy attacks] 
    b3a2 ---> b3a2a[3.2.1. Feature inference attacks]
    b3a2 ---> b3a2b[3.2.2. Membership inference attacks]
    b3a2 ---> b3a2c[3.2.3. Property inference attacks]

    a ---> b4[4.Defence methods against <br>adversarial attacks:Taxonomy]
    b4 ---> b4a[4.1. Server defences]
    b4a ---> b4a1[4.1.1. Robust aggregation operators]
    b4a ---> b4a2[4.1.2. Anomaly detection]
    b4a ---> b4a3[4.1.3. Based on differential privacy]
    b4a ---> b4a4[4.1.4. Modification of the learning rate]
    b4a ---> b4a5[4.1.5. Less is more]

    b4 ---> b4b[4.2. Client defences]
    b4b ---> b4b1[4.2.1. Based on differential privacy]
    b4b ---> b4b2[4.2.2. Perturbation methods]
    b4b ---> b4b3[4.2.3. Optimized training]

    b4 ---> b4v[4.3. Communication channel defences]

    a ---> b5[5.Expermental study]
    a ---> b6[6.Guidelines for the application <br>of defences against adversarial attacks]
    a ---> b7[7.Lessons Learned]
    a ---> b8[8.Challenges of addressing <br>federated learning threats]
    a ---> b9[9.Conclusions]


   ```


``` mermaid  
graph LR  
a["联邦学习攻击与防御综述"]  
a --->a1["1.联邦学习中的攻击类型"]
a --->a2["2.联邦学习中的防御设施"]


a1 ---> a1a["1.1 数据中毒"]  
a1 --->a1b["1.2 模型攻击"]  
a1 ---> a1c["1.3 推理攻击"]
a1 ---> a1d["1.4 服务器漏洞"]  

a2 ---> a2a["2.1 联邦学习通用隐私保护设施"]  
a2a ---> a2a1["2.1.1 差分隐私"]  
a2a ---> a2a2["2.1.2 同态加密"] 
a2a ---> a2a3["2.1.3 秘密共享"]  

a2 ---> a2b["2.2 联邦学习针对性防御措施"]
a2b ---> a2b1["2.2.1 防御数据中毒"]
a2b ---> a2b2["2.2.2 防御模型攻击"]
a2b ---> a2b3["2.2.3 防御推理攻击"]
a2b ---> a2b4["2.2.4 防御服务器漏洞"]
```


```mermaid  
graph LR 
a(A Survey of Trustworth Federated Learning <br>with Perspectives on Security, Robustness, and Privacy)  
a ---> b1[1.Introduction] ---> b1a[1.1 From Trustworthy AI to <br> Trustworthy Federated Learning]  
b1 ---> b1b[1.2Framework of Trustworthy Federated Learning]
a ---> b2[2.Threats in Trustworthy Federated Learning] ---> b2a[2.1 Threats in Data Processing of Federated Learninig]  
b2a --->b2a1[Information Leakage]
b2a ---> b2a2[Non-IID Data]
b2a ---> b2a3[Data Poisoning Attack]
b2 ---> b2b[2.2 Threats in Model Training of Federated Learning]  
b2b ---> b2b1[Model Poisoning Attack]
b2b ---> b2b2[Privacy Leakage and Communication Eavesdropping]
b2 ---> b2c[2.3 Threats in Development of Federated Learning]  
b2c ---> b2c1[Inference Phase Data Security]
b2c ---> b2c2[Inference Phase Attack]

a --->b3[3.Security]
a --->b4[4.Robustness]
a --->b5[5.Privacy]
a --->b6[6.Challenges and Future Directions]

b3 ---> b3a[3.1 The Definition of Secure Federated Learning]
b3 ---> b3b[3.2 Defense Methods in Secure Federate Learning]
b3 ---> b3c[3.3 Secure Federated Learning Works]
b3b---> b3b1[3.2.1 Secure Multi-Party Computation]
b3b---> b3b2[3.2.2 Homomorphic Encryption]
b3b---> b3b3[3.2.3 Trusted Execution Environment]

b3c ---> b3c1[3.3.1 Data Security]
b3c ---> b3c2[3.3.2 Model Security]
b3c ---> b3c3[3.3.3 Secure System]  

b4 ---> b4a[4.1 Robustness to Non-IID Data]
b4 ---> b4b[4.2 Robustness to Byzantine Problem]
b4 ---> b4c[4.3 Robustness to Targeted Attacks]

```  

```mermaid  
graph LR 

a[Trustworthy Federated Learning: A Survey] ---> b1[1.Introduction]  
a ---> b2[2.Federated Learning An Overview]   
b2 ---> b2a[A. Data Distribution-Based FL Architectures]
b2 ---> b2b[B. Scale and Communication-Based FL Architectures]
b2 ---> b2c[C. Coordination-Based FL Architectures]
a ---> b3[3.Trustworthy Federated Learning An Overview]
b3 ---> b3a[A. What is trust in FL?]
b3 ---> b3b[B. Fundamentals of Trustworthiness in FL]
b3 ---> b3c[C. Architecture of Trustworthy FL]
a ---> b4[4.Literature Review]
a ---> b5[5.Trust Evaluation In FL]
a ---> b6[6.Fairness Aware Trustworthiness In FL]
b6 ---> b6a[A. Trustworthy Feature and Sample Selection]
b6 ---> b6b[B. Trustworthy Data Sharing]
b6 ---> b6c[C. Trustworthy Model Selection]
b6 ---> b6d[D. Discussion]

a ---> b7[7.Security and Privacy Aware Trustworthy FL]  
b7 ---> b7a[A. Trustworthy Client Selection]
b7 ---> b7b[B. Trustworthy Contribution Evaluation]
b7 ---> b7c[C. Trustworthy Incentive Mechanism]
b7 ---> b7d[D. Accountability and Auditibility in FL]
a ---> b8[8.Security And Privacy Aware Trustworthy FL]
b8 ---> b8a[A. Varifiablity in Trustworthy FL]
b8 ---> b8b[B. Secure Aggregation]
b8 ---> b8c[C. Privacy Preserving FL]
b8 ---> b8d[D. Discussion]

``` 

0807 Teachers Advices  
+ 题目问题。