[English](README_en.md) | 中文

# PaddleVideo

## 近期更新

- 发布轻量化行为识别模型🌟[PP-TSMv2](./docs/zh-CN/model_zoo/recognition/pp-tsm.md)🌟, Kinetics-400精度74.38%，25fps的10s视频cpu推理时间仅需433ms.
- 新增[知识蒸馏](./docs/zh-CN/distillation.md)功能.
- 发布各模型[benchmark](./docs/zh-CN/benchmark.md)文档.
- 更新[快速开始](./docs/zh-CN/quick_start.md)文档.
- 新增基于transformer的行为识别模型[TokenShift](https://github.com/PaddlePaddle/PaddleVideo/blob/develop/docs/zh-CN/model_zoo/recognition/tokenshift_transformer.md).
- 新增基于骨骼点的行为识别模型[2s-ACGN](https://github.com/PaddlePaddle/PaddleVideo/blob/develop/docs/zh-CN/model_zoo/recognition/agcn2s.md)、[CTR-GCN](./docs/zh-CN/model_zoo/recognition/ctrgcn.md).


👀 🌟  **《产业级视频技术与应用案例》系列课程回放链接**:  https://aistudio.baidu.com/aistudio/course/introduce/6742 🌟

​																	  💖 **欢迎大家扫码入群讨论** 💖
<div align="center">
  <img src="docs/images/user_group.png" width=250/></div>

- 添加成功后回复【视频】加入交流群

## 简介

![python version](https://img.shields.io/badge/python-3.7+-orange.svg) ![paddle version](https://img.shields.io/badge/PaddlePaddle-2.0-blue)


PaddleVideo是[飞桨官方](https://www.paddlepaddle.org.cn/?fr=paddleEdu_github)出品的视频模型开发套件，旨在帮助开发者更好的进行视频领域的学术研究和产业实践。

<div align="center">
  <img src="docs/images/home.gif" width="450px"/><br>
</div>


## 模型案例库

### 模型

- 模型库使用前请参考[安装说明](docs/zh-CN/install.md)、[使用指南](docs/zh-CN/usage.md)。

<table style="margin-left:auto;margin-right:auto;font-size:1.3vw;padding:3px 5px;text-align:center;vertical-align:center;">
  <tr>
    <td colspan="5" style="font-weight:bold;">行为识别方法</td>
  </tr>
  <tr>
    <td><a href="./docs/zh-CN/model_zoo/recognition/pp-tsm.md">PP-TSM</a> (PP series)</td>
    <td><a href="./docs/zh-CN/model_zoo/recognition/pp-tsn.md">PP-TSN</a> (PP series)</td>
    <td><a href="./docs/zh-CN/model_zoo/recognition/pp-timesformer.md">PP-TimeSformer</a> (PP series)</td>
    <td><a href="./docs/zh-CN/model_zoo/recognition/tsn.md">TSN</a> (2D’)</td>
    <td><a href="./docs/zh-CN/model_zoo/recognition/tsm.md">TSM</a> (2D‘)</td>
  <tr>
    <td><a href="./docs/zh-CN/model_zoo/recognition/slowfast.md">SlowFast</a> (3D’)</td>
    <td><a href="./docs/zh-CN/model_zoo/recognition/timesformer.md">TimeSformer</a> (Transformer‘)</td>
    <td><a href="./docs/zh-CN/model_zoo/recognition/videoswin.md">VideoSwin</a> (Transformer’)</td>
    <td><a href="./docs/zh-CN/model_zoo/recognition/attention_lstm.md">AttentionLSTM</a> (RNN‘)</td>
    <td><a href="./docs/zh-CN/model_zoo/recognition/movinet.md">MoViNet</a> (Lite‘)</td>
  </tr>
  <tr>
    <td colspan="5" style="font-weight:bold;">基于骨骼点的动作识别方法</td>
  </tr>
  <tr>
    <td><a href="./docs/zh-CN/model_zoo/recognition/stgcn.md">ST-GCN</a> (GCN’)</td>
    <td><a href="./docs/zh-CN/model_zoo/recognition/agcn.md">AGCN</a> (GCN‘)</td>
    <td><a href="./docs/zh-CN/model_zoo/recognition/ctrgcn.md">CTR-GCN</a> (GCN‘)</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td colspan="5" style="font-weight:bold;">时序动作检测方法</td>
  </tr>
  <tr>
    <td><a href="./docs/zh-CN/model_zoo/localization/bmn.md">BMN</a> (One-stage‘)</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td colspan="5" style="font-weight:bold;">视频时序分割</td>
  </tr>
  <tr>
    <td><a href="./docs/zh-CN/model_zoo/segmentation/mstcn.md">MS-TCN</a> </td>
    <td><a href="./docs/zh-CN/model_zoo/segmentation/asrf.md">ASRF</a> </td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td colspan="5" style="font-weight:bold;">时空动作检测方法</td>
  </tr>
  <tr>
    <td><a href="docs/zh-CN/model_zoo/detection/SlowFast_FasterRCNN.md">SlowFast+Fast R-CNN</a>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td colspan="5" style="font-weight:bold;">多模态</td>
  </tr>
  <tr>
    <td><a href="./docs/zh-CN/model_zoo/multimodal/actbert.md">ActBERT</a> (Learning‘)</td>
    <td><a href="./applications/T2VLAD/README.md">T2VLAD</a> (Retrieval‘)</td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td colspan="5" style="font-weight:bold;">视频目标分割</td>
  </tr>
  <tr>
    <td><a href="./docs/zh-CN/model_zoo/segmentation/cfbi.md">CFBI</a> (Semi‘)</td>
    <td><a href="./applications/EIVideo/EIVideo/docs/zh-CN/manet.md">MA-Net</a> (Supervised‘)</td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td colspan="5" style="font-weight:bold;">单目深度估计</td>
  </tr>
  <tr>
    <td><a href="./docs/zh-CN/model_zoo/estimation/adds.md">ADDS</a> (Unsupervised‘)</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
</table>


### 数据集

<table>
  <tbody><tr>
    <td colspan="4">动作识别</td>
  </tr>
  <tr>
    <td><a href="docs/zh-CN/dataset/k400.md">Kinetics-400</a> (<a href="https://deepmind.com/research/open-source/kinetics/" rel="nofollow">Homepage</a>) (CVPR'2017)</td>
    <td><a href="docs/zh-CN/dataset/ucf101.md">UCF101</a> (<a href="https://www.crcv.ucf.edu/research/data-sets/ucf101/" rel="nofollow">Homepage</a>) (CRCV-IR-12-01)</td>
    <td><a href="docs/zh-CN/dataset/ActivityNet.md">ActivityNet</a> (<a href="http://activity-net.org/" rel="nofollow">Homepage</a>) (CVPR'2015)</td>
    <td><a href="docs/zh-CN/dataset/youtube8m.md">YouTube-8M</a> (<a href="https://research.google.com/youtube8m/" rel="nofollow">Homepage</a>) (CVPR'2017)</td>
  </tr>
  <tr>
    <td colspan="4">动作定位</td>
  </tr>
  <tr>
    <td><a href="docs/zh-CN/dataset/ActivityNet.md">ActivityNet</a> (<a href="http://activity-net.org/" rel="nofollow">Homepage</a>) (CVPR'2015)</td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td colspan="4">时空动作检测</td>
  </tr>
  <tr>
    <td><a href="docs/zh-CN/dataset/AVA.md">AVA</a> (<a href="https://research.google.com/ava/index.html" rel="nofollow">Homepage</a>) (CVPR'2018)</td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td colspan="4">基于骨架的动作识别</td>
  </tr>
  <tr>
    <td><a href="docs/zh-CN/dataset/ntu-rgbd.md">NTURGB+D</a> (<a href="https://rose1.ntu.edu.sg/dataset/actionRecognition/" rel="nofollow">Homepage</a>) (IEEE CS'2016)</td>
    <td><a href="docs/zh-CN/dataset/fsd.md">FSD</a> (<a href="https://aistudio.baidu.com/aistudio/competition/detail/115/0/introduction" rel="nofollow">Homepage</a>)</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td colspan="4">单目深度估计</td>
  </tr>
  <tr>
    <td><a href="docs/zh-CN/dataset/Oxford_RobotCar.md">Oxford-RobotCar</a> (<a href="https://robotcar-dataset.robots.ox.ac.uk/" rel="nofollow">Homepage</a>) (IJRR'2017)</td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td colspan="4">文本视频检索</td>
  </tr>
  <tr>
    <td><a href="docs/zh-CN/dataset/msrvtt.md">MSR-VTT</a> (<a href="https://www.microsoft.com/en-us/research/publication/msr-vtt-a-large-video-description-dataset-for-bridging-video-and-language/" rel="nofollow">Homepage</a>) (CVPR'2016)</td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td colspan="4">文本视频预训练</td>
  </tr>
  <tr>
    <td><a href="docs/zh-CN/dataset/howto100m.md">HowTo100M</a> (<a href="https://www.di.ens.fr/willow/research/howto100m/" rel="nofollow">Homepage</a>) (ICCV'2019)</td>
    <td></td>
    <td></td>
    <td></td>
  </tr>

</tbody>
</table>


### 应用案例

| Applications | Descriptions |
| :--------------- | :-------- |
| [FootballAction](applications/FootballAction) | 足球动作检测方案|
| [BasketballAction](applications/BasketballAction) | 篮球动作检测方案 |
| [TableTennis](applications/TableTennis) | 乒乓球动作识别方案|
| [FigureSkating](applications/FigureSkating) | 花样滑冰动作识别方案|
| [VideoTag](applications/VideoTag) | 3000类大规模视频分类方案 |
| [MultimodalVideoTag](applications/MultimodalVideoTag) | 多模态视频分类方案|
| [VideoQualityAssessment](applications/VideoQualityAssessment) | 视频质量评估方案|
| [PP-Care](applications/PP-Care) | 3DMRI医疗图像识别方案 |
| [EIVideo](applications/EIVideo) | 视频交互式分割工具|
| [Anti-UAV](applications/Anti-UAV) |无人机检测方案|
| [AbnormalActionDetection](applications/AbnormalActionDetection) |异常行为检测方案|
| [PP-Human](applications/PPHuman) | 行人分析场景动作识别方案 |


## 文档教程
- AI-Studio教程
    - [【官方】Paddle 2.1实现视频理解优化模型 -- PP-TSM](https://aistudio.baidu.com/aistudio/projectdetail/3399656?contributionType=1)
    - [【官方】Paddle 2.1实现视频理解优化模型 -- PP-TSN](https://aistudio.baidu.com/aistudio/projectdetail/2879980?contributionType=1)
    - [【官方】Paddle 2.1实现视频理解经典模型 -- TSN](https://aistudio.baidu.com/aistudio/projectdetail/2250682)
    - [【官方】Paddle 2.1实现视频理解经典模型 -- TSM](https://aistudio.baidu.com/aistudio/projectdetail/2310889)
    - [BMN视频动作定位](https://aistudio.baidu.com/aistudio/projectdetail/2250674)
    - [花样滑冰选手骨骼点动作识别ST-GCN教程](https://aistudio.baidu.com/aistudio/projectdetail/2417717)
    - [【实践】CV领域的Transformer模型TimeSformer实现视频理解](https://aistudio.baidu.com/aistudio/projectdetail/3413254?contributionType=1)
- 贡献代码
    - [如何添加新算法](./docs/zh-CN/contribute/add_new_algorithm.md)
    - [配置系统设计解析](./docs/en/tutorials/config.md)
    - [如何提pr](./docs/zh-CN/contribute/how_to_contribute.md)


## 赛事支持

- [基于飞桨实现花样滑冰选手骨骼点动作识别大赛](https://aistudio.baidu.com/aistudio/competition/detail/115/0/introduction), [AI Studio项目](https://aistudio.baidu.com/aistudio/projectdetail/2417717), [视频教程](https://www.bilibili.com/video/BV1w3411172G)
- [基于飞桨实现乒乓球时序动作定位大赛](https://aistudio.baidu.com/aistudio/competition/detail/127/0/introduction)
- [CCKS 2021：知识增强的视频语义理解](https://www.biendata.xyz/competition/ccks_2021_videounderstanding/)

## 许可证书
本项目的发布受[Apache 2.0 license](LICENSE)许可认证。

## 致谢
- 非常感谢 [mohui37](https://github.com/mohui37)、[zephyr-fun](https://github.com/zephyr-fun)、[voipchina](https://github.com/voipchina) 贡献相关代码
