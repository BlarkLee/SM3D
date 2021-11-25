# SM3D: SIMULTANEOUS MONOCULAR MAPPING AND 3D DETECTION
This is the offical repository for the implementation of our ICIP2021 pulication, SM3D. Official version is available at https://ieeexplore.ieee.org/document/9506302. Preprint version is available at https://arxiv.org/abs/2111.12643

## Abstract
Mapping and 3D detection are two major issues in vision-based robotics, and self-driving. While previous works only focus on each task separately, we present an innovative and efficient multi-task deep learning framework (SM3D) for Simultaneous Mapping and 3D Detection by bridging the gap with robust depth estimation and "Pseudo-LiDAR" point cloud for the first time. The Mapping module takes consecutive monocular frames to generate depth and pose estimation. In 3D Detection module, the depth estimation is projected into 3D space to generate "Pseudo-LiDAR" point cloud, where LiDAR-based 3D detector can be leveraged on point cloud for vehicular 3D detection and localization. By end-to-end training of both modules, the proposed mapping and 3D detection method outperforms the state-of-the-art baseline by 10.0% and 13.2% in accuracy, respectively. While achieving better accuracy, our monocular multi-task SM3D is more than 2 times faster than pure stereo 3D detector, and 18.3% faster than using two modules separately.

## Overview
![Image text](https://raw.githubusercontent.com/BlarkLee/SM3D/main/overview.png)
Overview of our SM3D. Mapping Module: Jointly learning and estimating depth and pose. 3D Detection Module: Jointly learning and estimating depth and 3D detection. Input: Monocular snippet. Output: Mapping/3D Detection & Location.
## Demo
Here is a demo video of our SM3D testing on KITTI dataset. The top video shows the original input monocular RGB frames, with 3D detection; The middle video shows the depth estimation; The bottom one shows the ego motion mapping over time. 

![](https://raw.githubusercontent.com/BlarkLee/SM3D/main/sm3d_demo.mp4)

## Code will be released soon!!!
