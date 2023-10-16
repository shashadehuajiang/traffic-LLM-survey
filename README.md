# traffic-LLM-survey
some related work about traffic and large language model 





## ref (useful)
1. [Transformer 是 RNN：具有线性注意力的快速自回归 Transformer](https://proceedings.mlr.press/v119/katharopoulos20a.html)

内容很好，略。

2. [A survey of transformers](https://www.sciencedirect.com/science/article/pii/S2666651022000146)

较全的一个survey

3. [On The Computational Complexity of Self-Attention](https://proceedings.mlr.press/v201/duman-keles23a.html)

结论：在强指数时间假设下，在最坏情况下，这里可能存在一种基本的“没有免费午餐”现象：似乎不太可能获得自注意力的可证明的次二次算法，同时对于所有输入也是可证明的近似准确的算法。

4. [Training Vision Transformers with Only 2040 Images](https://link.springer.com/chapter/10.1007/978-3-031-19806-9_13)



## traffic classification

1. [ET-bert](https://dl.acm.org/doi/pdf/10.1145/3485447.3512217)

2. [BFCN: A Novel Classification Method of Encrypted Traffic Based on BERT and CNN](https://www.mdpi.com/2079-9292/12/3/516)

数据包level bert + 序列的CNN特征

3. [Yet Another Traffic Classifier: A Masked Autoencoder Based Traffic Transformer with Multi-Level Flow Representation](https://ojs.aaai.org/index.php/AAAI/article/view/25674)

实际上是flow 转5个数据包的图 （40*40），然后利用图像transformer进行。

![123](./figs/Yet%20Another.PNG)

4. [M3F: A novel multi-session and multi-protocol based malware traffic fingerprinting](https://www.sciencedirect.com/science/article/abs/pii/S1389128623001688)

一阶马尔可夫

5. [TSFN: A Novel Malicious Traffic Classification Method Using BERT and LSTM](https://www.mdpi.com/1099-4300/25/5/821)

数据包level bert + 序列的LSTM特征 和 BFCN同一个作者，设计细节没写。

6. [I^2 RNN: An Incremental and Interpretable Recurrent Neural Network for Encrypted Traffic Classification](https://ieeexplore.ieee.org/abstract/document/10056861)

略

7. [Low-Quality Training Data Only? A Robust Framework for Detecting Encrypted Malicious Network Traffic](https://arxiv.org/abs/2309.04798)

略

8. [FusionTC: Encrypted App Traffic Classification Using Decision-Level Multimodal Fusion Learning of Flow Sequence](https://www.hindawi.com/journals/wcmc/2023/9118153/)

略

9. [FA-Net: More Accurate Encrypted Network Traffic Classification Based on Burst with Self-Attention](https://ieeexplore.ieee.org/abstract/document/10191615)

一眼看上去有点怪的模型

10. [NetGPT: Generative Pretrained Transformer for Network Traffic](https://arxiv.org/abs/2304.09513)

3个数据包的bert (转NLP)

11. [Spatial-Temporal Feature with Dual-Attention Mechanism for Encrypted Malicious Traffic Detection](https://www.hindawi.com/journals/scn/2023/7117863/)

cnn+gru

12. [Rosetta: Enabling Robust TLS Encrypted Traffic Classification in Diverse Network Environments with TCP-Aware Traffic Augmentation](https://dl.acm.org/doi/abs/10.1145/3603165.3607437)

2页短文？没看懂

13. [Transformer-Based Device-Type Identification in Heterogeneous IoT Traffic](https://ieeexplore.ieee.org/abstract/document/9951051)

transformer + 一些trick做分类

14. [FastTraffic: A lightweight method for encrypted traffic fast classification](https://www.sciencedirect.com/science/article/abs/pii/S1389128623004103)

略

## network traffic generation

1. [Network Traffic Generation: A Survey and Methodology](https://dl.acm.org/doi/abs/10.1145/3488375)

分析了92个流量生成器工具

2. [Generating practical adversarial network traffic flows using NIDSGAN](https://arxiv.org/abs/2203.06694)

利用GAN生成对抗性flow，但是生成的是特征，不是flow。缺了一半

3. [用于物联网流量生成的知识增强 GAN](https://dl.acm.org/doi/abs/10.1145/3485447.3511976)

GAN+LSTM+知识图 生成 flow的时间序列

4. [Flow-based network traffic generation using generative adversarial networks](https://www.sciencedirect.com/science/article/pii/S0167404818308393)

GAN+flow特征的生成

5. [使用 NetShare 生成实用的基于 GAN 的合成 IP 标头跟踪](https://dl.acm.org/doi/abs/10.1145/3544216.3544251)

GAN+ packet/flow的特征生成

6. [PAC-GAN: Packet Generation of Network Traffic using Generative Adversarial Networks](https://ieeexplore.ieee.org/abstract/document/8936224)

GAN + packet

7. [DBWE-Corbat：使用动态词嵌入和网络范围对比学习生成后台网络流量](https://www.sciencedirect.com/science/article/pii/S0167404823001128)

数据包-->ip+port

8. [Design and Implementation of Traffic Generation Model and Spectrum Requirement Calculator for Private 5G Network](https://ieeexplore.ieee.org/abstract/document/9703352)

GAN学习流量的时间--字节数矩阵

9. [DPNeT：具有生成对抗网络的差分专用网络流量合成](https://link.springer.com/chapter/10.1007/978-3-030-81242-3_1)

GAN+差分隐私+flow特征

10. [FlowGAN - Synthetic Network Flow Generation using Generative Adversarial Networks](https://ieeexplore.ieee.org/abstract/document/9724556)

WGAN + 流特征

11. [Generative Adversarial Networks (GANs): A Survey on Network Traffic Generation](https://wrap.warwick.ac.uk/165738/)

一个比较全的survey

12. [SyNIG: Synthetic Network Traffic Generation through Time Series Imaging](https://ieeexplore.ieee.org/abstract/document/10223392)

使用格拉姆角场(GAF)将时间序列数据转换为图像

13. [Stan: Synthetic network traffic generation with generative neural models](https://link.springer.com/chapter/10.1007/978-3-030-87839-9_1)

卷积神经层 (CNN) 与混合密度神经层 (MDN) 和 softmax 层集成 

14. [(SIGCOMM'22) Practical GAN-based synthetic IP header trace generation using NetShare](https://dl.acm.org/doi/abs/10.1145/3544216.3544251)

合成数据包和流标头跟踪, gan +sequence +header


## Efficient Transformers

1. [Segmented Recurrent Transformer: An Efficient Sequence-to-Sequence Model](https://arxiv.org/abs/2305.16340)

2. [Block-State Transformers](https://arxiv.org/pdf/2306.09539.pdf)

3. [扩散器：具有长序列多跳注意力扩散的高效变压器](https://ojs.aaai.org/index.php/AAAI/article/view/26502)


## other ref (network related)

1. [Datasets are not enough: Challenges in labeling network traffic](https://www.sciencedirect.com/science/article/abs/pii/S0167404822002048)

## other ref (deep learning related)

1. [A review on the attention mechanism of deep learning](https://www.sciencedirect.com/science/article/pii/S092523122100477X)


## my experiments

1. [my experiments](https://github.com/shashadehuajiang/LLM_traffic_expriments)










