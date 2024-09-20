---
title: "Nishio Lab - Research Project"
layout: personal
excerpt: "Nishio Lab -- Research Project"
permalink: /project/
---

# Research Projects

## Vision-Wireless
無線通信とコンピュータビジョンの融合領域に関する研究を推進しています。5Gや6Gなどの次世代移動体通信ではミリ波やテラヘルツ波など、従来はレーダに用いられていたような非常に高い周波数が通信に用いられます。しかし、これらの高い周波数の信号は車両や歩行者によって遮られるだけで大きく減衰します。本研究では、身の回りに増えつつあるカメラやLiDARなどの環境センシング技術を用いてこれら高周波帯通信の状態を予測したり通信に役立てるVision 4 Wireless (V4W)技術や、その逆の問題、すなわち、無線通信の信号から環境の状態を推定するWireless for Vision (W4V)技術を研究しています。

<div class="row">
  <div class="col-sm-3">
      <center>
          <img src="{{ site.url }}{{ site.baseurl }}/images/research/viwi.png" alt="写真" width="250px">
      </center>
  </div>
  <div class="col-sm-9">
      <h4>Vision to Wireless Communications (V2W)</h4>
      カメラ画像などコンピュータビジョン技術を用いて無線通信を予測したり制御したりする新技術を創出します。
  </div>
</div>

<div class="row">
  <div class="col-sm-3">
      <center>
          <img src="{{ site.url }}{{ site.baseurl }}/images/research/imaging.png" alt="写真" width="250px">
      </center>
  </div>
  <div class="col-sm-9">
      <h4>Wireless for Vision　Sensing</h4>
      Wi-FiやWigigの信号から、部屋にいる人の人数や行動を推定したり、映像を復元したりする次世代のセンシング技術を実現します。
  </div>
</div>

## Communication-oriented Machine Learning
無線通信と機械学習の融合領域に関する研究を推進しています。特に通信ネットワーク上のスマートフォンやラップトップ、サーバやIoTデバイスが、互いに連携しながら機械学習のモデルの訓練や推論処理を分散協調に行う技術に関して、通信ネットワークとの親和性の高い手法を研究開発しています。具体的にはFederated Learning (連合機械学習)やSplit Computing（分散推論）、Semantic Communicationsの新たなアルゴリズムやメカニズムを研究します。

<div class="row">
  <div class="col-sm-3">
      <center>
          <img src="{{ site.url }}{{ site.baseurl }}/images/research/FL.png" alt="写真" width="250px">
      </center>
  </div>
  <div class="col-sm-9">
      <h4>Communication-efficient Federated Learning</h4>
      スマートフォンやセンサなど無線ネットワーク上の端末のもつデータや計算能力を活用して機械学習を分散的に行い、高度なAIを実現します。
  </div>
</div> 

<div class="row">
  <div class="col-sm-3">
      <center>
          <img src="{{ site.url }}{{ site.baseurl }}/images/research/SC.png" alt="写真" width="250px">
      </center>
  </div>
  <div class="col-sm-9">
      <h4>Communication-oriented Split Computing</h4>
      通信帯域の制限や通信路におけるパケットの欠損など、通信ネットワーク的な制約がある中でも効率的に動作する分散機械学習推論手法を研究します。
  </div>
</div> 

---


<br><br>
<div class="row">
  <div class="col-sm-3">
      <center>
          <img src="{{ site.url }}{{ site.baseurl }}/images/research/wifi.jpg" alt="写真" width="250px">
      </center>
  </div>
  <div class="col-sm-9">
      <h4>Self-optimizing wi-fi</h4>
      強化学習技術を用いて自律的に学習し、通信速度最大化や遅延最小化するWi-Fi制御を実現します。
  </div>
</div>
<br><br>



## JST さきがけIoT　「機械学習するIoT通信ネットワーク基盤」 （2020年度〜2023年度） 
本研究は、IoT-AIトラヒックの爆発的増加とデータプライバシの課題を解決するため、IoTデータの地産地消を実現する通信とAIデータ処理が一体化したIoT基盤構築を目指す。従来型クラウドAIを用いたIoTデータ処理ではなく、IoTデータを収集するローカルNW内で分散的にAI処理することで、コアNWのトラヒック削減とリアルタイム性向上および機密情報流出の危険性を大きく低減可能なIoT基盤を創出する。

#### Distillation-Based Semi-Supervised Federated Learning (DS-FL)
Federated Learningの課題であるモデル共有時に発生する大量の通信トラヒックを削減するため、モデル自体ではなくモデルの出力（logit）を用いた学習フレームワークを提案した。従来のモデル共有に基づくFLと比べ、一定の精度を達成するまでの通信トラヒックを1/50~1/100に低減できることを示した。

- S. Itahara, T. Nishio, Y. Koda, M. Morikura, and K. Yamamoto, "Distillation-Based Semi-Supervised Federated Learning for Communication-Efficient Collaborative Training with Non-IID Private Data," IEEE Transactions on Mobile Computing, Apr. 2021. (Early Access)

#### Communication-oriented Model Tuning for Split computing (COMtune)
ニューラルネットワークを分割し端末とサーバで分散的に行うSplit computingにおいて、ニューラルネットワークの構造を工夫することで通信トラヒックの削減やパケット損失耐性を向上し、Split computingの通信効率を向上する技術を提案した。70%のパケットが損失する状況においても推論性能の低下を維持できることを示した。

- S. Itahara, T. Nishio, K. Yamamoto, "Packet-Loss-Tolerant Split Inference for Delay-Sensitive Deep Learning in Lossy Wireless Networks," Proc. IEEE Globecom, Dec. 2021.
- Sohei Itahara, Takayuki Nishio, Yusuke Koda, Koji Yamamoto, “Communication-oriented Model Fine-tuning for Packet-loss Resilient Distributed Inference under Highly Lossy IoT Networks,” arXiv preprint arXiv:2112.09407, Dec. 2021.

---

## 科研費 若手研究 「無線通信環境をみるコンピュータビジョン技術」　　（2018年度〜2021年度） 
本研究は、カメラやレーダなどの視覚（ビジョン）データから無線通信品質を予測することである。ミリ波通信や可視光通信、テラヘルツ通信など超高周波帯を用いた通信では、歩行者や車、植物などが見通し通信路を遮蔽すると信号電力が大きく低下し、通信品質を劣化させる。一方、反射物となるようなものが近傍に存在すれば、強い反射波を受信することで通信を継続することができる。このような電波伝搬空間情報はカメラやレーダなどビジョンデータに内包されており、それを読み解くことで通信品質を予測できる可能性がある。


