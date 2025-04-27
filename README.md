# 颜色组学习资料分享


前言：为了帮助同学更快地了解和融入颜色课题组，找到属于自己的研究方向，特拟该资料。

## 该课题成立时间

2020年11月

## 项目组成员

2名老师，一名博士生，3名硕士生

## 研究方向

| 方向 | 描述 | 可能技术 |
| ---- | ---- | ---- |
| 美平衡 | 调整图像构图、色彩搭配等元素，实现视觉上的和谐美感，提升艺术价值 | \ |
| 人像Relighting | 对人像图像重新打光，改变光照效果以达到不同视觉氛围和艺术效果 | \ |
| 白平衡 | 用sRGB图像白平衡技术调整图像色彩平衡，还原真实色彩 | 元学习、对比学习 |
| 颜色恒常性 | 采用RAW图像白平衡技术，确保不同光照下物体颜色视觉感知稳定 | 迁移学习、对抗学习、多域学习 |
| HDR | 实现高动态范围图像重建，提升亮部和暗部细节与对比度 | 基于深度学习的图像生成技术、融合多帧图像算法、生成对抗网络 |
| 图像分割 | 对夜间图像进行分割，划分不同目标或区域以便后续处理 | 结合夜间图像特性的深度神经网络、注意力机制算法、半监督学习算法 |
| 图像抠图 | 在高分辨率下精准抠图，分离前景和背景 | 多任务学习、模型轻量化技术 |

- 正在进行的研究：美平衡，relighting，颜色恒常性

## 颜色恒常性背景
+ 定义：相机拍摄的原始RAW图像会受到外界非中性光影响，导致拍摄图像发生色偏，颜色恒常性就是消除色偏现象保持物体本来颜色的过程。
+ 步骤：光照估计：估计出物体表面的光照颜色；颜色矫正，去除光照色偏影响。
+ 示意图如下所示：<img src="https://github.com/ChunxiaoLe/CCC/blob/main/%E9%A2%9C%E8%89%B2%E6%81%92%E5%B8%B8%E6%80%A7%E8%83%8C%E6%99%AF.png" width = "550" height = "300" alt="" align=center />

## 实验室自研颜色恒常性代码库平台Anole[[link]](https://github.com/YuxiangTang/Anole)
+ 目的：提供规范化的图像处理框架；提供稳定、公平、可比较的平台；补充RAW图像处理缺口.
+ 主要模块：
  + RAW图像处理：RAW图像在相机前后端的处理功能。
  + 颜色恒常性模型：在同一套框架下提供流行和常用颜色恒常性模型。
  + 模型训练和验证：规范化颜色恒常性训练、测试、评价流程。
  + 实验环境配置：Hydra 和可视化技术生成报告来管理实验。

