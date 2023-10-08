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

![123](./figs/Yet%20Another.PNG)

4. [M3F: A novel multi-session and multi-protocol based malware traffic fingerprinting](https://www.sciencedirect.com/science/article/abs/pii/S1389128623001688)

一阶马尔可夫

5. [TSFN: A Novel Malicious Traffic Classification Method Using BERT and LSTM](https://www.mdpi.com/1099-4300/25/5/821)

数据包level bert + 序列的LSTM特征 和 BFCN同一个作者。

6. [I^2 RNN: An Incremental and Interpretable Recurrent Neural Network for Encrypted Traffic Classification](https://ieeexplore.ieee.org/abstract/document/10056861)

略

7. [Low-Quality Training Data Only? A Robust Framework for Detecting Encrypted Malicious Network Traffic](https://arxiv.org/abs/2309.04798)

略

8. [FusionTC: Encrypted App Traffic Classification Using Decision-Level Multimodal Fusion Learning of Flow Sequence](https://www.hindawi.com/journals/wcmc/2023/9118153/)

略

9. [FA-Net: More Accurate Encrypted Network Traffic Classification Based on Burst with Self-Attention](https://ieeexplore.ieee.org/abstract/document/10191615)

一眼看上去有点怪的模型

10. [NetGPT: Generative Pretrained Transformer for Network Traffic](https://arxiv.org/abs/2304.09513)

3个数据包的bert

11. [Spatial-Temporal Feature with Dual-Attention Mechanism for Encrypted Malicious Traffic Detection](https://www.hindawi.com/journals/scn/2023/7117863/)

cnn+gru

12. [Rosetta: Enabling Robust TLS Encrypted Traffic Classification in Diverse Network Environments with TCP-Aware Traffic Augmentation](https://dl.acm.org/doi/abs/10.1145/3603165.3607437)

2页短文？没看懂

13. [Transformer-Based Device-Type Identification in Heterogeneous IoT Traffic](https://ieeexplore.ieee.org/abstract/document/9951051)

14. [FastTraffic: A lightweight method for encrypted traffic fast classification](https://www.sciencedirect.com/science/article/abs/pii/S1389128623004103)



## Efficient Transformers

1. [Segmented Recurrent Transformer: An Efficient Sequence-to-Sequence Model](https://arxiv.org/abs/2305.16340)

2. [Block-State Transformers](https://arxiv.org/pdf/2306.09539.pdf)

3. [扩散器：具有长序列多跳注意力扩散的高效变压器](https://ojs.aaai.org/index.php/AAAI/article/view/26502)

## other ref

1. [A review on the attention mechanism of deep learning](https://www.sciencedirect.com/science/article/pii/S092523122100477X)
