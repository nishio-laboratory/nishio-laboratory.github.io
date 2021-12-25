---
title: "Nishio Lab - Research Project"
layout: personal
excerpt: "Nishio Lab -- Research Project"
permalink: /project/
---

---

## JST さきがけIoT　「機械学習するIoT通信ネットワーク基盤」　　（2020年度〜2023年度） 
本研究は、IoT-AIトラヒックの爆発的増加とデータプライバシの課題を解決するため、IoTデータの地産地消を実現する通信とAIデータ処理が一体化したIoT基盤構築を目指す。従来型クラウドAIを用いたIoTデータ処理ではなく、IoTデータを収集するローカルNW内で分散的にAI処理することで、コアNWのトラヒック削減とリアルタイム性向上および機密情報流出の危険性を大きく低減可能なIoT基盤を創出する。

### Distillation-Based Semi-Supervised Federated Learning (DS-FL)
Federated Learningの課題であるモデル共有時に発生する大量の通信トラヒックを削減するため、モデル自体ではなくモデルの出力（logit）を用いた学習フレームワークを提案した。従来のモデル共有に基づくFLと比べ、一定の精度を達成するまでの通信トラヒックを1/50~1/100に低減できることを示した。

- S. Itahara, T. Nishio, Y. Koda, M. Morikura, and K. Yamamoto, "Distillation-Based Semi-Supervised Federated Learning for Communication-Efficient Collaborative Training with Non-IID Private Data," IEEE Transactions on Mobile Computing, Apr. 2021. (Early Access)

### Communication-oriented Model Tuning for Split computing (COMtune)
ニューラルネットワークを分割し端末とサーバで分散的に行うSplit computingにおいて、ニューラルネットワークの構造を工夫することで通信トラヒックの削減やパケット損失耐性を向上し、Split computingの通信効率を向上する技術を提案した。70%のパケットが損失する状況においても推論性能の低下を維持できることを示した。

- S. Itahara, T. Nishio, K. Yamamoto, "Packet-Loss-Tolerant Split Inference for Delay-Sensitive Deep Learning in Lossy Wireless Networks," Proc. IEEE Globecom, Dec. 2021.
- Sohei Itahara, Takayuki Nishio, Yusuke Koda, Koji Yamamoto, “Communication-oriented Model Fine-tuning for Packet-loss Resilient Distributed Inference under Highly Lossy IoT Networks,” arXiv preprint arXiv:2112.09407, Dec. 2021.

---

## 科研費 若手研究 「無線通信環境をみるコンピュータビジョン技術」　　（2018年度〜2021年度） 
本研究は、カメラやレーダなどの視覚（ビジョン）データから無線通信品質を予測することである。ミリ波通信や可視光通信、テラヘルツ通信など超高周波帯を用いた通信では、歩行者や車、植物などが見通し通信路を遮蔽すると信号電力が大きく低下し、通信品質を劣化させる。一方、反射物となるようなものが近傍に存在すれば、強い反射波を受信することで通信を継続することができる。このような電波伝搬空間情報はカメラやレーダなどビジョンデータに内包されており、それを読み解くことで通信品質を予測できる可能性がある。


