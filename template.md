# Title

项目介绍。

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
    <td>&ensp;<a href="#travel-time-or-arrive-time-prediction">3.4 Travel time or Arrive time Prediction</a></td>
</tr>
</table>

# [Survey papers](#content)



# [Applications](#content)

## [Traffic Prediction](#content)

[1] **Spatio-Temporal Graph Structure Learning for Traffic Forecasting.** AAAI 2020. [note](./papers/2020/AAAI/SLC/note.md) [paper](https://www.aaai.org/ojs/index.php/AAAI/article/view/5470).

| Models |  Modules   |                 Architecture                 | conclusion                                                   |
| :----- | :--------: | :------------------------------------------: | :----------------------------------------------------------- |
| SLC    | SLCNN, P3D | ![STGCN](./papers/2020/AAAI/SLC/img/SLC.png) | This paper proposes a new type of graph convolution formula. ***\*The article mentions that it is necessary to learn not only the feature information on the graph, but also the structure information of the graph\****, which means that the structure of the graph changes dynamically. Use P3D to model the time dependence. |

*Qi Zhang, Jianlong Chang, Gaofeng Meng, Shiming Xiang, Chunhong Pan*

---

[2] **GMAN: A Graph Multi-Attention Network for Traffic Prediction.** AAAI 2020. [paper](https://arxiv.org/pdf/1911.08415.pdf), [github](https://github.com/zhengchuanpan/GMAN)
| Models |                   Modules                    |                 Architecture                  | conclusion                                                   |
| :----: | :------------------------------------------: | :-------------------------------------------: | :----------------------------------------------------------- |
|  GMAN  | Encoder-Decoder,ST-Attention,Trans Attention | ![GMAN](./papers/2020/AAAI/GMAN/img/GMAN.png) | This paper proposes a spatial-temporal attention mechanism with gated fusion to simulate complex spatial-temporal correlation. |

*Chuanpan Zheng, Xiaoliang Fan, Cheng Wang, Jianzhong Qi*

---

<details><summary> 2018 </summary>
[1] **[Spatio-Temporal Graph Convolutional Networks: A Deep Learning Framework for Traffic Forecasting.](./papers/2018/IJCAI/STGCN)** IJCAI 2018. [note](./papers/2018/IJCAI/STGCN/note.md) [paper](https://arxiv.org/pdf/1709.04875.pdf), [github](https://github.com/VeritasYin/STGCN_IJCAI-18).

  *Bing Yu, Haoteng Yin, Zhanxing Zhu*
<hr>
[2] **[Graph WaveNet for Deep Spatial-Temporal Graph Modeling.](./papers/2018/IJCAI/GWN)** IJCAI 2019. [note](./papers/2019/IJCAI/GWN/note.md) [paper](https://arxiv.org/abs/1906.00121), [github](https://github.com/nnzhan/Graph-WaveNet)

  *Zonghan Wu, Shirui Pan, Guodong Long, Jing Jiang, Chengqi Zhang*
<hr>
</details>


## [Flows Prediction](#content)

## [Demand Prediction](#content)

## [Travel time or Arrive time Prediction](#content)


# Contributors

<a href="https://github.com/SuperSupeng"><img src="https://avatars2.githubusercontent.com/u/20471278?s=460&u=f62611f65c6c368293c0fd73b92aac7d7219b71&v=4" width=98px></img></a> <a href="https://github.com/Sylvia822"><img src="https://avatars0.githubusercontent.com/u/63226742?s=460&u=f8485c2378d4454cdedb483e35d9aa603e687e78&v=4" width=98px></img></a>

## LICENSE

<img alt="知识共享许可协议" src="https://camo.githubusercontent.com/75335faf011cd2856b147fa63e9ee383cc15a0a3/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6c6963656e73652d434325323042592d2d4e432d2d5341253230342e302d6c6967687467726579" data-canonical-src="https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey" style="max-width:100%;">

本作品采用<a href="http://creativecommons.org/licenses/by-nc-sa/4.0/" rel="nofollow">知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议</a>进行许可。