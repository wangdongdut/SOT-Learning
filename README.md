# SOT-Learning

## 内容

## 资源

* **代码框架**
     | **框架**              | **链接**    | **简介**    |
     |:-----------           |:----------------|:----------------|
     | **pysot**             | https://github.com/STVIR/pysot             | STVIR组提供的跟踪框架，主要包括SiamFC，SiamRPN，DaSiamRPN，SiamRPN++，SiamMask等算法。|     
     | **pytracking**        | https://github.com/visionml/pytracking     | visionml组提供的跟踪框架，主要包括pyECO, ATOM, Dimp, PrDimp, KeepTrack等算法。|     
     | **TracKit**           | https://github.com/researchmm/TracKit      | MSRA-MM组提供的跟踪框架，主要包括SiamDW，Ocean跟踪算法。|
     | **mmtracking**        | https://github.com/open-mmlab/mmtracking   | Open-mmlab Tracking相关库，包括视频目标检测，单目标跟踪，多目标跟踪，视频实例分割。其中单目标跟踪算法支持SiameseRPN++(CVPR2019)，STARK(ICCV2021)，PrDiMP(CVPR2020)等算法。和Open-mmlab一脉相承，未来有很大潜力。 |
     | **got-10k-toolkit**   | https://github.com/got-10k/toolkit   | Got-10k数据集网站提供的评估工具，方便大量跟踪数据库上的实验测评，如OTB(2013/2015), VOT(2013~2018), DTB70, TColor128, NfS(30/240 fps), UAV(123/20L), LaSOT, TrackingNet等。 |

