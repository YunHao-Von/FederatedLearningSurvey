# Survey on Federated Learning Threats: concepts, taxonomy on attacks and defences, experimental study and challenges   

Contributions:  
+ 回顾了水平联邦学习，垂直联邦学习和联邦迁移学习所面临的威胁和防御。  
+ 定义联邦学习中对抗攻击的分类及其相应的防御政策。  
+ 在一个共同的评估框架中比较相关的对抗性攻击的强度，以及最突出的防御方法的防御能力。  



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