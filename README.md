# 颜色组学习资料分享


前言：为了帮助同学更快地了解和融入颜色课题组，找到属于自己的研究方向，特拟该资料。

## 该课题成立时间

2020年11月

## 项目组成员

2名老师，1名博士生，3名硕士生

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

## 必备技能
- python教程：
  - [python快速入门](https://www.bilibili.com/video/BV14v411V7Xe/?spm_id_from=333.1387.upload.video_card.click)
  - [python核心编程](https://www.bilibili.com/video/BV1AN4y137uT/?spm_id_from=333.1387.upload.video_card.click)
  - [python高阶](https://www.bilibili.com/video/BV1FS4y1v7CW/?spm_id_from=333.1387.upload.video_card.click)
- pytorch教程：
  - [入门](https://space.bilibili.com/18161609/lists/48290?type=season)
  - [入门](https://www.bilibili.com/video/BV1hE411t7RN/?spm_id_from=333.337.search-card.all.click)
- 深度学习教程：[【機器學習2021】(中文版)](https://www.youtube.com/playlist?list=PLJV_el3uVTsMhtt7_Y6sgTHGHp1Vb2P2J)
- 论文写作相关：[论文写作、阅读指导、常用工具](https://pan.baidu.com/s/1_h2g5WFKUPWct-7fCGIAMg?pwd=ysmx ), 提取码:[ysmx]
## 美平衡
### 什么是美平衡

- 概念
  - 白平衡：要理解美平衡，首先要知道什么是白平衡(Auto-White-Balance,AWB)，所谓的白平衡简单理解就是让相机拍摄出来的物体，无论在什么光源场景下，最终所呈现出来的视觉效果都和白光下一样
  - 美平衡：与AWB不同，A-AWB在用户可接受的颜色保真范围内，结合用户的审美偏好和通用颜色美学，进行用户定制的最美图像颜色渲染

- 示例展示

<div align="center">
  <img src="https://github.com/user-attachments/assets/92d0f7b1-74dd-4fb5-80c1-d1b0dfc7f51b" alt="image" />
</div>

### 入门参考论文
- Deep White-Balance Editing,[[paper]](https://openaccess.thecvf.com/content_CVPR_2020/papers/Afifi_Deep_White-Balance_Editing_CVPR_2020_paper.pdf),[[code]](https://github.com/mahmoudnafifi/Deep_White_Balance)
- A Software Platform for Manipulating the Camera Imaging Pipeline,[[paper]](https://karaimer.github.io/camera-pipeline/paper/Karaimer_Brown_ECCV16.pdf),[[code]](https://karaimer.github.io/camera-pipeline/)
- When Color Constancy Goes Wrong:  Correcting Improperly White-Balanced Images,[[paper]](https://openaccess.thecvf.com/content_CVPR_2019/papers/Afifi_When_Color_Constancy_Goes_Wrong_Correcting_Improperly_White-Balanced_Images_CVPR_2019_paper.pdf),[[code]](https://github.com/mahmoudnafifi/WB_sRGB)
- ALL-E: Aesthetics-guided Low-light Image Enhancement,[[paper]](https://www.ijcai.org/proceedings/2023/0118.pdf),[[code]](https://github.com/gaoyuanhang/ALL-E)
- Physically-plausible illumination distribution estimation,[[paper]](https://openaccess.thecvf.com/content/ICCV2023/papers/Ershov_Physically-Plausible_Illumination_Distribution_Estimation_ICCV_2023_paper.pdf),[[code]](https://github.com/createcolor/IDE?tab=readme-ov-file)

### 领域知名实验室




## 人像Relighting
### 什么是人像Relighting

- 概念：人像Relighting是一种通过调整人像照片的光照条件，以实现不同光照效果的技术。它可以帮助修复拍摄时因光照不足或不理想导致的问题，甚至创造出全新的光影效果，增强照片的艺术感和真实感。这种技术可以应用于多种场景，包括摄影后期处理、影视特效制作、虚拟现实和增强现实、游戏开发以及广告与商业图像制作等‌。
- 示例展示：


<div align="center">
  <video src="https://github.com/user-attachments/assets/086aaf1c-55fc-415c-9ecd-205298cbbda8" controls width="600"></video>
</div>


### 入门参考论文
+ Zhou H, Hadap S, Sunkavalli K, et al. : "*Deep Single-Image Portrait Relighting*" ICCV (2019) [[paper]](https://openaccess.thecvf.com/content_ICCV_2019/papers/Zhou_Deep_Single-Image_Portrait_Relighting_ICCV_2019_paper.pdf) [[code]](https://zhhoper.github.io/dpr.html)
+ Hou A, Zhang Z, Sarkis M, et al. : "*Towards high fidelity face relighting with realistic shadows*" CVPR (2021) [[paper]](https://openaccess.thecvf.com/content/CVPR2021/papers/Hou_Towards_High_Fidelity_Face_Relighting_With_Realistic_Shadows_CVPR_2021_paper.pdf) [[code]](https://github.com/andrewhou1/Shadow-Mask-Face-Relighting)
+ Hou A, Sarkis M, Bi N, et al. : "*Face Relighting with Geometrically Consistent Shadows*" CVPR (2022) [[paper]](https://openaccess.thecvf.com/content/CVPR2022/papers/Hou_Face_Relighting_With_Geometrically_Consistent_Shadows_CVPR_2022_paper.pdf) [[code]](https://github.com/andrewhou1/GeomConsistentFR)
+ Ponglertnapakorn P, Tritrong N, Suwajanakorn S: "*DiFaReli: Diffusion Face Relighting*" ICCV (2023) [[paper]](https://openaccess.thecvf.com/content/ICCV2023/papers/Ponglertnapakorn_DiFaReli_Diffusion_Face_Relighting_ICCV_2023_paper.pdf) [[code]](https://diffusion-face-relighting.github.io)

### 交互应用
+ IC-Light [[code]](https://github.com/lllyasviel/IC-Light)
+ LuminaBrush [[code]](https://github.com/lllyasviel/LuminaBrush)
+ ClipDrop [[web]](https://clipdrop.co/relight)


## 颜色恒常性

### 什么是颜色恒常性
+ 定义：相机拍摄的原始RAW图像会受到外界非中性光影响，导致拍摄图像发生色偏，颜色恒常性就是消除色偏现象保持物体本来颜色的过程。
+ 步骤：光照估计：估计出物体表面的光照颜色；颜色矫正，去除光照色偏影响。
+ 示意图如下所示：


<div align="center">
  <img src="https://github.com/ChunxiaoLe/CCC/blob/main/%E9%A2%9C%E8%89%B2%E6%81%92%E5%B8%B8%E6%80%A7%E8%83%8C%E6%99%AF.png?raw=true" width="550" height="300" alt=""/>
</div>

### 入门资料：
- *博客：RAW图像到sRGB图像的全过程*  [[link]](https://ridiqulous.com/process-raw-data-using-matlab-and-dcraw/comment-page-3/#comments)
- *公开课：RAW图像处理全流程代码* [[linke]](https://nbviewer.jupyter.org/github/yourwanghao/CMUComputationalPhotography/blob/master/class2/notebook2.ipynb)
- 经典论文
  - Hu, Yuanming and Wang, Baoyuan and Lin, Stephen: "*Fc4: Fully convolutional color constancy with confidence-weighted pooling*" CVPR (2017) [[paper]](https://openaccess.thecvf.com/content_cvpr_2017/papers/Hu_FC4_Fully_Convolutional_CVPR_2017_paper.pdf) [[code]](https://github.com/yuanming-hu/fc4)
  - Lo Y C, Chang C C, Chiu H C, et al. : "*Clcc: Contrastive learning for color constancy*" CVPR (2021) [[paper]](https://openaccess.thecvf.com/content/CVPR2021/papers/Lo_CLCC_Contrastive_Learning_for_Color_Constancy_CVPR_2021_paper.pdf) [[code]](https://openaccess.thecvf.com/content/CVPR2021/papers/Lo_CLCC_Contrastive_Learning_for_Color_Constancy_CVPR_2021_paper.pdf)

  
### 实验室自研代码平台
- Anole[[link]](https://github.com/YuxiangTang/Anole)
- 目的：提供规范化的图像处理框架；提供稳定、公平、可比较的平台；补充RAW图像处理缺口.
- 主要模块：
  - RAW图像处理：RAW图像在相机前后端的处理功能。
  - 颜色恒常性模型：在同一套框架下提供流行和常用颜色恒常性模型。
  - 模型训练和验证：规范化颜色恒常性训练、测试、评价流程。
  - 实验环境配置：Hydra 和可视化技术生成报告来管理实验。

### Demos:


<div align="center">
  <video src="https://github.com/ChunxiaoLe/CCC_Tutorial/assets/58202703/4273e625-b831-4371-96ce-bc33d2bb1d19" controls width="600"></video>
</div>



<div align="center">
  <video src="https://github.com/ChunxiaoLe/CCC_Tutorial/assets/58202703/7567d5a1-82a4-4f1d-a76e-2dc86cd2efe2" controls width="600"></video>
</div>








可用数据集
--------------
各类颜色恒常性数据集大全[dataset](http://colorconstancy.com/evaluation/datasets/index.html)，数据集处理可参考链接[link](https://github.com/ChunxiaoLe/CCC/blob/main/color_constancy_data_process_all.py)

| 数据集名称  | 数据集描述  | 数据集规模    |   作用   | 链接|
| :-----------: | :--------: | :--------: | :--------: | :--------: |
| CCC | 经典单光照数据集 | 568张照片 | 评价单光照颜色恒常性性能 | [link](https://www2.cs.sfu.ca/~colour/data/shi_gehler/) |
| NUS8 | 单光照+8相机数据集| 1700+图像 | 评价单光照颜色恒常性性能、跨相机性能| [link](https://cvil.eecs.yorku.ca/projects/public_html/illuminant/illuminant.html) |
| Cube+ | 单光照+双光照数据集、立方蜘蛛 | 1700+张图像 | 评价单光照和双光照颜色恒常性性能 | [link](https://ipg.fer.hr/ipg/resources/color_constancy) |
| LSMI | 大规模多光照数据集 |7,486张图像 | 评价多光照颜色恒常性性能 | [link](https://github.com/DY112/LSMI-dataset) |


## 组内已投中顶会顶刊：
+ Yuxiang Tang, Xuejing Kang, Chunxiao Li, Zhaowen Lin, Anlong Ming*, Transfer Learning for Color Constancy via Statistic Perspective, AAAI 2022, 人工智能领域顶会. [[pdf]](https://ojs.aaai.org/index.php/AAAI/article/download/20135/19894)  [[code]](https://github.com/YuxiangTang/TLCC)
+ Zhifeng Zhang, Xuejing Kang, Anlong Ming*, Domain Adversarial Learning for Color Constancy,IJCAI 2022，人工智能领域顶会.  [[pdf]](https://www.ijcai.org/proceedings/2022/0236.pdf)  [[code]](https://github.com/Zhi-Feng-Zhang/DALCC)
+ Chunxiao Li, Xuejing Kang, Zhifeng Zhang, Anlong Ming*, SWBNet: A Stable White Balance Network for sRGB images, AAAI 2023, 人工智能领域顶会. [[pdf]](https://github.com/ChunxiaoLe/SWBNet/blob/master/paper/9786.ChunxiaoLi.pdf) [[code]](https://github.com/ChunxiaoLe/SWBNet)
+ Chunxiao Li, Xuejing Kang, Anlong Ming*, WBFlow: Few-shot White Balance for sRGB Images via Reversible Neural Flows，IJCAI 2023, 人工智能领域顶会.
+ Chenghao Dong, Xuejing Kang, Anlong Ming, ICDA: Illumination-Coupled Domain Adaptation Framework for Unsupervised Nighttime Semantic Segmentation,IJCAI 2023, 人工智能领域顶会.
+ 在投3篇

