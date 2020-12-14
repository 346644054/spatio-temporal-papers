# Spatio-Temporal-papers
本项目包括：时空领域历年顶会/顶刊论文，相关数据集与时空领域知名专家学者信息。



This project includes: papers of the top conferences/journals in the field of Spatio-Temporal domain, relevant data sets and information of well-known experts and scholars in the field of Spatio-Temporal domain.

# Contribution

Contributions are always welcome! Make an individual pull request for each suggestion. Please follow the specification：**[contribute](./contribute.md)**.

# Content

<table>
<tr><td colspan="2"><a href="#survey-papers">1. Survey</a></td></tr> 
<tr><td colspan="2"><a href="#applications">2. Applications</a></td></tr> 
<tr>
    <td>&emsp;<a href="#traffic-prediction">2.1 Traffic Prediction</a></td>
    <td>&ensp;<a href="#flows-prediction">2.2 Flows Prediction</a></td>
</tr> 
<tr>
    <td>&emsp;<a href="#demand-prediction">2.3 Demand Prediction</a></td>
    <td>&ensp;<a href="#travel-time-or-arrive-time-prediction">2.4 Travel time or Arrive time Prediction</a></td>
</tr>
<tr><td colspan="2"><a href="#datasets">3. Datasets</a></td></tr>
<tr>
    <td>&emsp;<a href="#sensor-data">3.1 Sensor data</a></td>
    <td>&ensp;<a href="#trajectory-data">3.2 Trajectory data</a></td>
</tr> 
<tr>
    <td>&emsp;<a href="#Others">3.3 others</a></td>
</tr> 
<tr><td colspan="2"><a href="#experts">4. Experts</a></td></tr> 
</table>
# [Survey papers](#content)

[1] **Urban Computing: Concepts, Methodologies, and Applications.** ACM Transactions on Intelligent Systems and Technology 2014. [paper](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/UrbanComputing-zheng-tist2014.pdf)

*YU ZHENG, LICIA CAPRA, OURI WOLFSON, HAI YANG*

---

