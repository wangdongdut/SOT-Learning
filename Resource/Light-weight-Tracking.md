# Light-weight Tracking

* **SiamFC:** Luca Bertinetto, Jack Valmadre, João F. Henriques, Andrea Vedaldi, Philip H. S. Torr. Fully-Convolutional Siamese Networks for Object Tracking. ECCVW, 2016. [[Paper](https://arxiv.org/pdf/1606.09549.pdf)][[Project](https://www.robots.ox.ac.uk/~luca/siamese-fc.html)][[PySOTCode](https://github.com/STVIR/pysot)] 
* **ECO-HC:** Martin Danelljan, Goutam Bhat, Fahad Shahbaz Khan, Michael Felsberg. ECO: Efficient Convolution Operators for Tracking. CVPR, 2017. [[Paper](https://arxiv.org/pdf/2103.17154.pdf)][[Code](https://github.com/visionml/pytracking)]
* **LightTrack:** Bin Yan, Houwen Peng, Kan Wu, Dong Wang, Jianlong Fu, Huchuan Lu. LightTrack: Finding Lightweight Neural Networks for Object Tracking via One-Shot Architecture Search. CVPR, 2021. [[Paper](https://arxiv.org/pdf/2104.14545.pdf)][[Code](https://github.com/researchmm/LightTrack)] 
* **STARK-Lightning:** Bin Yan, Houwen Peng, Jianlong Fu, Dong Wang, Huchuan Lu. Learning Spatio-Temporal Transformer for Visual Tracking. ICCV, 2021. [[Paper](https://arxiv.org/pdf/2103.17154.pdf)][[Code](https://github.com/researchmm/Stark)]
* **FEAR:** Vasyl Borsuk, Roman Vei, Orest Kupyn, Tetiana Martyniuk, Igor Krashenyi, Jiři Matas. FEAR: Fast, Efficient, Accurate and Robust Visual Tracker. ECCV, 2022. [[Paper](https://arxiv.org/pdf/2112.07957.pdf)][[Code](https://github.com/PinataFarms/FEARTracker)] 
* **HCAT:** Xin Chen, Dong Wang, Dongdong Li, Huchuan Lu. Efficient Visual Tracking via Hierarchical Cross-Attention Transformer. ECCVW, 2022. [[Paper](https://arxiv.org/pdf/2203.13537.pdf)][[Code](https://github.com/chenxin-dlut/HCAT)] 
* **E.T.Track:** Philippe Blatter, Menelaos Kanakis, Martin Danelljan, Luc Van Gool. Efficient Visual Tracking with Exemplar Transformers. WACV, 2023. [[Paper](https://arxiv.org/pdf/2112.09686.pdf)][[Code](https://github.com/pblatter/ettrack)] 
* **HiT:** Ben Kang, Xin Chen, Dong Wang, Houwen Peng, Huchuan Lu. Exploring Lightweight Hierarchical Vision Transformers for Efficient Visual Tracking. ICCV, 2023. [[Paper](https://arxiv.org/abs/2308.06904)][[Code](https://github.com/kangben258/HiT)]
 
* **Others:** 
  * **NanoTrack:** https://github.com/HonglinChu/SiamTrackers/tree/master/NanoTrack
  * **让视觉目标跟踪在移动端起飞[YaqiLYU]：** [[一](https://zhuanlan.zhihu.com/p/416413600)], [[二](https://zhuanlan.zhihu.com/p/416754498)], [[三](https://zhuanlan.zhihu.com/p/419900331)]

* **Benchmark Results**

     | Tracker              | LaSOT (AUC)   | TrackingNet (AUC) | GOT-10K (AO)  |
     |:-----------          |:----------------:|:----------------:|:----------------:|
     | HCAT                 | 59.1  | 76.6 | 65.3 |        
     | E.T.Track            | 59.1  | 70.6 | - |      
     | FEAR                 | 57.9 | - | 64.5 |  
     | STARK-Lightning      | 58.6| - | - |  
     | LightTrack           | 53.8 | 72.5 | 61.1 |      
     | ECO-HC               | 32.4 | 55.4 | 31.6 |  
     | SiamFC               | - | - | - | 

<!-- 

# Light-weight Transformer Backbone

* **DeLighT:** Sachin Mehta, Marjan Ghazvininejad, Srinivasan Iyer, Luke Zettlemoyer, Hannaneh Hajishirzi. DeLighT: Deep and Light-weight Transformer. ICLR, 2021. 
 [[Paper](https://arxiv.org/pdf/2008.00623.pdf)][[Code](https://github.com/sacmehta/delight)]
* **LeViT:** Benjamin Graham, Alaaeldin El-Nouby, Hugo Touvron, Pierre Stock, Armand Joulin, Hervé Jégou, Matthijs Douze. LeViT: a Vision Transformer in ConvNet's Clothing for Faster Inference. ICCV, 2021. [[Paper](https://arxiv.org/pdf/2104.01136.pdf)][[Code](https://github.com/apple/ml-cvnets)]
*  **LVT:** Chenglin Yang, Yilin Wang, Jianming Zhang, He Zhang, Zijun Wei, Zhe Lin, Alan Yuille. Lite Vision Transformer with Enhanced Self-Attention. CVPR, 2022. [[Paper](https://arxiv.org/pdf/2112.10809.pdf)][[Code](https://github.com/Chenglin-Yang/LVT)] 
* **Mobile-Former:** Yinpeng Chen, Xiyang Dai, Dongdong Chen, Mengchen Liu, Xiaoyi Dong, Lu Yuan, Zicheng Liu. Mobile-Former: Bridging MobileNet and Transformer. CVPR, 2022. [[Paper](https://arxiv.org/pdf/2108.05895.pdf)][[Code](https://github.com/apple/ml-cvnets)] 
* **MobileViT:** 
  * **MobileViT:** Sachin Mehta, Mohammad Rastegari. MobileViT: Light-weight, General-purpose, and Mobile-friendly Vision Transformer. ICLR, 2022. [[Paper](https://arxiv.org/pdf/2110.02178v2.pdf)][[Code](https://github.com/apple/ml-cvnets)]
  * **MobileViTv2:** Sachin Mehta, Mohammad Rastegari. Separable Self-attention for Mobile Vision Transformers. Arxiv, 2022. [[Paper](https://arxiv.org/pdf/2206.02680.pdf)][[Code](https://github.com/apple/ml-cvnets)]
* **EdgeViT:** Junting Pan, Adrian Bulat, Fuwen Tan, Xiatian Zhu, Lukasz Dudziak, Hongsheng Li, Georgios Tzimiropoulos, Brais Martinez. EdgeViTs: Competing Light-weight CNNs on Mobile Devices with Vision Transformers. ECCV, 2022. [[Paper](https://arxiv.org/pdf/2205.03436.pdf)][[Code](https://github.com/saic-fi/edgevit)]
* **TinyViT:** Kan Wu, Jinnian Zhang, Houwen Peng, Mengchen Liu, Bin Xiao, Jianlong Fu, Lu Yuan. TinyViT: Fast Pretraining Distillation for Small Vision Transformers. ECCV, 2022. [[Paper](https://arxiv.org/pdf/2207.10666.pdf)][[Code](https://github.com/microsoft/Cream/tree/main/TinyViT)]
* **ParC-Net:** Haokui Zhang, Wenze Hu, Xiaoyu Wang. ParC-Net: Position Aware Circular Convolution with Merits from ConvNets and Transformer. ECCV, 2022. [[Paper](https://arxiv.org/pdf/2203.03952v5.pdf)][[Code](https://github.com/hkzhang91/ParC-Net)]
* **SReT:** Zhiqiang Shen, Zechun Liu, Eric Xing. Sliced Recursive Transformer. ECCV, 2022. [[Paper](https://arxiv.org/pdf/2111.05297.pdf)][[Code](https://github.com/szq0214/SReT)] 
* **LightViT:** Tao Huang, Lang Huang, Shan You, Fei Wang, Chen Qian, Chang Xu. LightViT: Towards Light-Weight Convolution-Free Vision Transformers. Arxiv, 2022. [[Paper](https://arxiv.org/pdf/2207.05557.pdf)][[Code](https://github.com/hunto/LightViT)] 
* **EdgeNeXt:**  Muhammad Maaz, Abdelrahman Shaker, Hisham Cholakkal, Salman Khan, Syed Waqas Zamir, Rao Muhammad Anwer, Fahad Shahbaz Khan. EdgeNeXt: Efficiently Amalgamated CNN-Transformer Architecture for Mobile Vision Applications. Arxiv, 2022. [[Paper](https://arxiv.org/pdf/2206.10589.pdf)][[Code](https://github.com/mmaaz60/EdgeNeXt)]
* **EfficientFormer:** Yanyu Li, Geng Yuan, Yang Wen, Eric Hu, Georgios Evangelidis, Sergey Tulyakov, Yanzhi Wang, Jian Ren. EfficientFormer: Vision Transformers at MobileNet Speed. Arxiv, 2022. [[Paper](https://arxiv.org/pdf/2206.01191.pdf)][[Code](https://github.com/snap-research/EfficientFormer)] 

# Light-weight CNN Backbone

* **MobileNet:**
  * **MobileNetV1:** Andrew G. Howard, Menglong Zhu, Bo Chen, Dmitry Kalenichenko, Weijun Wang, Tobias Weyand, Marco Andreetto, Hartwig Adam. MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications. Arxiv, 2017. [[Paper](https://arxiv.org/pdf/1704.04861.pdf)]
  * **MobileNetV2:** Mark Sandler, Andrew Howard, Menglong Zhu, Andrey Zhmoginov, Liang-Chieh Chen. MobileNetV2: Inverted Residuals and Linear Bottlenecks. CVPR, 2018. [[Paper](https://arxiv.org/pdf/1801.04381.pdf)]
  * **MobileNetV3:** Andrew Howard, Mark Sandler, Grace Chu, Liang-Chieh Chen, Bo Chen, Mingxing Tan, Weijun Wang, Yukun Zhu, Ruoming Pang, Vijay Vasudevan, Quoc V. Le, Hartwig Adam. Searching for MobileNetV3. ICCV, 2019. [[Paper](https://arxiv.org/pdf/1905.02244.pdf)]
* **ShuffleNet:**
  * Xiangyu Zhang, Xinyu Zhou, Mengxiao Lin, Jian Sun. ShuffleNet: An Extremely Efficient Convolutional Neural Network for Mobile Devices. CVPR, 2018. [[Paper](https://arxiv.org/pdf/1707.01083.pdf)] 
  * Ningning Ma, Xiangyu Zhang, Hai-Tao Zheng, Jian Sun. ShuffleNet V2: Practical Guidelines for Efficient CNN Architecture Design. ECCV, 2018. [[Paper](https://arxiv.org/pdf/1807.11164.pdf)] 

# Reference
* **Ultimate-Awesome-Transformer-Attention:** https://github.com/cmhungsteve/Awesome-Transformer-Attention
* **Efficient-AI-Backbones:** https://github.com/huawei-noah/Efficient-AI-Backbones
* **轻量级网络综述—主干网络篇:** https://mp.weixin.qq.com/s/-LAfyLA3U4C27thFlRgDhw
* **Efficient Transformers: A Survey** https://arxiv.org/abs/2009.06732

-->