* **综述文章**

     | **论文**              | **链接**    | **内容摘要**    |
     |:-----------           |:----------------:|:----------------|
     | ***Visual Object Tracking with Discriminative Filters and Siamese Networks: A Survey and Outlook.*** <br /> **Arxiv, 2021.** Sajid Javed, Martin Danelljan, Fahad Shahbaz Khan, et al. | [[Paper](https://arxiv.org/abs/2112.02838)]   |  **:star2:非常详尽的判决性滤波和深度孪生网络方面的综述**，大量的实验评估。SiamR-CNN基本上算是深度孪生卷积网络类跟踪算法的精度巅峰，但于2021年被简单的Transformer跟踪算法超越。*2021年开始，SOT全面进入Transformer时代。* | 
     | ***Deep Learning for Visual Tracking: A Comprehensive Survey.*** <br /> **IEEE TITS, 2022.** Seyed Mojtaba Marvasti-Zadeh, Li Cheng, Hossein Ghanei-Yakhdan, Shohreh Kasae.     |  [[Paper](https://ieeexplore.ieee.org/document/9339950)]   |  **:star2:非常详尽的深度学习类跟踪算法综述**， 从网络结构，网络利用，网络训练，网络目标，网络输出，深度学习与相关滤波，长时跟踪，在线更新跟踪等多个维度详尽地综述了2013-2020年的深度学习类跟踪算法。<br /> *2019-2020时的深度学习类跟踪相关已显著超越相关滤波结合深度特征类算法，SOT已彻底全面步入深度学习时代。* |   
     | ***Handcrafted and Deep Trackers: Recent Visual Object Tracking Approaches and Trends.*** <br />  **ACM CS, 2019.** Mustansar Fiaz, Arif Mahmood, Sajid Javed, Soon Ki Jung.     |  [[Paper](https://dl.acm.org/doi/abs/10.1145/3309665)]   |  主要综述了2018年之前的相关滤波类算法和非相关滤波类算法，对2015-2018年提出的相关滤波类算法综述较为详尽。<br />  *深度学习类跟踪算法更推荐看《Deep Learning for Visual Tracking: A Comprehensive Survey》*  |  
     | ***Deep Visual Tracking: Review and Experimental Comparison.*** <br />  **PR, 2018.** Peixia Li, Dong Wang, Lijun Wang, Huchuan Lu.    |  [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0031320317304612)]   |   主要综述了早期深度学习跟踪算法，从网络结构，网络形式，网络训练三个角度进行了细致的分析。当时，在端到端深度跟踪算法和传统跟踪算法结合深度特征还平分秋色；2019年后，端到端深度跟踪算法占据绝对统治地位。<br /> *深度学习类跟踪算法更推荐看《Deep Learning for Visual Tracking: A Comprehensive Survey》*  |  
     | ***Object Tracking Benchmark.*** <br />  **IEEE TPAMI, 2015.** Yi Wu, Jongwoo Lim, Ming-Hsuan Yang. |  [[Paper](https://ieeexplore.ieee.org/document/7001050)] <br /> [[Website](http://cvlab.hanyang.ac.kr/tracker_benchmark/)]   | **跟踪领域最经典Benchmark：OTB-100**，同样也是2013年及之前跟踪算法很好的总结，推动了跟踪算法评测的标准化，提出的**Precision和Success**指标现在仍是主流评测指标。评测了29个代表性的Trackers，但排名未进前5的CSK算法在结合了HOG特征之后，成为了2015-2019年最主要的主流算法，即相关滤波算法。| 
     | ***Understanding and Diagnosing Visual Tracking Systems.*** <br /> **ICCV, 2015.**  Naiyan Wang, Jianping Shi, Dit-Yan Yeung, Jiaya Jia.   | [[Paper](https://ieeexplore.ieee.org/document/7410712)] <br />  [[Website](http://www.winsty.net/tracker_diagnose.html)]  | 一份非常值得读的早期跟踪系统解析报告，重要结论：跟踪器性能**特征为王**，运动模型不那么重要（这个其实有数据集偏见在里面）。对现在SOT等相关领域研究也有启发意义。如果发现**所选用的特征**落后时代了，那么把外观模型（公式或结构）搞的再花哨也是意义不大的。|  
     | ***Visual Tracking: An Experimental Survey.*** <br /> **IEEE TPAMI, 2014.**  Arnold W. M. Smeulders, Dung Manh Chu, Rita Cucchiara, et al.   | [[Paper](https://ieeexplore.ieee.org/document/6671560)]    | 早期的跟踪评估综述，主要总结和评估了2012年前的知名算法。提出了有315个视频的评测数据集ALOV++，但由于在CVPR2013和TPAMI2015上发表和扩充的OTB数据库和评测标准更受研究者欢迎，ALOV++现在鲜有人用，而OTB已成为业内标准之一。   |   
     | ***Sparse Coding Based Visual Tracking: Review and Experimental Comparison.*** <br /> **PR, 2013**.  Shengping Zhang, Hongxun Yao, Xin Sun, Xiusheng Lu.   | [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0031320312004396)]    |  稀疏表示跟踪算法的综述，稀疏表示类跟踪算法大约集中在2009-2013年，当时稀疏表示的冗余字典表示，遮挡建模，多任务建模，稀疏编码特征具有一定的优势。*但后来精度和速度均完败于**KCF**，被历史淘汰。*  |   
     | ***A Survey of Appearance Models in Visual Object Tracking.*** <br /> **ACM TIST, 2013.** Xi Li, Weiming Hu, Chunhua Shen, Zhongfei Zhang, et al.   | [[Paper](https://dl.acm.org/doi/10.1145/2508037.2508039)]   |  早期跟踪算法的综述，主要总结了2012年及之前的跟踪算法。 **当时跟踪算法主要分为：生成模型和判决模型两大流派。** **生成模型**流派主要以混合高斯，核密度估计，子空间学习，稀疏表示等为主，特点是建模目标本身，不关心背景信息；**判决模型**流派主要以各种在线分类器，判决性子空间和字典学习等为主，特点是同时建模目标和背景，强调目标和背景的区分。*后来判决模型占据主流，甚至一统SOT江湖。*  |  
     | ***Object Tracking: A Survey.*** <br /> **ACM CS, 2006.**  lper Yilmaz, Omar Javed, Mubarak Shah.   |  [[Paper](https://dl.acm.org/doi/10.1145/1177352.1177355)]   |远古时期跟踪的综述。(1) 从目标表示角度分类：中心点，多关键点，矩形框，椭圆框，多块结构，骨架，边界控制点，边界轮廓，剪影（和Mask类似）； **后来矩形框和分割Mask成为目标表示的主流** (2) 从跟踪算法的角度分类：点跟踪，核跟踪（代表性算法Meanshift, KLT, Eigentracking, SCM），剪影跟踪; **后来点跟踪更多发展为特征点跟踪，应用于SLAM等领域；核跟踪成为SOT的主流（虽然叫法不同）；剪影跟踪发展成为了基于分割的跟踪或视频分割任务。**    |

* **历年[VOT](https://www.votchallenge.net/)冠军算法**

     | **年份**              | **赛道**    | **冠军简介**    |
     |:-----------           |:----------------|:----------------|    
     | [**VOT2021**](https://www.votchallenge.net/vot2021/)  | | |     
     | [**VOT2020**](https://www.votchallenge.net/vot2020/)  | | |
     | [**VOT2019**](https://www.votchallenge.net/vot2019/)  | | |
     | [**VOT2018**](https://www.votchallenge.net/vot2018/)  | | |
     | [**VOT2017**](https://www.votchallenge.net/vot2017/)  | | |   
     | [**VOT2016**](https://www.votchallenge.net/vot2016/)  | TIR | |  
     | [**VOT2016**](https://www.votchallenge.net/vot2016/)  | ST | | 
     | [**VOT2015**](https://www.votchallenge.net/vot2015/)  | TIR | |
     | [**VOT2015**](https://www.votchallenge.net/vot2015/)  | ST | |
     | [**VOT2014**](https://www.votchallenge.net/vot2014/)  | ST | |
     | [**VOT2013**](https://www.votchallenge.net/vot2013/)  | ST | **PLT**(Single scale pixel based LUT tracker)：PLT runs a classifier at a fixed single scale for each test image, to determine the top scoring bounding box which is then the result of object detection. The classifier uses a binary feature vector constructed from color, grayscale and gradient information. To select a small set of discriminative features, an online sparse [structural SVM](https://ieeexplore.ieee.org/document/6126251) is used. Since the object can be non-rigid and the bounding box may be noisy, not all pixels in the bounding box belong to the object. Hence, a probabilistic object-background segmentation mask from color histograms is created and used to weight the features during SVM training. The resulting weighted and convex problem can be solved in three steps: (i) compute the probability that a pixel belongs to the objectby using its color. (ii) solve the original non-sparse structural SVM and (iii) [shrink the solution](https://ieeexplore.ieee.org/document/6248061), i.e. features with smallest values are discarded. Since the feature vector is binary, the linear classifier can be implemented as a lookup table for fast speed.  --From [《VOT2013 Report》](https://www.votchallenge.net/vot2013/Download/vot_2013_paper.pdf)|


* **在线学习/报告资源**

     | **视频/博客**              | 内容摘要    |
     |:-----------               |:----------------:|
     |**[叫我林林就行](https://space.bilibili.com/209664735/)：[Github](https://github.com/HonglinChu), [B站视频](https://space.bilibili.com/209664735/)** |CF和Siamese系列工作介绍复现；轻量级跟踪器NanoTrack|
     |**[东大阿德](https://space.bilibili.com/6794832/)：[单目标跟踪零基础代码入门-B站视频](https://space.bilibili.com/6794832/channel/collectiondetail?sid=400776)** |SiamFC, SiamRPN, pytracking系列代码讲解；RGBT跟踪介绍|
     |**[深度大脑](https://space.bilibili.com/9456738)：[从零开始的单目标跟踪算法世界-B站视频](https://www.bilibili.com/video/BV1WK4y1C7JG)** |pytracking系列代码讲解|
     |**[VALSE_Webinar](https://space.bilibili.com/562085182/)(跟踪问题)：[B站视频](https://space.bilibili.com/562085182/search/video?keyword=%E8%B7%9F%E8%B8%AA)** |基础知识，前沿报告，论文速览；公众号：VALSE |
     |**[极市平台](https://space.bilibili.com/85300886/)(跟踪问题)：[B站视频](https://space.bilibili.com/85300886/search/video?keyword=%E8%B7%9F%E8%B8%AA)** |部分原作者论文报告；公众号：极市平台|
     |**[AITracker](https://space.bilibili.com/8948069)：[B站视频](https://space.bilibili.com/8948069)** |系列讲座，经验分享；公众号：目标跟踪与检测基础前沿|
     |**[人工智能前沿讲习](https://bbs.sffai.com/)(跟踪问题)：[B站视频](https://space.bilibili.com/388690539/search/video?keyword=%E8%B7%9F%E8%B8%AA)** |系列讲座，经验分享；公众号：人工智能前沿讲习|
     |**[YaqiLYU(知乎)](https://www.zhihu.com/people/YaqiLYU)：[深度学习和目标跟踪(知乎专栏)](https://www.zhihu.com/column/DCF-tracking)** |算法总结感悟，移动端跟踪|
     |**[NTRのSAO年(B站)](https://space.bilibili.com/5567932)：[B站专栏](https://space.bilibili.com/5567932/article)** |部分论文速览|
