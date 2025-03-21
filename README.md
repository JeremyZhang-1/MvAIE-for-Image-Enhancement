# MvAIE-for-Image-Enhancement
# Multi-view Adaptive Image Enhancement with Hierarchical Attention for Complex Underground Mining Scenes
#  Introduction
The Multi-view Adaptive Image Enhancement with Hierarchical Attention Network (MvAIE) is designed to enhance images in underground mines, specifically tackling challenges posed by darkness, fog, and glare. 

This code was collaboratively developed by Wuhan University of Technology and The Hong Kong Polytechnic University to enhance perception capabilities for autonomous driving in underground mines, facilitating the practical implementation of autonomous driving technology in such environments.

# Abstract
The harsh environmental conditions in underground mines, including low illumination, haze, and dust, pose significant challenges to the visual perception systems of autonomous mining vehicles. To address these challenges, this paper proposes a novel multi-view adaptive image enhancement with Hierarchical Attention (MvAIE) that combines adaptive enhancement with multi-view feature fusion strategies to achieve efficient and precise image restoration. Specifically, the proposed adaptive enhancement module dynamically adjusts gamma correction and HSV color space parameters in response to varying lighting and color conditions. Furthermore, the multi-branch feature fusion module leverages dilated convolutions and a hierarchical encoder-decoder structure to extract features across multiple scales, capturing both global context and fine details. It is particularly effective for recovering essential features such as object edges and textures in degraded images, directly benefiting task-specific performance. To further enhance task relevance, the framework incorporates a multi-receptive global-local attention mechanism that prioritizes critical image regions, improving the network’s focus on areas important for accurate object detection and localization. By aligning the enhancement process with the requirements of downstream tasks, MvAIE ensures that restored images not only achieve superior visual quality but also provide robust support for autonomous mining applications. Experimental results demonstrate that MvAIE outperforms existing methods in enhancing image quality, providing robust support for autonomous driving in intelligent mining applications.


![Figure_2](https://github.com/user-attachments/assets/f4df3958-ef1b-4a89-99bb-c0bbda40cee6)

# Prerequisites
```
conda create -n dehaze python=3.7
conda activate dehaze
conda install pytorch=1.10.2 torchvision torchaudio cudatoolkit=11.3 -c pytorch
python3 -m pip install scipy==1.7.3
python3 -m pip install opencv-python==4.4.0.46
```

# Result

The visual comparison result on (a) synthesized degraded CDD-11 images with (b) 4kdehaze , (c) APSF , (d) C2PNet, (e) DHFormer, (f) GMLC, (g) IENHC, (h) MRP, (i) OSFD, (j) Our method, and (k) Gronud Truth, respectively.
![Figure15](https://github.com/user-attachments/assets/4bb2c1cf-9e06-404e-a000-ed0368e1cb2c)

The visual comparison result on (a) synthesized degraded mining images with (b) 4kdehaze , (c) APSF , (d) C2PNet, (e) DHFormer, (f) GMLC, (g) IENHC, (h) MRP, (i) OSFD, (j) Our method, and (k) Gronud Truth, respectively.
![Figure16](https://github.com/user-attachments/assets/5170c1c4-fd96-468b-9fe9-d57f2f92c7cf)

# License
The code and models in this repository are licensed under the WHUT License for academic and other non-commercial uses.
For commercial use of the code and models, separate commercial licensing is available. Please contact:
- Jingming Zhang (jeremy.zhang@whut.edu.cn)
- Yuxu LU (yuxulouis.lu@connect.polyu.hk)

