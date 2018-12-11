# Field_Search_Save_Robot
Some files during developing

### Sensor setup
3D lidar, GPS, IMU, Multicameras，UWB
1. [Simultaneous exploration and segmentation for search and rescue](http://sci-hub.tw/10.1002/rob.21847)
#### Localization 
1. [3D LiDAR SLAM Integration with GPS/INS for UAVs in Urban GPS-Degraded Environments](http://sci-hub.tw/10.2514/6.2017-0448) 采用自适应卡尔曼滤波融合GPS,IMU,Lidar。
2. [INS/GPS/LiDAR Integrated Navigation System for Urban and Indoor Environments Using Hybrid Scan Matching Algorithm ](https://www.mdpi.com/1424-8220/15/9/23286/pdf) GPS,Lidar 在室内外可以交替使用，且采用了Lidar与IMU紧耦合。
3. [Robust and Precise Vehicle Localization based on Multi-sensor Fusion in Diverse City Scenes](http://sci-hub.tw/10.1109/icra.2018.8461224) 百度团队，使用了预制地图。
4. [A Robust Vehicle Localization Approach Based on GNSS/IMU/DMI/LiDAR Sensor Fusion for Autonomous Vehicles](https://www.ncbi.nlm.nih.gov/pubmed/28926996) multi-constraint fault detection approach is proposed to smooth the vehicle locations in spite of GNSS jumps
5. [GPS-LiDAR Sensor Fusion Aided by 3D City Models for UAVs](https://pdfs.semanticscholar.org/7529/a44668100610c324b08310a37666ad791910.pdf) 使用了城市三维模型
6. [A Robust Solution to High-Accuracy Geolocation: Quadruple Integration of GPS, IMU, Pseudolite, and Terrestrial Laser Scanning](https://sci-hub.tw/10.1109/tim.2010.2050981)
7. [Mapping forests using an unmanned ground vehicle with 3D LiDAR and graph-SLAM](https://sci-hub.tw/https://www.sciencedirect.com/science/article/pii/S0168169917301631) 回环检测lidar SLAM
8. [Visual-LiDAR SLAM with loop closure](http://www.nada.kth.se/~ann/exjobb/yoshua_nava.pdf)硕士论文
9. [MIM_SLAM: A Multi-Level ICP Matching Method for Mobile Robot in Large-Scale and Sparse Scenes](http://scholar.google.com/scholar_url?url=https://www.mdpi.com/2076-3417/8/12/2432/pdf&hl=zh-CN&sa=X&d=8739146617895809254&scisig=AAGBfm2fkjIJo88IXVwXnOtV5j9VxFa5Zg&nossl=1&oi=scholaralrt&hist=3Pwx2kMAAAAJ:1517064718869459059:AAGBfm1Kl9JfeLhbdQRODVtfx-m4eUMwdA) 多层ICP 

#### 3D Reconstruction 
1. [Real-time probabilistic fusion of sparse 3D LIDAR and dense stereo](https://sci-hub.tw/https://ieeexplore.ieee.org/abstract/document/7759342/) lidar visual 融合产生深度图
2. [A 3D Reconstruction with High Density and Accuracy using Laser Profiler and Camera Fusion System on a Rover](http://www.cvl.iis.u-tokyo.ac.jp/data/uploads/papers/Ishikawa_Fusion_3DV2016.pdf)
3. [PCL 点云库](https://github.com/PointCloudLibrary/pcl)
4. [PLVS](https://www.luigifreda.com/research/plvs-an-open-source-rgb-d-and-stereo-slam-for-volumetric-reconstruction-and-3d-incremental-segmentation/)
5. [TRADR](https://www.luigifreda.com/2017/03/23/tradr-review-year-3-montelibretti-work-package-4-got-excellent-evaluation/)救援机器人
6. [State of the Art on 3D Reconstruction with RGB-D Cameras](https://web.stanford.edu/~zollhoef/papers/EG18_RecoSTAR/paper.pdf)
#### 3D Mapping
1. [3D Registration of Aerial and Ground Robots for Disaster Response: An Evaluation of Features, Descriptors, and 
Transformation Estimation](https://sci-hub.tw/https://ieeexplore.ieee.org/abstract/document/8088136/)无人机配合地面机器人建图
2. [Fusing Lidar and Semantic Image Information in Octree Maps](http://www.araa.asn.au/acra/acra2017/papers/pap109s1-file1.pdf)
3. [Developing a Robust Disaster Response Robot: HIMP and the Robotics Challenge](https://sci-hub.tw/https://onlinelibrary.wiley.com/doi/abs/10.1002/rob.21696)综合性救援机器人
4. [Developing and deploying a tethered robot to map extremely steep terrain](https://sci-hub.tw/https://onlinelibrary.wiley.com/doi/abs/10.1002/rob.21813) 针对特别陡峭场地
5. [Classification of Outdoor 3D Lidar Data Based on Unsupervised Gaussian Mixture Models](https://sci-hub.tw/https://ieeexplore.ieee.org/abstract/document/7728040/) 激光点云分类
6. [Improving Path Planning and Mapping Based on Stereo Vision and Lidar ](https://sci-hub.tw/https://ieeexplore.ieee.org/abstract/document/4795550/)

#### 3D Path Planning 
1. [Normal Distributions Transform Traversability Maps: LIDAR-Only Approach for Traversability Mapping in Outdoor Environments](https://sci-hub.tw/https://onlinelibrary.wiley.com/doi/abs/10.1002/rob.21657) 识别点云内可通行区域
2. [Learned Ultra-Wideband RADAR Sensor Model for Augmented LIDAR-based Traversability Mapping in Vegetated Environments](https://sci-hub.tw/https://ieeexplore.ieee.org/abstract/document/7266662/) UWB 辅助激光建图
3. [Augmenting Traversability Maps with Ultra-Wideband Radar to Enhance Obstacle Detection in Vegetated Environments](https://sci-hub.tw/10.1109/iros.2013.6697101) 同上
4. [Real-Time Autonomous Ground Vehicle Navigation in Heterogeneous Environments Using a 3D LiDAR](https://sci-hub.tw/https://ieeexplore.ieee.org/abstract/document/8206083/) 用2D path planer做
5. [Active Autonomous Aerial Exploration for Ground Robot Path Planning](https://sci-hub.tw/https://ieeexplore.ieee.org/abstract/document/7812671/) 很贴切的论文
6. [Autonomous Planetary Exploration using LIDAR data](https://sci-hub.tw/https://ieeexplore.ieee.org/abstract/document/5152504/) 使用Delaunay 剖分
7. [https://sci-hub.tw/https://www.computer.org/csdl/proceedings/crv/2006/2542/00/25420061-abs.html](https://sci-hub.tw/https://www.computer.org/csdl/proceedings/crv/2006/2542/00/25420061-abs.html) 06年论文，也比较不错
8. [Path Planning for Autonomous Vehicles in Unknown Semi-structured Environments](https://sci-hub.tw/http://journals.sagepub.com/doi/abs/10.1177/0278364909359210) 场景不够复杂，水平停车场
9. [3D Terrestrial lidar data classification of complex natural scenes using a multi-scale dimensionality criterion:applications in geomorphology.](https://arxiv.org/pdf/1107.0550.pdf)点云分类
10. [CLASSIFICATION OF WATER SURFACES USING AIRBORNE TOPOGRAPHIC LIDAR DATA](https://www.int-arch-photogramm-remote-sens-spatial-inf-sci.net/XL-1-W1/321/2013/isprsarchives-XL-1-W1-321-2013.pdf)激光点云水路边界线分割
11. [Survey of Robot 3D Path Planning Algorithms](https://sci-hub.tw/10.1155/2016/7426913) 3D 路径规划review 2016年
12. [3D Navigation Mesh Generation for Path Planning in Uneven Terrain](https://jochen.sprickerhof.de/Sprickerhof_iav2016.pdf) 2016年
13. [Rough Terrain Reconstruction for Rover Motion Planning](https://sci-hub.tw/10.1109/crv.2010.32) 2010年

#### Multi Robots Collaboration
1. [An Online Multi-Robot SLAM System for 3D LiDARs](http://sci-hub.tw/10.1109/iros.2017.8202268) 多机器人三维激光点云匹配，有代码
2. [SegMatch: Segment based loop-closure for 3D point clouds](https://arxiv.org/pdf/1609.07720.pdf) 点云匹配方法
3. [SegMap: 3D Segment Mapping using Data-Driven Descriptors](http://www.roboticsproceedings.org/rss14/p03.pdf) 跟1， 2配合的文章
4. [Orbiting a Moving Target with Multi-Robot Collaborative Visual SLAM](https://www.cs.sfu.ca/~pingtan/Papers/rss_mvigro_2015.pdf) 
5. [multirobot_map_merge](http://wiki.ros.org/multirobot_map_merge)
6. [A ROS package that implements a multi-robot SLAM system using the condensed graphs approach](https://github.com/mtlazaro/cg_mrslam)
7. [A Cooperative SLAM Framework with Efficient Information Sharing over Mobile Ad Hoc Networks](http://ap.isr.uc.pt/archive/GMartins_dissertation_final.pdf)
8. [Collaborative Monocular SLAM with Multiple Micro Aerial Vehicles](https://www.ifi.uzh.ch/dam/jcr:9d6012bb-a1fe-4b8a-a54a-e0ead5e0f60e/IROS13_Forster_CSFM.pdf) 基于视觉的多机器人SLAM
9. [Experimental Validation of a Multirobot Distributed Receding Horizon Motion Planning Approach](https://hal.archives-ouvertes.fr/hal-01935322/document)
10. [Multi-UAV Collaborative Monocular SLAM Focusing on Data Sharing](https://sci-hub.tw/https://link.springer.com/chapter/10.1007/978-3-030-04239-4_10)