[2] **Deep Learning for Spatio-Temporal Data Mining: A Survey.** IEEE Transactions on Knowledge and Data Engineering(TKDE) 2020. [paper](https://arxiv.org/pdf/1906.04928.pdf)

*Senzhang Wang, Jiannong Cao, Fellow, Philip S. Yu*

---

[3] **A Survey on Modern Deep Neural Network for Traffic Prediction: Trends, Methods and Challenges.** IEEE Transactions on Knowledge and Data Engineering(TKDE) 2020. [paper](https://ieeexplore.ieee.org/abstract/document/9112608)

*David Alexander Tedjopurnomo, Zhifeng Bao, Baihua Zheng, Farhana Murtaza Choudhury, Kai Qin*

---

[4] **How to Build a Graph-Based Deep Learning Architecture in Traffic Domain: A Survey.** arXiv 2020. [paper](https://arxiv.org/pdf/2005.11691.pdf)

*Jiexia Ye, Juanjuan Zhao, Kejiang Ye, Chengzhong Xu*

---

# [Applications](#content)

## [Traffic Prediction](#content)

[1] **[Spatio-Temporal Graph Structure Learning for Traffic Forecasting.](./papers/2020/AAAI/SLC)** AAAI 2020. [note](./papers/2020/AAAI/SLC/note.md), [paper](https://www.aaai.org/ojs/index.php/AAAI/article/view/5470).

| Models |  Modules   |                 Architecture                 | conclusion                                                   |
| :----- | :--------: | :------------------------------------------: | :----------------------------------------------------------- |
| SLC    | SLCNN, P3D | ![STGCN](./papers/2020/AAAI/SLC/img/SLC.png) | This paper proposes a new type of graph convolution formula. **The article mentions that it is necessary to learn not only the feature information on the graph, but also the structure information of the graph**, which means that the structure of the graph changes dynamically. Use P3D to model the time dependence. |

*Qi Zhang, Jianlong Chang, Gaofeng Meng, Shiming Xiang, Chunhong Pan*

---

[2] **GMAN: A Graph Multi-Attention Network for Traffic Prediction.** AAAI 2020. [note](./papers/2020/AAAI/GMAN/note.md), [paper](https://arxiv.org/pdf/1911.08415.pdf), [github](https://github.com/zhengchuanpan/GMAN)

| Models |                   Modules                    |                 Architecture                  | conclusion                                                   |
| :----: | :------------------------------------------: | :-------------------------------------------: | :----------------------------------------------------------- |
|  GMAN  | Encoder-Decoder,ST-Attention,Trans Attention | ![GMAN](./papers/2020/AAAI/GMAN/img/GMAN.png) | This paper proposes a spatial-temporal attention mechanism with gated fusion to simulate complex spatial-temporal correlation. |

*Chuanpan Zheng, Xiaoliang Fan, Cheng Wang, Jianzhong Qi*

---

[3] **Dynamic Graph Convolution Network for Traffic Forecasting Based on Latent Network of Laplace Matrix Estimation.** IEEE Transactions on Intelligent Transportation Systems(TITS) 2020. [note](./papers/2020/TITS/DGCN/note.md), [paper](https://ieeexplore.ieee.org/document/9190068)

| Models | Modules  |                  Architecture                   | conclusion                                                   |
| :----: | :------: | :---------------------------------------------: | :----------------------------------------------------------- |
|  DGCN  | TCL,GTCL | ![STSGCN](./papers/2020/TITS/DGCN/img/DGCN.png) | Different from most of the current GCN based methods, which generally used empirical graph Laplace matrix in graph convolution, this paper propose a latent network to estimate the dynamic Laplace matrix adaptively, which is verified with good ability to extract spatial-temporal correlation of the traffic data. |

*Kan Guo, Yongli Hu, ZhenQian, Yanfeng Sun, Junbin Gao, Baocai Yin*

---

[4] **Spatial-Temporal Synchronous Graph Convolutional Networks: A New Framework for Spatial-Temporal Network Data Forecasting.** AAAI 2020. [note](./papers/2020/AAAI/STSGCN/note.md), [paper](https://www.aaai.org/ojs/index.php/AAAI/article/view/5438), [github](https://github.com/Davidham3/STSGCN)

| Models |               Modules               |                    Architecture                     | conclusion                                                   |
| :----: | :---------------------------------: | :-------------------------------------------------: | :----------------------------------------------------------- |
| STSGCN | Spatial-Temporal Embedding, STSGCM, | ![STSGCN](./papers/2020/AAAI/STSGCN/img/STSGCN.png) | This paper proposes a new structured local spatio-temporal graph. By combining the graph structures of adjacent time slices into a local spatio-temporal graph, a new adjacency matrix is constructed, which can simultaneously capture spatio-temporal dependence. |

*Chao Song, Youfang Lin, Shengnan Guo, Huaiyu Wan*

---

<details><summary> 2019 </summary>

[1] **[Graph WaveNet for Deep Spatial-Temporal Graph Modeling.](./papers/2019/IJCAI/GWN)** IJCAI 2019. [note](./papers/2019/IJCAI/GWN/note.md). [paper](https://arxiv.org/abs/1906.00121), [github](https://github.com/nnzhan/Graph-WaveNet)

  *Zonghan Wu, Shirui Pan, Guodong Long, Jing Jiang, Chengqi Zhang*

<hr>

</details>

---

<details><summary> 2018 </summary>

[1] **[Spatio-Temporal Graph Convolutional Networks: A Deep Learning Framework for Traffic Forecasting.](./papers/2018/IJCAI/STGCN)** IJCAI 2018. [note](./papers/2018/IJCAI/STGCN/note.md), [paper](https://arxiv.org/pdf/1709.04875.pdf), [github](https://github.com/VeritasYin/STGCN_IJCAI-18).

  *Bing Yu, Haoteng Yin, Zhanxing Zhu*

<hr>
</details>



## [Flows Prediction](#content)


<details><summary> 2019 </summary>

[1] **[Graph WaveNet for Deep Spatial-Temporal Graph Modeling.](./papers/2019/IJCAI/GWN)** IJCAI 2019. [note](./papers/2019/IJCAI/GWN/note.md). [paper](https://arxiv.org/abs/1906.00121), [github](https://github.com/nnzhan/Graph-WaveNet)

  *Zonghan Wu, Shirui Pan, Guodong Long, Jing Jiang, Chengqi Zhang*

<hr>

</details>

---

<details><summary> 2018 </summary>

[1] **[Spatio-Temporal Graph Convolutional Networks: A Deep Learning Framework for Traffic Forecasting.](./papers/2018/IJCAI/STGCN)** IJCAI 2018. [note](./papers/2018/IJCAI/STGCN/note.md), [paper](https://arxiv.org/pdf/1709.04875.pdf), [github](https://github.com/VeritasYin/STGCN_IJCAI-18).

  *Bing Yu, Haoteng Yin, Zhanxing Zhu*

<hr>
</details>

## [Demand Prediction](#content)

[1] **Taxi Demand Prediction Using Parallel Multi-Task Learning Model.** TITS 2020. [note](), [paper](https://ieeexplore.ieee.org/document/9172100)

| Models | Modules | Architecture | conclusion |
| :----: | :-----: | :----------: | :--------: |
|        |         |              |            |

*Chizhan Zhang, Fenghua Zhu, Xiao Wang, Leilei Sun, Haina Tang, Yisheng Lv*

---

[2] **Traffic Demand Prediction Based on Dynamic Transition Convolutional Neural Network.** TITS 2020. [note](), [paper](https://ieeexplore.ieee.org/abstract/document/8968739)

| Models | Modules | Architecture | conclusion |
| :----: | :-----: | :----------: | :--------: |
|        |         |              |            |

*Bowen Du, Xiao Hu, Leilei Sun, Junming Liu, Yanan Qiao, Weifeng Lv*

---


<details><summary> 2019 </summary>

[1] **Origin-Destination Matrix Prediction via Graph Convolution: a New Perspective of Passenger Demand Modeling.** SIGKDD 2019. [note](), [paper](https://dl.acm.org/doi/abs/10.1145/3292500.3330877)

  *Yuandong Wang, Hongzhi Yin, Hongxu Chen, Tianyu Wo, Jie Xu, Kai Zheng*

<hr>

[2] **STG2Seq: Spatial-temporal Graph to Sequence Model for Multi-step Passenger Demand Forecasting.** IJCAI 2019. [paper](https://arxiv.org/abs/1905.10069)

  *Lei Bai, Lina Yao , Salil.S Kanhere, Xianzhi Wang, Quan.Z Sheng*

<hr>


</details>

---

<details><summary> 2018 </summary>

[1] **Deep Multi-View Spatial-Temporal Network for Taxi Demand Prediction.** AAAI 2018. [note](), [paper](https://arxiv.org/pdf/1802.08714.pdf)

  *Huaxiu Yao, Fei Wu, Jintao Ke, Xianfeng Tang, Yitian Jia, Siyu Lu, Pinghua Gong, Jieping Ye, Zhenhui Li*

<hr>
</details>

## [Travel time or Arrive time Prediction](#content)

**HetETA: Heterogeneous Information Network Embedding for Estimating Time of Arrival.** SIGKDD 2020. [note](), [paper](https://www.kdd.org/kdd2020/accepted-papers/view/heteta-heterogeneous-information-network-embedding-for-estimating-time-of-a), [github](https://github.com/didi/heteta)

| Models |    Modules     |        Architecture         | conclusion                                                   |
| :----: | :------------: | :-------------------------: | :----------------------------------------------------------- |
| HetETA | GatedCNNs, GCN | ![HetETA](./img/HetETA.png) | In this paper, traffic structure is constructed by digging deeper semantic information of traffic network. HetETA combines gated convolution neural networks and graph neural networks to capture the correlations in spatiotemporal information. |

*Huiting Hong, Yucheng Lin, Xiaoqing Yang, Zang Li, Kun Fu, Zheng Wang, Xiaohu Qie, Jieping Ye*

---

**CompactETA: A Fast Inference System for Travel Time Prediction.** KDD 2020. [note](), [paper](https://www.kdd.org/kdd2020/accepted-papers/view/compacteta-a-fast-inference-system-for-travel-time-prediction)

| Models | Modules | Architecture | conclusion |
| :----: | :-----: | :----------: | :--------: |
|        |         |              |            |

*Kun Fu, Fanlin Meng, Jieping Ye, Zheng Wang*

---




<details><summary> 2019 </summary>

[1] **Spatiotemporal Multi-Graph Convolution Network for Ride-hailing Demand Forecasting.** AAAI 2019. [paper](http://www-scf.usc.edu/~yaguang/papers/aaai19_multi_graph_convolution.pdf).

  *Xu Geng, Yaguang Li, Leye Wang, Lingyu Zhang, Qiang Yang, Jieping Ye, Yan Liu*

<hr>

</details>

---

<details><summary> 2018 </summary>

<hr>
</details>


# [Datasets](#content)

[1] GAIA Open Dataset: [link](https://outreach.didichuxing.com/research/opendata/)

[2] 智慧足迹: [link](http://www.smartsteps.com/)

## [Sensor data](#content)

[1] UK traffic flow datasets: [link](https://www.gov.uk/)

[2] Illinois traffic flow datasets: [link](http://www.travelmidwest.com/)

[3] PeMS: [link](http://pems.dot.ca.gov/), [Baidu Netdisk](https://pan.baidu.com/s/1c3NNV7nGnDylFJ9tBYUF0g) password:jutw | [PeMS Guide](https://github.com/Knowledge-Precipitation-Tribe/Urban-computing-papers/blob/master/PEMS.md)

## [Trajectory data](#content)

[1] Chengdu: [link](https://outreach.didichuxing.com/app-vue/TTItrajectory?id=1001)

[2] Xian: [link](https://outreach.didichuxing.com/app-vue/TTItrajectory?id=1001)

## [Others](#content)

[1] Weather and events data: [link](https://www.wunderground.com/)

[2] Weather and climate data: [link](https://www.ncdc.noaa.gov/data-access)

[3] NSW POI data: [link](https://sdi.nsw.gov.au/catalog/search/resource/details.page?uuid=%7BC41F6FE5-1C56-4556-%209EC6-EC9BD7094BBB%7D)

[4] Road network data: [link](http://networkrepository.com/road.php)

[5] NYC OpenData: [link](https://opendata.cityofnewyork.us/)

[6] METR-LA: [link](http://geohub.lacity.org/datasets/traffic-data?geometry=-119.170%2C33.900%2C-117.193%2C34.298), [Baidu Netdisk](https://pan.baidu.com/s/1g9yxZMDVf9nI0eN-ixeiPQ) password:xsz5

[7] TaxiBJ: [link](https://github.com/TolicWang/DeepST/tree/master/data/TaxiBJ), [Baidu Netdisk](https://pan.baidu.com/s/1aoi7gEkFQFn2MTYlGuc7Iw) password:sg4n

[8] BikeNYC: [link](https://www.citibikenyc.com/system-data), [Baidu Netdisk](https://pan.baidu.com/s/1SdSPWu5c761H3e8XjtzuaA) password:lmwj

[9] NYC-Taxi: [link](https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page), [Baidu Netdisk](https://pan.baidu.com/s/1W2UV-xiDG_wbM9tuPvfrsA) password:022y

[10] NYC-Bike: [link](https://www.citibikenyc.com/system-data)

[11] San Francisco taxi: [link](https://crawdad.org/)

[12] Chicago bike: [link](https://www.divvybikes.com/system-data)

[13] BikeDC: [link](https://www.capitalbikeshare.com/system-data)

# [Experts](#content)

(排名不分先后)

[1] Yu Zheng: [link](http://urban-computing.com/yuzheng)

[2] Yanhua Li: [link](http://users.wpi.edu/~yli15/index.html)

[3] Xun Zhou: [link](https://www.biz.uiowa.edu/faculty/xzhou/)

[4] YaGuang Li: [link](http://www-scf.usc.edu/~yaguang/)

[5] Zhenhui Jessie Li: [link](https://faculty.ist.psu.edu/jessieli/Site/index.html)

[6] David S. Rosenblum: [link](https://www.comp.nus.edu.sg/~david/)

[7] Huaiyu Wan: [link](http://faculty.bjtu.edu.cn/8793/)

[8] Junbo Zhang: [link](https://zhangjunbo.org/)

[9] Shining Xiang:[link](https://scholar.google.com/citations?hl=zh-CN&user=0ggsACEAAAAJ)


# Contributors

<a href="https://github.com/SuperSupeng"><img src="https://avatars2.githubusercontent.com/u/20471278?s=460&u=f62611f65c6c368293c0fd73b92aac7d7219b71&v=4" width=98px></img></a> <a href="https://github.com/Sylvia822"><img src="https://avatars0.githubusercontent.com/u/63226742?s=460&u=f8485c2378d4454cdedb483e35d9aa603e687e78&v=4" width=98px></img></a>

## LICENSE

<img alt="知识共享许可协议" src="https://camo.githubusercontent.com/75335faf011cd2856b147fa63e9ee383cc15a0a3/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6c6963656e73652d434325323042592d2d4e432d2d5341253230342e302d6c6967687467726579" data-canonical-src="https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey" style="max-width:100%;">

本作品采用<a href="http://creativecommons.org/licenses/by-nc-sa/4.0/" rel="nofollow">知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议</a>进行许可。