## 组内已投中顶会顶刊：
+ Yuxiang Tang, Xuejing Kang, Chunxiao Li, Zhaowen Lin, Anlong Ming*, Transfer Learning for Color Constancy via Statistic Perspective, AAAI 2022, 人工智能领域顶会. [[pdf]](https://ojs.aaai.org/index.php/AAAI/article/download/20135/19894)  [[code]](https://github.com/YuxiangTang/TLCC)
+ Zhifeng Zhang, Xuejing Kang, Anlong Ming*, Domain Adversarial Learning for Color Constancy,IJCAI 2022，人工智能领域顶会.  [[pdf]](https://www.ijcai.org/proceedings/2022/0236.pdf)  [[code]](https://github.com/Zhi-Feng-Zhang/DALCC)
+ Chunxiao Li, Xuejing Kang, Zhifeng Zhang, Anlong Ming*, SWBNet: A Stable White Balance Network for sRGB images, AAAI 2023, 人工智能领域顶会. [[pdf]](https://github.com/ChunxiaoLe/SWBNet/blob/master/paper/9786.ChunxiaoLi.pdf) [[code]](https://github.com/ChunxiaoLe/SWBNet)
+ Chunxiao Li, Xuejing Kang, Anlong Ming*, WBFlow: Few-shot White Balance for sRGB Images via Reversible Neural Flows，IJCAI 2023, 人工智能领域顶会.
+ Chenghao Dong, Xuejing Kang, Anlong Ming, ICDA: Illumination-Coupled Domain Adaptation Framework for Unsupervised Nighttime Semantic Segmentation,IJCAI 2023, 人工智能领域顶会.
+ 在投3篇

## Demos:

https://github.com/ChunxiaoLe/CCC_Tutorial/assets/58202703/4273e625-b831-4371-96ce-bc33d2bb1d19






https://github.com/ChunxiaoLe/CCC_Tutorial/assets/58202703/7567d5a1-82a4-4f1d-a76e-2dc86cd2efe2






## 其它资料：
+ *博客：RAW图像到sRGB图像的全过程*  [[code]](https://ridiqulous.com/process-raw-data-using-matlab-and-dcraw/comment-page-3/#comments)
+ *公开课：RAW图像处理全流程代码* [[code]](https://nbviewer.jupyter.org/github/yourwanghao/CMUComputationalPhotography/blob/master/class2/notebook2.ipynb)
+ 经典论文：Hu, Yuanming and Wang, Baoyuan and Lin, Stephen: "*Fc4: Fully convolutional color constancy with confidence-weighted pooling*" CVPR (2017) [[pdf]](https://openaccess.thecvf.com/content_cvpr_2017/papers/Hu_FC4_Fully_Convolutional_CVPR_2017_paper.pdf) [[code]](https://github.com/yuanming-hu/fc4)
+ 经典论文：Lo Y C, Chang C C, Chiu H C, et al. : "*Clcc: Contrastive learning for color constancy*" CVPR (2021) [[pdf]](https://openaccess.thecvf.com/content/CVPR2021/papers/Lo_CLCC_Contrastive_Learning_for_Color_Constancy_CVPR_2021_paper.pdf) [[code]](https://openaccess.thecvf.com/content/CVPR2021/papers/Lo_CLCC_Contrastive_Learning_for_Color_Constancy_CVPR_2021_paper.pdf)



可用数据集
--------------
各类颜色恒常性数据集大全[dataset](http://colorconstancy.com/evaluation/datasets/index.html)，数据集处理可参考链接[link](https://github.com/ChunxiaoLe/CCC/blob/main/color_constancy_data_process_all.py)

| 数据集名称  | 数据集描述  | 数据集规模    |   作用   | 链接|
| :-----------: | :--------: | :--------: | :--------: | :--------: |
| CCC | 经典单光照数据集 | 568张照片 | 评价单光照颜色恒常性性能 | [link](https://www2.cs.sfu.ca/~colour/data/shi_gehler/) |
| NUS8 | 单光照+8相机数据集| 1700+图像 | 评价单光照颜色恒常性性能、跨相机性能| [link](https://cvil.eecs.yorku.ca/projects/public_html/illuminant/illuminant.html) |
| Cube+ | 单光照+双光照数据集、立方蜘蛛 | 1700+张图像 | 评价单光照和双光照颜色恒常性性能 | [link](https://ipg.fer.hr/ipg/resources/color_constancy) |
| LSMI | 大规模多光照数据集 |7,486张图像 | 评价多光照颜色恒常性性能 | [link](https://github.com/DY112/LSMI-dataset) |

## 理论知识
+ "*李宏毅机器学习课程.*" 哔哩哔哩 [[link]](https://www.bilibili.com/video/BV1JE411g7XF?from=search&seid=16114573361443816126)

## 动手实践
+ "*动手学深度学习(PyTorch版).*" GitHub [[link]](https://tangshusen.me/Dive-into-DL-PyTorch/#/)
+ "*深度学习框架PyTorch：入门与实践.*" GitHub [[link]](https://github.com/chenyuntc/pytorch-book)




## 其它工具
+ "*Zotero.*" 论文整理工具 [[link]](https://www.zotero.org/)
+ "*connectedpapers.*" 论文追溯工具 [[link]](https://www.connectedpapers.com/)
+ "*Paperswithcode.*" 论文代码查找工具 [[link]](https://paperswithcode.com/)
+ "*Google colab.*" 免费线上GPU平台，如额外需要线下服务器资源，请联系负责管理GPU的同学 [[link]](https://colab.research.google.com/notebooks/intro.ipynb)


