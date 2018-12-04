# Field_Search_Save_Robot
Some files during developing

### sensor setup
3D lidar, GPS, IMU, Multicamera
#### Localization 
1. [3D LiDAR SLAM Integration with GPS/INS for UAVs in Urban GPS-Degraded Environments](http://sci-hub.tw/10.2514/6.2017-0448) 采用自适应卡尔曼滤波融合GPS,IMU,Lidar。
2. [INS/GPS/LiDAR Integrated Navigation System for Urban and Indoor Environments Using Hybrid Scan Matching Algorithm ](https://www.mdpi.com/1424-8220/15/9/23286/pdf) GPS,Lidar 在室内外可以交替使用，且采用了Lidar与IMU紧耦合。
3. [Robust and Precise Vehicle Localization based on Multi-sensor Fusion in Diverse City Scenes](http://sci-hub.tw/10.1109/icra.2018.8461224) 百度团队，使用了预制地图。
4. [A Robust Vehicle Localization Approach Based on GNSS/IMU/DMI/LiDAR Sensor Fusion for Autonomous Vehicles](https://www.ncbi.nlm.nih.gov/pubmed/28926996) multi-constraint fault detection approach is proposed to smooth the vehicle locations in spite of GNSS jumps
5. [GPS-LiDAR Sensor Fusion Aided by 3D City Models for UAVs](https://pdfs.semanticscholar.org/7529/a44668100610c324b08310a37666ad791910.pdf) 使用了城市三维模型
6. [A Robust Solution to High-Accuracy Geolocation: Quadruple Integration of GPS, IMU, Pseudolite, and Terrestrial Laser Scanning](https://sci-hub.tw/10.1109/tim.2010.2050981)
#### Sensing 

#### 3D Reconstruction 

#### 3D Path Planning 

#### Multi Robots Collaboration
1. [An Online Multi-Robot SLAM System for 3D LiDARs](http://sci-hub.tw/10.1109/iros.2017.8202268) 多机器人三维激光点云匹配，有代码
2. [SegMatch: Segment based loop-closure for 3D point clouds](https://arxiv.org/pdf/1609.07720.pdf) 点云匹配方法
3. [SegMap: 3D Segment Mapping using Data-Driven Descriptors](http://www.roboticsproceedings.org/rss14/p03.pdf) 跟1， 2配合的文章
4. [Orbiting a Moving Target with Multi-Robot Collaborative Visual SLAM](https://www.cs.sfu.ca/~pingtan/Papers/rss_mvigro_2015.pdf) 
5. [multirobot_map_merge](http://wiki.ros.org/multirobot_map_merge)
6. [A ROS package that implements a multi-robot SLAM system using the condensed graphs approach](https://github.com/mtlazaro/cg_mrslam)
7. [A Cooperative SLAM Framework with Efficient Information Sharing over Mobile Ad Hoc Networks](http://ap.isr.uc.pt/archive/GMartins_dissertation_final.pdf)
8. [Collaborative Monocular SLAM with Multiple Micro Aerial Vehicles](https://www.ifi.uzh.ch/dam/jcr:9d6012bb-a1fe-4b8a-a54a-e0ead5e0f60e/IROS13_Forster_CSFM.pdf) 基于视觉的多机器人SLAM
