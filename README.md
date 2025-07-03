# MSCFF

Deep Learning Based Cloud Detection for Images of Different Sensors

<br>

This page has been rebuilt and redirected from [https://sendimage.whu.edu.cn/en/mscff](https://sendimage.whu.edu.cn/en/mscff)

<br>

**Introduction**

Cloud detection is an important preprocessing step for the precise application of optical satellite imagery. In this paper, we propose a deep learning based cloud detection method named multi-scale convolutional feature fusion (MSCFF) for remote sensing images of different sensors. In the network architecture of MSCFF, the symmetric encoder-decoder module, which provides both local and global context by densifying feature maps with trainable convolutional filter banks, is utilized to extract multi-scale and high-level spatial features. The feature maps of multiple scales are then up-sampled and concatenated, and a novel multi-scale feature fusion module is designed to fuse the features of different scales for the output. The two output feature maps of the network are cloud and cloud shadow maps, which are in turn fed to binary classifiers outside the model to obtain the final cloud and cloud shadow mask. The MSCFF method was validated on hundreds of globally distributed optical satellite images, with spatial resolutions ranging from 0.5 to 50 m, including Landsat-5/7/8, Gaofen-1/2/4, Sentinel-2, Ziyuan-3, CBERS-04, Huanjing-1, and collected high-resolution images exported from Google Earth. The experimental results show that MSCFF achieves a higher accuracy than the traditional rule-based cloud detection methods and the state-of-the-art deep learning models, especially in bright surface covered areas. The effectiveness of MSCFF means that it has great promise for the practical application of cloud detection for multiple types of medium and high-resolution remote sensing images. Our established global high-resolution cloud detection validation dataset has been made available online.

<br>

**Method**

**Li, Z., Shen, H., Cheng, Q., Liu, Y., You, S., & He, Z. (2019). [Deep learning based cloud detection for medium and high resolution remote sensing images of different sensors](https://zhiweili.net/assets/pdf/2019.4_ISPRS%20P&RS_Deep%20learning%20based%20cloud%20detection%20for%20medium%20and%20high%20resolution%20remote%20sensing%20images%20of%20different%20sensors.pdf). *ISPRS Journal of Photogrammetry and Remote Sensing*, 150, 197-212.**

![img](https://raw.githubusercontent.com/dr-lizhiwei/MSCFF/main/Flowchart.jpg)

Fig. 1. Flowchart of cloud and cloud shadow detection based on the multi-scale convolutional feature fusion method

<br>

**Experimental data and results**

![img](https://raw.githubusercontent.com/dr-lizhiwei/MSCFF/main/Datasets.jpg)

Fig. 2. Global distribution of the experimental data, including L7_Irish, L8_Biome, and GF1_WHU. The HRC_WHU data are not shown as they lack accurate geolocation information. The numbers in brackets denote the total number of images used for training or testing (base map credit: NASA Visible Earth).

<br>

![img](https://raw.githubusercontent.com/dr-lizhiwei/MSCFF/main/Results.jpg)

Fig. 3. Cloud detection examples of MSCFF in multiple types of images of different land covers

<br>

**Download Links**

- **MSCFF**: Multi-Scale Convolutional Feature Fusion model ([Link](https://raw.githubusercontent.com/dr-lizhiwei/MSCFF/main/mscff.zip))
- **HRC_WHU**: High-Resolution Google Earth Image Cloud Detection Dataset ([Link](https://github.com/dr-lizhiwei/HRC_WHU))
