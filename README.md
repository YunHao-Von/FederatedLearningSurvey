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
