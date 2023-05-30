# FAT:Federated Adversarial Training   
# 联邦对抗训练   
## Abstract  
In this paper, we take the first known steps towards federated adversarial training (FAT) combining both methods to reduce the threat of evasion during inference while preserving the data privacy during training. We investigate the effectiveness of the FAT protocol for idealised federated settings using MNIST, Fashion-MNIST, and CIFAR10, and provide first insights on stabilising the training on the LEAF benchmark dataset which specifically emulates a federated learning environment.  
在本文中，我们第一次向联邦对抗训练迈出了探索的脚步，通过将联邦学习和对抗训练两种方法结合起来，在保护数据隐私的同时，减少推理期间的风险。本文以MNIST，Fashion-MNIST和CIFAR10数据集为例，研究了联邦对抗训练对经典联邦学习设定的有效性，并且提供了在专门模拟联邦学习环境的LEAF标准数据集商的进行稳定训练的第一个分析。  

We identify challenges with this natural extension of adversarial training with regards to achieved adversarial robustness and further examine the idealised settings in the presence of clients undermining model convergence. We find that Trimmed Mean and Bulyan defences can be compromised and we were able to subvert Krum with a novel distillation based attack which presents an apparently "robust" model to the defender while in fact the model fails to provide robustness against simple attack modifications.  
本文通过对抗训练的自然拓展来识别挑战，以实现对抗鲁棒性，并在客户端有可能破坏模型收敛的情况下，进一步检查理想化的设定。我们发现Trimmed Mean 和Bulyan Defences会受到影响。本文提出了一个新颖的基于蒸馏的攻击来破坏Krum，该攻击对防御者提供了一个明显“稳健”的模型，但是实际上该模型无法提供针对对抗攻击的鲁棒性。   

