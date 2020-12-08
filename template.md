# Introduction

用于做项目介绍。

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

**Qi Zhang, Jianlong Chang, Gaofeng Meng, Shiming Xiang, Chunhong Pan**

---

<details><summary> 2018 </summary>
[2] **Spatio-Temporal Graph Convolutional Networks: A Deep Learning Framework for Traffic Forecasting.** IJCAI 2018. **[note](./papers/2018/IJCAI/STGCN/note.md)** [paper](https://arxiv.org/pdf/1709.04875.pdf), [github](https://github.com/VeritasYin/STGCN_IJCAI-18).
| Models |    Modules    |                   Architecture                    | conclusion                                                   |
| :----- | :-----------: | :-----------------------------------------------: | :----------------------------------------------------------- |
| STGCN  | GCN,Gated CNN | ![STGCN](./papers/2018/IJCAI/STGCN/img/STGCN.png) | This paper uses GCN to model spatial dependence, temporal dependence modeling uses causal convolution, and uses the gating mechanism GLU. The bottleneck strategy is used in the structure to achieve feature compression. This paper is also the first application of GCN in the field of transportation. |
*Bing Yu, Haoteng Yin, Zhanxing Zhu*
---
## [Flows Prediction](#content)

## [Demand Prediction](#content)

## [Travel time or Arrive time Prediction](#content)



