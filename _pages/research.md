---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---
{% include base_path %}

<style>
.research-text p {
  text-align: justify;
  text-justify: inter-word;
}

.research-text p.image-center {
  text-align: center;
}

.research-text li {
  text-align: left;
}
</style>

<div class="research-text" markdown="1">

Vision
----

My Fusion Intelligence Laboratory aims to **use machine intelligence and multi-source information fusion to benefit humanity.**

The idea of **Fusion Intelligence** was first conceived during my time at Imperial College London and was formalised in 2024 when I established the Fusion Intelligence Laboratory. It describes my long-term research agenda: developing intelligent systems that can integrate complementary information from multiple sensors, modalities, and data sources to perceive, reason, and support decision-making more reliably in complex real-world environments. Rather than treating multimodal learning, image fusion, robotics, healthcare AI, and trustworthy AI as separate topics, my work connects them through a common goal: building AI systems that combine complementary sources of information to support human-centred perception, decision-making, and action.


Research areas
----
Under the vision of Fusion Intelligence, my research spans five closely connected directions:

- [Multimodal Learning and Image Fusion](#multimodal-learning-and-image-fusion)  
- [Robotics and Embodied Intelligence](#robotics-and-embodied-intelligence)  
- [Human-Centered Computer Vision](#human-centered-computer-vision)  
- [Trustworthy and Responsible AI](#trustworthy-and-responsible-ai)  
- [AI for Healthcare](#ai-for-healthcare)  

[**Multimodal learning and image fusion**](#multimodal-learning-and-image-fusion) provide the methodological foundation for integrating complementary visual and sensory information. [**Robotics and embodied intelligence**](#robotics-and-embodied-intelligence) develop research capacity for studying intelligent systems in physical environments. [**Human-centered computer vision**](#human-centered-computer-vision) focuses on understanding and assisting people in real-world scenarios. [**Trustworthy and responsible AI**](#trustworthy-and-responsible-ai) focuses on robustness, privacy protection, and socially responsible AI technologies. [**AI for healthcare**](#ai-for-healthcare) explores how multimodal learning and image analysis can support the analysis of medical images and biomedical multimodal data.

Research topics
----

<h2 id="multimodal-learning-and-image-fusion">1. Multimodal Learning and Image Fusion</h2>

<div style="display: flex; justify-content: center; align-items: center;">
  <img src="/images/research/vif.png" alt="First Image" style="height: 300px; width: auto; margin-right: 20px;">
  <img src="/images/research/mef.png" alt="Second Image" style="height: 300px; width: auto;">
</div>

**Multimodal learning and image fusion** form the methodological foundation of my research on **Fusion Intelligence**. This direction focuses on developing algorithms that can integrate complementary information from multiple sensors, modalities, or data sources, such as visible images, infrared images, depth, event data, LiDAR, and medical imaging data. My work has covered both **low-level image fusion**, including visible-infrared, multi-focus, and multi-exposure image fusion, and **high-level multimodal understanding**, including RGB-T tracking, segmentation-oriented fusion, and multimodal medical image analysis.

Beyond developing individual algorithms, I have also contributed to the community through surveys, benchmarks, comparative studies, open resources, and books, including the published book [*Image Fusion*](https://link.springer.com/book/10.1007/978-981-15-4867-3) and the open-source book project [*Intelligence of Fusion*](https://xingchenzhang.github.io/imagefusionbook/). These efforts aim to organise and communicate the foundations, progress, and future directions of multimodal information fusion. Together, they provide the core perception and representation-learning capabilities that support my broader research in [embodied intelligence](#robotics-and-embodied-intelligence), [trustworthy AI](#trustworthy-and-responsible-ai), and [healthcare applications](#ai-for-healthcare).

Related publications:  
1. **X. Zhang**, Y. Demiris. Visible and Infrared Image Fusion using Deep Learning, IEEE Transactions on Pattern Analysis and Machine Intelligence, vol. 45, no. 8, pp. 10535-10554, 2023. (**ESI Highly Cited Paper, ESI hot paper)**  
2. **X. Zhang**. Deep Learning-based Multi-focus Image Fusion: A Survey and A Comparative Study, IEEE Transactions on Pattern Analysis and Machine Intelligence, vol. 44, No. 9, pp. 4819 – 4838, 2022. [[Link]](https://github.com/xingchenzhang/MFIFB) (**ESI Highly Cited Paper**)  
3. **X. Zhang**. Benchmarking and Comparing Multi-exposure Image Fusion Algorithms. Information Fusion, vol. 74, pp. 111-131, 2021. (The first multi-exposure image fusion benchmark) [[Benchmark link]](https://github.com/xingchenzhang/MEFB)  
4. **X. Zhang**, P. Ye, H. Leung, K. Gong, G. Xiao. Object Fusion Tracking Based on Visible and Infrared Images: A Comprehensive Review. Information Fusion, vol. 63, pp. 166-187, 2020. 
4. **X. Zhang**, P. Ye, G. Xiao. VIFB: A Visible and Infrared Image Fusion Benchmark, In the Proceedings of IEEE/CVF Conference on Computer Vision Workshops, 2020. (The first image fusion benchmark, which has been utilized by researchers from more than 10 countries.) [[Benchmark link]](https://github.com/xingchenzhang/VIFB)  
5. **X. Zhang**, P. Ye, S. Peng, J. Liu, G. Xiao. DSiamMFT: An RGB-T fusion tracking method via
dynamic Siamese networks using multi-layer feature fusion. Signal Processing: Image
Communication, vol. 84, 2020.  
6. **X. Zhang**, P. Ye, D. Qiao, J. Zhao, S. Peng, G. Xiao. Object Fusion Tracking Based on Visible and
Infrared Images Using Fully Convolutional Siamese Networks. In Proceedings of the 22nd
International Conference on Information Fusion, 2019.  
7. **X. Zhang**. "Multi-focus image fusion: A benchmark." arXiv preprint arXiv:2005.01116 (2020). (The first multi-focus image fusion benchmark in the community)  
8. Z. Zhao, A. Howes, **X. Zhang**\*. MultiTaskVIF: Segmentation-oriented visible and infrared image fusion via multi-task learning. IEEE Transactions on Image Processing. [[Link]](https://arxiv.org/pdf/2505.06665)  
10. Z. Zhao, **X. Zhang**\*. SSVIF: Self-Supervised Segmentation-Oriented Visible and Infrared Image Fusion. IEEE Transactions on Image Processing. [[Link]](https://arxiv.org/abs/2509.22450) 
11. Q. Li, Z. Zhao, **X. Zhang**\*. Brain tumor segmentation using multimodal MRI. DIFA 2025 Workshop, BMVC2025.  
1. G. Xiao, D.P. Bavirisetti , G. Liu , **X. Zhang**, [Image Fusion](https://link.springer.com/book/10.1007/978-981-15-4867-3), Springer Nature Singapore and Shanghai Jiao Tong University Press, 2020. This book has won the **National Science and Technology Academic Publications Fund of China** (2019).   
2. **X. Zhang**. Intelligence of Fusion: Deep Learning-based Image Fusion (written in Chinese). 2025. This book is available [here](https://xingchenzhang.github.io/imagefusionbook/). 

\* Corresponding authors



<h2 id="robotics-and-embodied-intelligence">2. Robotics and Embodied Intelligence</h2>

My lab has received funding and support from the Royal Society, NVIDIA Academic Grant, the European Commission, and UKRI AIRR to develop research capacity in robotics and embodied intelligence.

We are building a robotics research platform with mobile robots, different sensors, and NVIDIA Jetson edge-computing devices.

<p class="image-center"> 
  <img width="700" src="/images/research/FIL-robot.jpg" />
</p>


<h2 id="human-centered-computer-vision">3. Human-Centered Computer Vision</h2>
Human-centered computer vision focuses on developing AI systems that can understand, predict, and assist human behaviour in real-world environments. My research in this area has mainly explored pedestrian perception, including pedestrian trajectory prediction, crossing intention prediction, and pedestrian tracking. These studies aim to improve the ability of intelligent systems to understand people’s movements, intentions, and interactions with the surrounding environment, contributing to my broader goal of developing AI technologies that can assist humans and support safer, more intelligent real-world systems.

<h3>(1) Pedestrian Trajectory Prediction</h3>
<p class="image-center"> 
  <img width="500" src="/images/research/Demo Social TAG.gif" />
</p>

<h3>(2) Pedestrian Crossing Intention Prediction</h3>
<p class="image-center"> 
  <img width="700" src="/images/research/crossingpose.png" />
</p>

<h3>(3) Pedestrian Tracking</h3>
<p class="image-center"> 
  <img width="700" src="/images/research/Pedestrian-tracking.gif" />
</p>

<!-- <p align="center"> 
  <img width="500" src="/images/research/MOT17-03-SelectMOT.gif" />
</p> -->

Related publications:    

1. **X. Zhang***, P. Angeloudis, Y. Demiris. ST CrossingPose: A Spatial-Temporal Graph Convolutional Network for Skeleton-based Pedestrian Crossing Intention Prediction, IEEE Transactions on Intelligent Transportation Systems, vol. 23, no. 11, pp. 20773-20782, 2022.  
2. **X. Zhang***, P. Angeloudis, Y. Demiris. Dual-branch Spatio-Temporal Graph Neural Networks for Pedestrian Trajectory Prediction, Pattern Recognition, vol. 142, 2023.  
3. **X. Zhang**\*, Y. Demiris. Self-Supervised RGB-T Tracking with Cross-Input Consistency. arXiv preprint arXiv:2301.11274 (2023).   
4. J. Liu, P. Ye. **X. Zhang***, G. Xiao. Real-time long-term tracking with reliability assessment and
object recovery. IET Image Processing, vol. 15, no. 4, pp. 918-935, 2021.  
5. J. Liu, G. Xiao, **X. Zhang***, P. Ye, X. Xiong, S. Peng. Anti-occlusion object tracking based on
correlation filter. Signal, Image and Video Processing, vol. 14, no. 4, pp. 753-761, 2020.  
6. J. Zhao, G. Xiao\*, **X. Zhang***, D. P. Bavirisetti. An improved long-term correlation tracking method with occlusion handling. Chinese Optics Letters, vol. 17, no. 3, pp. 031001-1: 031001-6, 2019.  

<h2 id="trustworthy-and-responsible-ai">4. Trustworthy and Responsible AI</h2>
Trustworthy and responsible AI focuses on developing AI technologies that are reliable, robust, privacy-preserving, and socially responsible. My current work in this area includes privacy protection in visual data, with a particular focus on reducing the risk of exposing identifiable personal information while preserving the utility of images and videos for computer vision tasks.

<h3>Pedestrian Privacy Protection</h3>  

Many videos are captured to train AI models. We aim to protect pedestrian privacy in videos captured by cameras mounted on robots and vehicles while maintaining the utility of the anonymized videos. More details on our pedestrian privacy protection project can be found [here](https://xingchenzhang.github.io/research/privacy/). 

<!-- <img align="center" width="600" src="/images/word cloud.png" />  -->

<!-- 
<p align="center"> 
  <img width="600" src="/images/research/3PFS.png" />
</p>
-->

<div style="display: flex; justify-content: center; align-items: center;">
  <img src="/images/research/3PFS.png" alt="First Image" style="height: 300px; width: auto; margin-right: 20px;">
  <img src="/images/research/3PFS.gif" alt="Second Image" style="height: 300px; width: auto;">
</div>

Related publications:  
1. Z. Zhao, **X. Zhang***, Y. Demiris. 3PFS: Protecting pedestrian privacy through face swapping, IEEE Transactions on Intelligent Transportation Systems, vol. 25, no. 11, pp. 16845-16854, 2024.  
2. **X. Zhang***, Z. Zhao. More effort is needed to protect pedestrian privacy in the era of AI. NeurIPS Position Paper Track, 2025. **Oral paper**.


<h2 id="ai-for-healthcare">5. AI for Healthcare</h2>
AI for healthcare focuses on developing machine learning and computer vision methods for the analysis of medical images and biomedical multimodal data. My research in this area explores how AI can extract useful information from complex image-based and multimodal healthcare-related data. This direction builds on my broader interests in multimodal learning and image analysis.

Related publications:  
1. Q. Li, Z. Zhao, **X. Zhang**\*. Brain tumor segmentation using multimodal MRI. BMVC Workshop 2025. 

</div>
