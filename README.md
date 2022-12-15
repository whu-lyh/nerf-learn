# Nerf(神经辐射场)学习笔记
>本人的科研方向是三维重建与对抗生成，Nerf让人惊叹

>争取搞清楚每一个数学公式和每一行代码

### 一. 基本原理
01. [颠覆传统三维重建方法之nerf(一)---概述](01.颠覆传统三维重建方法之nerf(一)---概述.md)
02. [颠覆传统三维重建方法之nerf(二)---工作流程与基本原理](02.颠覆传统三维重建方法之nerf(二)---工作流程与基本原理.md)
03. [颠覆传统三维重建方法之nerf(三)---光线的数学表示与采样点](03.颠覆传统三维重建方法之nerf(三)---光线的数学表示与采样点.md)
04. [颠覆传统三维重建方法之nerf(四)---NeRF最核心公式推导-光线成像模型](04.颠覆传统三维重建方法之nerf(四)---公式推导-光线成像模型.md)
05. [颠覆传统三维重建方法之nerf(五)---相机小孔成像模型的逆变换](05.颠覆传统三维重建方法之nerf(五)---相机小孔成像模型的逆变换.md)

### 二. 读pytorch-nerf项目
06. [颠覆传统三维重建方法之nerf(六)---pytorch-nerf项目介绍](06.颠覆传统三维重建方法之nerf(六)---pytorch-nerf项目介绍.md)
07. [颠覆传统三维重建方法之nerf(七)---pytorch-nerf数据格式与数据加载](07.颠覆传统三维重建方法之nerf(七)---pytorch-nerf数据格式与数据加载.md)
08. [颠覆传统三维重建方法之nerf(八)---pytorch-nerf模型创建1之概述](08.颠覆传统三维重建方法之nerf(八)---pytorch-nerf模型创建1之概述.md)
09. [颠覆传统三维重建方法之nerf(九)---pytorch-nerf模型创建2之位置编码](09.颠覆传统三维重建方法之nerf(九)---pytorch-nerf模型创建2之位置编码.md)
10. [颠覆传统三维重建方法之nerf(十)---pytorch-nerf模型创建3之创建NeRF](10.颠覆传统三维重建方法之nerf(十)---pytorch-nerf模型创建3之创建NeRF.md)
11. [颠覆传统三维重建方法之nerf(十一)---pytorch-nerf模型训练1之概述](11.颠覆传统三维重建方法之nerf(十一)---pytorch-nerf模型训练1之概述.md)
12. [颠覆传统三维重建方法之nerf(十二)---pytorch-nerf模型训练2之计算光线](12.颠覆传统三维重建方法之nerf(十二)---pytorch-nerf模型训练2之计算光线.md)
13. [颠覆传统三维重建方法之nerf(十三)---pytorch-nerf模型训练3之渲染(光线成像)](13.颠覆传统三维重建方法之nerf(十三)---pytorch-nerf模型训练3之渲染(光线成像).md)
14. [颠覆传统三维重建方法之nerf(十四)---pytorch-nerf模型训练4之损失函数](14.颠覆传统三维重建方法之nerf(十四)---pytorch-nerf模型训练4之损失函数.md)
15. [颠覆传统三维重建方法之nerf(十五)---pytorch-nerf模型测试与推理](15.颠覆传统三维重建方法之nerf(十五)---pytorch-nerf模型测试与推理.md)
16. [颠覆传统三维重建方法之nerf(十六)---pytorch-nerf总结](16.颠覆传统三维重建方法之nerf(十六)---pytorch-nerf总结.md)

### 三. 读[instant-ngp](https://github.com/NVlabs/instant-ngp) 源码系列
1. [下载编译运行ngp](instant-ngp/1.下载编译运行ngp.md)

### 四. nerf模型提升的变种
1. mip-NeRF
2. **instant-ngp**
3. Block-NeRF
4. Plenoctree
5. Plenoxels
6. **Neus**
7. KeypointNeRF：基于图像的体积化身的泛化
8. point-NeRF：训练更快
2. 压缩模型：https://mp.weixin.qq.com/s/hltAHEEVd4_ZTeLXxF1-ow

### 五. 各种应用场景及其模型
1. NeuMan
    - [NeuMan](NeuMan/NeuMan.md)：基于Nerf的从单个视频实现人体三维重建。
    - [NeuMan-预处理](NeuMan/NeuMan-预处理.md)
2. AD-NeRF 
    - 由音频和人脸图像合成人脸视频并表现出自然的说话风格
    - https://yudongguo.github.io/ADNeRF/
    - https://github.com/YudongGuo/AD-NeRF
3. 4D-Facial-Avatars：
    - https://github.com/gafniguy/4D-Facial-Avatars
4. NeRFFaceEditing：
    - http://geometrylearning.com/NeRFFaceEditing/
    - https://mp.weixin.qq.com/s/cv6g-5i9C5ej2CQtI0tEGw
5. FENeRF
    - 使用 NeRF 进行人脸编辑
    - https://mrtornado24.github.io/FENeRF/
    - https://mp.weixin.qq.com/s/G6b9M3PrMjhwRWLJw6GmpQ
6. SMPL-CLIP-NeRF
    - 单张图片生成数字人
    - https://mp.weixin.qq.com/s/76-klqy_kiExjAyh2CVQvA
7. CLIP-NeRF 
    - 文字-图像驱动的 NeRF 操作
    - https://mp.weixin.qq.com/s/DDt6rVGk4inBFkDnlgBpQA
8. AdaNeRF
    - 自适应采样用于神经辐射场实时渲染
    - https://mp.weixin.qq.com/s/XJTrg-iAOC8PQLjsnmL1oQ
9. MoFaNeRF
    - 可变形面部神经辐射场
    - https://mp.weixin.qq.com/s/Wmx6l3IDOBV8PH1taka71w
10. NeRF-GAN
    - 在StyleGAN中注入可控三维感知，NeRF-GAN用于可编辑人像合成
    - https://mp.weixin.qq.com/s/QcLsHTKEEgB53Z0oi7kaPA
11. ENeRF：首次实现任意动态场景的实时照片级渲染
    - https://mp.weixin.qq.com/s/xuZ6x-ff4WHmGc-vW5j6dw
12. MoFaNeRF: 可变形面部神经辐射场
    - https://mp.weixin.qq.com/s/Wmx6l3IDOBV8PH1taka71w
13. NeRF-SLAM: 具有神经辐射场的实时密集单目SLAM
    - https://mp.weixin.qq.com/s/7ez-Jh9BQMQFtxd6x5OP4Q
14. DiffRF: 
    - Rendering-guided 3D Radiance Field Diffusion
    - https://sirwyver.github.io/DiffRF/
12. StyleNeRF
13. PixelNeRF
14. IBRNet
15. [查看更多1](https://github.com/yenchenlin/awesome-NeRF)
16. [查看更多2](https://www.bilibili.com/video/BV1GM41167Vo)
17. [查看更多3](https://www.bilibili.com/video/BV1fL4y1T7Ag)
### 六. 各种参考资料/课程/视频


