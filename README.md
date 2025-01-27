# C2P-Net：Comprehensive Depth Map to Planar Depth Conversion for Room Layout Estimation
This is PyTorch implementation of our paper "C2P-Net：Comprehensive Depth Map to Planar Depth Conversion for Room Layout Estimation".
![An overview of C2P-Net for panoramic images.](figure/pano_framework4.png)

Room layout estimation seeks to infer the overall spatial configuration of indoor scenes using perspective or panoramic images. As the layout is determined by the dominant indoor planes, this problem inherently requires the reconstruction of these planes. Some studies reconstruct indoor planes from perspective images by learning pixel-level or instance-level plane parameters. However, directly learning these parameters has the problems of susceptibility to occlusions and position dependency. In this paper, we introduce the Comprehensive depth map to Planar depth (C2P) conversion, which reformulates planar depth reconstruction into the prediction of a comprehensive depth map and planar visibility confidence. Based on the parametric representation of planar depth we propose, the C2P conversion is applicable to both panoramic and perspective images. Accordingly, we present an effective framework for room layout estimation that jointly learns the comprehensive depth map and planar visibility confidence. Due to the differentiability of the C2P conversion, our network autonomously learns planar visibility confidence by constraining the estimated plane parameters and reconstructed planar depth map. We further propose a novel approach for 3D layout generation through sequential planar depth map integration. Experimental results demonstrate the superiority of our method across all evaluated panoramic and perspective datasets.


#### Visual results
![The visual results of panoramic layout estimation on MatterportLayout datase.](figure/pano_visual4.png)


![The visual results of perspective layout estimation on Matterport3D-Layout and InteriorNet-Layout datasets.](figure/pers_visual3.png)


## Note
At present, this project has not been made public, but we plan to open source to the community. You are welcome to discuss the functional requirements and contribution methods of the project here and get relevant information in advance！
