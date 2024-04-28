# EgoFormer: Ego-Gesture Classification in Context of Autonomous Driving <br/>
 Link to paper: [![Paper](https://img.shields.io/badge/paper-IEEE%20Sensors-blue)](https://ieeexplore.ieee.org/document/10508297)

## Abstract <br/>
<p style="text-align: justify"> Decoding the intentions of passengers and other road users remains a critical challenge for autonomous vehicles and intelligent transportation systems. Hand gestures are key in these interactions, offering a direct communication channel. Moreover, egocentric videos mimic a first-person perspective, aligning closely with human visual perception. Yet, the development of deep learning algorithms for detecting egocentric hand gestures in autonomous driving is hindered by the absence of useful datasets. Furthermore, there is a pressing need for gesture recognition methods to evolve from CNN-based architectures to transformer models. To address these challenges, we present EgoDriving, a novel dataset of egocentric hand gestures, curated for driving-related hand gestures. Finally, we introduce EgoFormer, an efficient video transformer for egocentric hand gesture classification that is optimized for edge computing deployments. EgoFormer incorporates a Video Dynamic Position Bias (VDPB) module to enhance long-range positional awareness and leverage absolute positions from convolutional sub-layers within its transformer blocks. Designed for low-resource settings, EgoFormer offers substantial reductions in inference latency and GPU utilization while maintaining competitive accuracy against state-of-the-art hand gesture recognition frameworks.</p>

## EgoDriving Dataset
<img src = "images/Qazi3_Hand_gestures.jpg " alt="Raw image" width="50%" align="center"/>

## Overall pipeline
<img src = "images/Egoformer_pipeline.png " alt="Raw image" width="50%" align="center"/> 

## VDPB
<img src = "images/VDPB.png " alt="Raw image" width="50%" align="center"/>
