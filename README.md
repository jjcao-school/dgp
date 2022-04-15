# Digital Geometry 2022 (DLUT)
## 0. Introduction

Digital geometry processing (DGP), a subfield of computer graphics will be introduced in this course. Recent innovation in 3D acquisition (3D scanning, realtime depth sensor) and 3D production (3D printing) technologies, has made DGP become one of the vital technologies in applications ranging from CAD, interactive games, machine perception, robotics to other related fields. 

<!-- In this course, students should have a background in Linear Algebra and Computer Programming. -->
In this course, we study the algorithms and mathematics for representing, analyzing and manipulating geometric data. "These essential tools enable: geometric modeling for computer aided design, life-like animations for computer graphics, reliable physical simulations, and robust scene representations for computer vision." We wish students will implement a recent paper in the style of a [libigl tutorial](https://libigl.github.io/tutorial/), finally.


- Course Instructor: [Junjie Cao](http://jjcao.github.io/); Email: jjcao at dlut.edu.cn; 
- Lectures: Tuesday & Thursdays at 18:00 - 18:45, 18:55 - 19:40. 研教楼312.
- Textbook: <img src="https://images.tandf.co.uk/common/jackets/amazon/978156881/9781568814261.jpg"  width="20%" alt="M. Botsch, L. Kobbelt, M. Pauly, P. Alliez, and B. Lévy. Polygon mesh processing. CRC press, 2010." />
    [pdf](ftp://nozdr.ru/biblio/kolxo3/Cs/CsCg/Botsch%20M.,%20et%20al.%20Polygon%20mesh%20processing%20(AK%20Peters,%202010)(ISBN%201568814267)(C)(O)(243s)_CsCg_.pdf), with ppt & source code @ http://www.pmp-book.org.

## 1. Schedule
- [00_introduction](http://pan-yz.chaoxing.com/share/info/500d49595b4a971f)
- [01_03_01_meshes and manifolds](http://pan-yz.chaoxing.com/share/info/1a9e9608117f5f34)
- [01_03_02_meshes_datastructure](http://pan-yz.chaoxing.com/share/info/fa2e339d573f3d7e): Halfedge
- [02_01_points](): knn, filter
- 3d Scanning, [slider](http://pan-yz.chaoxing.com/share/info/3f34fcb074ff80e7)
  - Active Illumination Methods
    - Time of Flight Method, slider, [video](https://fpcv.cs.columbia.edu/)
    - LiDAR
- ### 1.1 LiDAR denosing
- [04_00_smoothing](http://pan-yz.chaoxing.com/share/info/715cb34431d2ebdb):
- 1 Airborne Particle Classification in LiDAR Point Clouds Using Deep Learning, fsr19
- 2 Weather Classification Using an Automotive LIDAR Sensor Based on Detections on Asphalt and Atmosphere, Sensors, 20
- 3 LaNoising: A Data-driven Approach for 903nm ToF LiDAR Performance Modeling under Fog, IROS 20
- 4 Deep Learning Method on Target Echo Signal Recognition for Obscurant Penetrating Lidar Detection in Degraded Visual Environments, sensors, 20.
- 5 Fast and Accurate Desnowing Algorithm for LiDAR Point Clouds, access, 20
- 6 Robust Multimodal Vehicle Detection in Foggy Weather Using Complementary Lidar and Radar Signals, cvpr 21
- 7 nuScenes: A Multimodal Dataset for Autonomous Driving, cvpr20
- 8 Seeing Through Fog Without Seeing Fog: Deep Multimodal Sensor Fusion in Unseen Adverse Weather, cvpr 20

### 1.2 Points
- [02_02_unoriented_normals](): PCA, RANSAC, n-jet
- [02_03_oriented_normals](): 
- [02_03_consolidation](): 
- [05_01_icp]()
- [05_01_matching]():
- [surface reconstruction - introduction](http://pan-yz.chaoxing.com/share/info/559b1b07ec8aad26)
- [surface reconstruction - RBF, MLS](http://pan-yz.chaoxing.com/share/info/27f75a18160b9dd1)
- [surface reconstruction - Poisson](http://pan-yz.chaoxing.com/share/info/c08e4dc471e3cf4b)
- [surface reconstruction - SSD](http://pan-yz.chaoxing.com/share/info/5654e17799fdcd95)
- 
- ### 1.2 Point cloud denoising
- 1. Dynamic point cloud denoising via manifold-to-manifold distance，TIP 2021. （点云序列的去噪）
- 2. RePCD-Net: Feature-Aware Recurrent Point Cloud Denoising Network，IJCV 2022.
- 3. PC2-PU: Patch Correlation and Position Correction for Effective Point Cloud Upsampling，2021
- 4. Rethinking Point Cloud Filtering: A Non-Local Position Based Approach，CAD 2022 （3，4都考虑了相似patch的问题）
- 5. Deep Point Set Resampling via Gradient Fields，2022.（score+拉普拉斯）
- 6. PD-Flow: A Point Cloud Denoising Framework with Normalizing Flows，2022

- ### 1.3 Detection
- 1. DisARM: Displacement Aware Relation Module for 3D Detection，CVPR2022，（室内检测）
- 2. Point2Seq: Detecting 3D Objects as Sequences，CVPR2022
- 3. SE-SSD: Self-Ensembling Single-Stage Object Detector From Point Cloud，CVPR2021，
- 4. Pv-rcnn++: Point-voxel feature set abstraction with local vector representation for 3d object detection
- 5. Embracing Single Stride 3D Object Detector with Sparse Transformer, cvpr 22

- ### 1.4 Tracing
- 1. PTTR: Relational 3D Point Cloud Object Tracking with Transformer，CVPR2022
- 2. 3D Siamese Voxel-to-BEV Tracker for Sparse Point Clouds，NIPS2021
- 3. Beyond 3D Siamese Tracking: A Motion-Centric Paradigm for 3D - 4. Single Object Tracking in Point Clouds，CVPR2022
- 5. Exploring Simple 3D Multi-Object Tracking for Autonomous Driving，ICCV2021（多目标）

- ### 1.5 Normal Estimation
- 1. Deep Iterative Surface Normal Estimations, cvpr 2020.
- 2. DeepFit: 3D Surface Fitting via Neural Network Weighted Least Squares, eccv 2020
- 3. PCPNET: Learning Local Shape Properties from Raw Point Clouds, eg 2018
- 4. Latent Tangent Space Representation for Normal Estimation, tie 2021
- 5. Normal Estimation for Accurate 3D Mesh Reconstruction with Point Cloud Model Incorporating Spatial Structure, cvpr workshop 2019
- 6. Geometry Guided Deep Surface Normal Estimation. CAD 22.

### Implicit neural representations [1]
- Convolutional Occupancy Networks
- Implicit Functions in Feature Space for 3D Shape Reconstruction and Completion, 19
- 
- DeepSDF: Learning Continuous Signed Distance Functions for Shape Representation, 19
- Deep Local Shapes: Learning Local SDF Priors for Detailed 3D Reconstruction 2020
- PatchNets: Patch-Based Generalizable Deep Implicit 3D Shape Representations 2021
- 
- MetaSDF: Meta-learning Signed Distance Functions, 2020

### Implicit neural representations [2]
- Points2Surf 2020
- Local Deep Implicit Functions for 3D Shape 2020 [a set of ellipses]
- Neural Unsigned Distance Fields for ImplicitFunction Learning 2020
- Neural Geometric Level of Detail: Real-time Rendering with Implicit 3D Shapes 2021 [octree]

### Implicit neural representations [3]
- Scene Representation Networks: Continuous 3D-Structure-Aware Neural Scene Representations, NeurIPS 2019.
- Implicit Geometric Regularization for Learning Shapes, 2020, Yaron Lipman
- SAL: Sign Agnostic Learning of Shapes from Raw Data 2020
- SALD: Sign Agnostic Learning with Derivatives, icld 2021
- **[SIREN2020], Implicit Neural Representations with Periodic Activation Functions, NeurIPS 2020 (Oral)**


### 1.1 Representations
- [01_00_geometry & its representations](http://pan-yz.chaoxing.com/share/info/bce1099958c1faaf)
- [01_01_implicit_representations](http://pan-yz.chaoxing.com/share/info/4d2497d6e132c4d1)
- [01_02_explicit_representations](http://pan-yz.chaoxing.com/share/info/d6056d09fb0fab80)

- [01_04_implicit_explicit_conversion](http://pan-yz.chaoxing.com/share/info/8e58aec9f08e3a00): Fast Marching, Marching Cube
  
### 1.3 Meshes
- [04_00_remeshing](http://pan-yz.chaoxing.com/share/info/efcea209e9db3ad1):
- [vector field](http://pan-yz.chaoxing.com/share/info/4cb4b53b2a094c5e): simple version
- [07_parameterization](http://pan-yz.chaoxing.com/share/info/7d6968f1f2aa12b3):
- [space deformation](http://pan-yz.chaoxing.com/share/info/a29cb47c36f2815c):
- [surface deformation](http://pan-yz.chaoxing.com/share/info/292c93d2206c6550):
### 1.4 Discrete Differential Geometry  
- [Continuous Differential Geometry-Curve]():
- [Continuous Differential Geometry-Surface]():
- [Discrete Differential Geometry]():
  
## 2. Assignments
- [Rules & Setup](assignments/), deadline: 1st weekend
- [Assignment 1: Hello World (Mesh display, Connected Components & Subdivision)](assignments/Assignment_1), deadline: 2nd weekend
- [Assignment 2: Implicit Surface Reconstruction](assignments/Assignment_2), deadline: TBD
- [Assignment 3: Normals, Curvatures, and Smoothing](assignments/Assignment_3), deadline: TBD
- [Assignment 4: Mesh Parameterization](assignments/Assignment_4), deadline: TBD
- [Assignment 5: Shape Deformation](assignments/Assignment_5), deadline: TBD

## 3. Reading Topics
### Deep point basic
- Self-Supervised Deep Learning on Point Clouds by Reconstructing Space, nips 19
- PointContrast: Unsupervised Pre-training for 3D Point Cloud Understanding, ECCV, 2020.
- PointAugment: An Auto-Augmentation Framework for Point Cloud Classification
- A Simple Framework for Contrastive Learning of Visual Representations
- fixmatch，nips 2020

### Detection & Tracking
- Robust Multi-Modality Multi-Object Tracking, iccv 2019
- Probabilistic 3D Multi-Modal, Multi-Object Tracking
for Autonomous Driving 2020
- PointFusion: Deep Sensor Fusion for 3D Bounding Box Estimation (2018CVPR)
- Center-based 3d object detection and tracking
- Detection and Tracking of Small Objects in Sparse 3D Laser Range Data, 2019, ICRA

<!--
### Implicit neural representations [4]
- Neural Volumes: Learning Dynamic Renderable Volumes from Images, sig19
- Deep Implicit Templates for 3D Shape Representation, 2020
- DIST: Rendering deep implicit signed distance function with differentiable sphere tracing, cvpr20
- SDFDiff: Differentiable rendering of signed distance fields for 3D shape optimization, cvpr20 -->
  
<!-- ### Matching -->
<!-- ### Reconstruction
- Deep Marching Cubes: Learning Explicit Surface Representations, cvpr18 
- Analytic Marching: An Analytic Meshing Solution from Deep Implicit Surface Networks 2020
- MeshSDF: Differentiable Iso-Surface Extraction, 2020 [image 2 mesh]
- PIFu: Pixel-Aligned Implicit Function for High-Resolution Clothed Human Digitization
- ARCH: Animatable Reconstruction of Clothed Humans (CVPR 2020)
- Multiview Neural Surface Reconstruction by Disentangling Geometry and Appearance 2020 -->
- 
## 4. Resources
### Suggestions [->](https://github.com/jjcao-school/common/tree/main/for_students)

### Softwares [->](softwares/) 
- Deep Exploration (or its next version: SAP Visual Enterprise Author) for browsing, converting & simplifing meshes
- MeshLab: mesh viewer & large amount of basic operations
- [CloudCompare](https://www.danielgm.net/cc/): 3D point cloud and mesh processing software

### References:
- [Geometric Modeling - CSCI-GA.3033-018, Daniele Panozzo](https://github.com/danielepanozzo/gp)


<!-- <li>[Book]: <img src="https://images-na.ssl-images-amazon.com/images/I/41ahRBWW%2BjL._SX335_BO1,204,203,200_.jpg"  width="20%" alt="A Sampler of Useful Computational Tools for Applied Geometry, Computer Graphics, and Image Processing. Daniel Cohen-Or, Chen Greif, Tao Ju, Niloy J. Mitra, Ariel Shamir, Olga Sorkine-Hornung, Hao Zhang, 2015." />
    </li>
<li>[Course]: Geometric Computing with Python, SIGGRAPH course 2018, Daniele Panozzo.</li>
<li>[Course]: CSCI 621: Digital Geometry Processing SS 2019, Hao Li. PMP, scanning, Dynamic Geometry processing, facial performance capture, deep learning for geometry. PMP execises.</li>
<li>[Course]: CS749: Digital Geometry Processing, Spring 2017, Siddhartha Chaudhuri. Points, diatances, features, Laplacian, segmentation. Many reading materials, better assignments. 
<li>[Course]: CENG789 - Digital Geometry Processing, Yusuf Sahillioğlu. PMP, Delaunay, Voronoi, Descriptors on mesh, 3D printing. Some team projects topics.</li>
<li>[Course]: 6.838: Shape Analysis (Spring 2017) @ MIT. Numerical Tools, geodesic, inverse distance, Laplacian, Vector field, Optimal transport, correspondence. with youtube. 4 homework by ipython notebook.</li>
<li>[Course]: CS 15-458/858: Discrete Differential Geometry, @CMU by  Keenan Crane</li>
<li>[Course]: Digital Geometry Processing 2019, Xiao-Ming Fu. Barycentric coordinate, Mapping, PolyCube, Atlas, Spere parameterization, Morping. PMP exscises topics with assigned new papers.</li>
<li>...</li>
<li>[Course]: ENGN 2501 Digital Geometry Processing, Gabriel Taubin, 2019</li>

<li>[Course]: 524 Computer Graphics: Modeling - Alla Sheffer</li>
<li>[Course]: CS468 - Data-Driven Shape Analysis - Vladimir (Vova) Kim, & Qixing (Peter) Huan</li>
<li>[Course]: Advanced Topics in Computer Graphics: Mesh Processing (600.657) - Michael Misha Kazhdan</li>
<li>[Course]: SIGGRAPH AISA 2008 course: Mesh Parameterization: Theory and Practice</li>
<li>[Course]: SIGGRAPH Asia 2009 course: Spectral Mesh Processing</li>
<li>[Course]: SIGGRAPH 2014 course: Structure-Aware Shape Processing</li>
<li>[Course]: Eurographics 2014 course: State of the Art in Surface Reconstruction from Point Clouds</li>
<li>[Course]: SGP 2015 course: Dynamic 2D/3D Registration</li>
<li>[Course]: Graduate School of SGP 2017. lecture videos</li>
 -->
