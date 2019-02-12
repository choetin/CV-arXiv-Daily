# CV-arXiv-Daily

**分享计算机视觉每天的arXiv文章，主要集中在目标检测，单目标跟踪，多目标跟踪，人体行为识别，人体姿态估计与跟踪，行人重识别，模型搜索等。每周周末会将本周的Archive起来**

[2019-01-23~2019-01-26](2019/2019.01.23-2019.01.26.md)

[2019-01-28~2019-02-01](2019/2019.01.28-2019.02.01.md)

**2019-02-12**

[1] activity prediction文章

论文题目：Peeking into the Future: Predicting Future Person Activities and Locations in Videos

作者：Junwei Liang, Lu Jiang, Juan Carlos Niebles, Alexander Hauptmann, Li Fei-Fei

文章链接：https://arxiv.org/abs/1902.03748

摘要：Deciphering human behaviors to predict their future paths/trajectories and what they would do from videos is important in many applications. Motivated by this idea, this paper studies predicting a pedestrian's future path jointly with future activities. We propose an end-to-end, multi-task learning system utilizing rich visual features about the human behavioral information and interaction with their surroundings. To facilitate the training, the network is learned with two auxiliary tasks of predicting future activities and the location in which the activity will happen. Experimental results demonstrate our state-of-the-art performance over two public benchmarks on future trajectory prediction. Moreover, our method is able to produce meaningful future activity prediction in addition to the path. The result provides the first empirical evidence that a joint modeling of paths and activities benefits future path prediction.

[2] ICRA 2019 SLAM文章

论文题目：Visual SLAM: Why Bundle Adjust?

作者：Alvaro Parra Bustos, Tat-Jun Chin, Anders Eriksson, Ian Reid

文章链接：https://arxiv.org/abs/1902.03747

摘要：Bundle adjustment plays a vital role in feature-based monocular SLAM. In many modern SLAM pipelines, bundle adjustment is performed to estimate the 6DOF camera trajectory and 3D map (3D point cloud) from the input feature tracks. However, two fundamental weaknesses plague SLAM systems based on bundle adjustment. First, the need to carefully initialise bundle adjustment means that all variables, in particular the map, must be estimated as accurately as possible and maintained over time, which makes the overall algorithm cumbersome. Second, since estimating the 3D structure (which requires sufficient baseline) is inherent in bundle adjustment, the SLAM algorithm will encounter difficulties during periods of slow motion or pure rotational motion. 
We propose a different SLAM optimisation core: instead of bundle adjustment, we conduct rotation averaging to incrementally optimise only camera orientations. Given the orientations, we estimate the camera positions and 3D points via a quasi-convex formulation that can be solved efficiently and globally optimally. Our approach not only obviates the need to estimate and maintain the positions and 3D map at keyframe rate (which enables simpler SLAM systems), it is also more capable of handling slow motions or pure rotational motions.

[3] Dense Depth Estimation文章

论文题目：A Motion Free Approach to Dense Depth Estimation in Complex Dynamic Scene

作者：Suryansh Kumar, Ram Srivatsav Ghorakavi, Yuchao Dai, Hongdong Li

文章链接：https://arxiv.org/abs/1902.03791

摘要：Despite the recent success in per-frame monocular dense depth estimation of rigid scenes using deep learning methods, they fail to achieve similar success for complex dynamic scenes, such as MPI Sintel \cite{butler2012naturalistic}. Moreover, conventional geometric methods to address this problem using a piece-wise rigid scene model requires a reliable estimation of motion parameters for each local model, which is difficult to obtain and validate. In this work, we show that, given per-pixel optical flow correspondences between two consecutive frames and the sparse depth prior for the reference frame, we can recover the dense depth map for the successive frames without solving for motion parameters. By assigning the locally rigid structure to the piece-wise planar approximation of a dynamic scene which transforms as rigid as possible over frames, we demonstrate that we can bypass the motion estimation step. In essence, our formulation provides a new way to think and recover dense depth map of a complex dynamic scene which is recursive, incremental and motion free in nature and therefore, it can also be integrated with the modern neural network frameworks for large-scale depth-estimation applications. Our proposed method does not make any prior assumption about the rigidity of a dynamic scene, as a result, it is applicable to a wide range of scenarios. Experimental results show that our method can effectively provide the depth for the successive/multiple frames of a dynamic scene without using any motion parameters.

[4] SLAM文章

论文题目：UcoSLAM: Simultaneous Localization and Mapping by Fusion of KeyPoints and Squared Planar Markers

作者：Rafael Munoz-Salinas, Rafael Medina-Carnicer

文章链接：https://arxiv.org/abs/1902.03729

摘要：This paper proposes a novel approach for Simultaneous Localization and Mapping by fusing natural and artificial landmarks. Most of the SLAM approaches use natural landmarks (such as keypoints). However, they are unstable over time, repetitive in many cases or insufficient for a robust tracking (e.g. in indoor buildings). On the other hand, other approaches have employed artificial landmarks (such as squared fiducial markers) placed in the environment to help tracking and relocalization. We propose a method that integrates both approaches in order to achieve long-term robust tracking in many scenarios. 
Our method has been compared to the start-of-the-art methods ORB-SLAM2 and LDSO in the public dataset Kitti, Euroc-MAV, TUM and SPM, obtaining better precision, robustness and speed. Our tests also show that the combination of markers and keypoints achieves better accuracy than each one of them independently.

[5] 运动目标分割文章

论文题目：Towards Segmenting Everything That Moves

作者：Achal Dave, Pavel Tokmakov, Deva Ramanan

文章链接：https://arxiv.org/abs/1902.03715

摘要：Video analysis is the task of perceiving the world as it changes. Often, though, most of the world doesn't change all that much: it's boring. For many applications such as action detection or robotic interaction, segmenting all moving objects is a crucial first step. While this problem has been well-studied in the field of spatiotemporal segmentation, virtually none of the prior works use learning-based approaches, despite significant advances in single-frame instance segmentation. We propose the first deep-learning based approach for video instance segmentation. Our two-stream models' architecture is based on Mask R-CNN, but additionally takes optical flow as input to identify moving objects. It then combines the motion and appearance cues to correct motion estimation mistakes and capture the full extent of objects. We show state-of-the-art results on the Freiburg Berkeley Motion Segmentation dataset by a wide margin. One potential worry with learning-based methods is that they might overfit to the particular type of objects that they have been trained on. While current recognition systems tend to be limited to a "closed world" of N objects on which they are trained, our model seems to segment almost anything that moves.

[6] MOT+segmentation数据集

论文题目：MOTS: Multi-Object Tracking and Segmentation

作者：Paul Voigtlaender, Michael Krause, Aljosa Osep, Jonathon Luiten, Berin Balachandar Gnana Sekar, Andreas Geiger, Bastian Leibe

文章链接：https://arxiv.org/abs/1902.03604

摘要：This paper extends the popular task of multi-object tracking to multi-object tracking and segmentation (MOTS). Towards this goal, we create dense pixel-level annotations for two existing tracking datasets using a semi-automatic annotation procedure. Our new annotations comprise 70,430 pixel masks for 1,084 distinct objects (cars and pedestrians) in 10,870 video frames. For evaluation, we extend existing multi-object tracking metrics to this new task. Moreover, we propose a new baseline method which jointly addresses detection, tracking, and segmentation with a single convolutional network. We demonstrate the value of our datasets by achieving improvements in performance when training on MOTS annotations. We believe that our datasets, metrics and baseline will become a valuable resource towards developing multi-object tracking approaches that go beyond 2D bounding boxes.

[7] CVIU 2019 Face-SSD文章

论文题目：Registration-free Face-SSD: Single shot analysis of smiles, facial attributes, and affect in the wild

作者：Youngkyoon Jang, Hatice Gunes, Ioannis Patras

文章链接：https://arxiv.org/abs/1902.04042

摘要：In this paper, we present a novel single shot face-related task analysis method, called Face-SSD, for detecting faces and for performing various face-related (classification/regression) tasks including smile recognition, face attribute prediction and valence-arousal estimation in the wild. Face-SSD uses a Fully Convolutional Neural Network (FCNN) to detect multiple faces of different sizes and recognise/regress one or more face-related classes. Face-SSD has two parallel branches that share the same low-level filters, one branch dealing with face detection and the other one with face analysis tasks. The outputs of both branches are spatially aligned heatmaps that are produced in parallel - therefore Face-SSD does not require that face detection, facial region extraction, size normalisation, and facial region processing are performed in subsequent steps. Our contributions are threefold: 1) Face-SSD is the first network to perform face analysis without relying on pre-processing such as face detection and registration in advance - Face-SSD is a simple and a single FCNN architecture simultaneously performing face detection and face-related task analysis - those are conventionally treated as separate consecutive tasks; 2) Face-SSD is a generalised architecture that is applicable for various face analysis tasks without modifying the network structure - this is in contrast to designing task-specific architectures; and 3) Face-SSD achieves real-time performance (21 FPS) even when detecting multiple faces and recognising multiple classes in a given image. Experimental results show that Face-SSD achieves state-of-the-art performance in various face analysis tasks by reaching a recognition accuracy of 95.76% for smile detection, 90.29% for attribute prediction, and Root Mean Square (RMS) error of 0.44 and 0.39 for valence and arousal estimation.

[8] Biomedical Image Segmentation文章

论文题目：MultiResUNet : Rethinking the U-Net Architecture for Multimodal Biomedical Image Segmentation

作者：Nabil Ibtehaz, M. Sohel Rahman

文章链接：https://arxiv.org/abs/1902.04049

摘要：In recent years Deep Learning has brought about a breakthrough in Medical Image Segmentation. U-Net is the most prominent deep network in this regard, which has been the most popular architecture in the medical imaging community. Despite outstanding overall performance in segmenting multimodal medical images, from extensive experimentations on challenging datasets, we found out that the classical U-Net architecture seems to be lacking in certain aspects. Therefore, we propose some modifications to improve upon the already state-of-the-art U-Net model. Hence, following the modifications we develop a novel architecture MultiResUNet as the potential successor to the successful U-Net architecture. We have compared our proposed architecture MultiResUNet with the classical U-Net on a vast repertoire of multimodal medical images. Albeit slight improvements in the cases of ideal images, a remarkable gain in performance has been attained for challenging images. We have evaluated our model on five different datasets, each with their own unique challenges, and have obtained a relative improvement in performance of 10.15%, 5.07%, 2.63%, 1.41%, and 0.62% respectively.

[9] Face Recognition文章

论文题目：Cross-spectral Face Completion for NIR-VIS Heterogeneous Face Recognition

作者：Ran He, Jie Cao, Lingxiao Song, Zhenan Sun, Tieniu Tan

文章链接：https://arxiv.org/abs/1902.03565

摘要：Near infrared-visible (NIR-VIS) heterogeneous face recognition refers to the process of matching NIR to VIS face images. Current heterogeneous methods try to extend VIS face recognition methods to the NIR spectrum by synthesizing VIS images from NIR images. However, due to self-occlusion and sensing gap, NIR face images lose some visible lighting contents so that they are always incomplete compared to VIS face images. This paper models high resolution heterogeneous face synthesis as a complementary combination of two components, a texture inpainting component and pose correction component. The inpainting component synthesizes and inpaints VIS image textures from NIR image textures. The correction component maps any pose in NIR images to a frontal pose in VIS images, resulting in paired NIR and VIS textures. A warping procedure is developed to integrate the two components into an end-to-end deep network. A fine-grained discriminator and a wavelet-based discriminator are designed to supervise intra-class variance and visual quality respectively. One UV loss, two adversarial losses and one pixel loss are imposed to ensure synthesis results. We demonstrate that by attaching the correction component, we can simplify heterogeneous face synthesis from one-to-many unpaired image translation to one-to-one paired image translation, and minimize spectral and pose discrepancy during heterogeneous recognition. Extensive experimental results show that our network not only generates high-resolution VIS face images and but also facilitates the accuracy improvement of heterogeneous face recognition.

[10] 

论文题目：NeurAll: Towards a Unified Model for Visual Perception in Automated Driving

作者：Ganesh Sistu, Isabelle Leang, Sumanth Chennupati, Stefan Milz, Senthil Yogamani, Samir Rawashdeh

文章链接：https://arxiv.org/abs/1902.03589

摘要：Convolutional Neural Networks (CNNs) are successfully used for the important automotive visual perception tasks including object recognition, motion and depth estimation, visual SLAM, etc. However, these tasks are independently explored and modeled. In this paper, we propose a joint multi-task network design called NeurAll for learning all tasks simultaneously. Our main motivation is the computational efficiency achieved by sharing the expensive initial convolutional layers between all tasks. Indeed, the main bottleneck in automated driving systems is the limited processing power available on deployment hardware. There could be other benefits in improving accuracy for some tasks and it eases development effort. It also offers scalability to add more tasks leveraging existing features and achieving better generalization. We survey various CNN based solutions for visual perception tasks in automated driving. Then we propose a unified CNN model for the important tasks and discuss several advanced optimization and architecture design techniques to improve the baseline model. The paper is partly review and partly positional with demonstration of several preliminary results promising for future research. Firstly, we show that an efficient two-task model performing semantic segmentation and object detection achieves similar accuracies compared to separate models on various datasets with minimized runtime. We then illustrate that using depth regression as auxiliary task improves semantic segmentation and using multi-stream semantic segmentation outperforms one-stream semantic segmentation. The two-task network achieves 30 fps on an automotive grade low power SOC for 1280x384 image resolution

[11] 3D Hand Pose文章

论文题目：3D Hand Shape and Pose from Images in the Wild

作者：Adnane Boukhayma, Rodrigo de Bem, Philip H.S. Torr

文章链接：https://arxiv.org/abs/1902.03451

摘要：We present in this work the first end-to-end deep learning based method that predicts both 3D hand shape and pose from RGB images in the wild. Our network consists of the concatenation of a deep convolutional encoder, and a fixed model-based decoder. Given an input image, and optionally 2D joint detections obtained from an independent CNN, the encoder predicts a set of hand and view parameters. The decoder has two components: A pre-computed articulated mesh deformation hand model that generates a 3D mesh from the hand parameters, and a re-projection module controlled by the view parameters that projects the generated hand into the image domain. We show that using the shape and pose prior knowledge encoded in the hand model within a deep learning framework yields state-of-the-art performance in 3D pose prediction from images on standard benchmarks, and produces geometrically valid and plausible 3D reconstructions. Additionally, we show that training with weak supervision in the form of 2D joint annotations on datasets of images in the wild, in conjunction with full supervision in the form of 3D joint annotations on limited available datasets allows for good generalization to 3D shape and pose predictions on images in the wild.

[12] 网络结构压缩文章

论文题目：Architecture Compression

作者：Anubhav Ashok

文章链接：https://arxiv.org/abs/1902.03326

摘要：In this paper we propose a novel approach to model compression termed Architecture Compression. Instead of operating on the weight or filter space of the network like classical model compression methods, our approach operates on the architecture space. A 1-D CNN encoder-decoder is trained to learn a mapping from discrete architecture space to a continuous embedding and back. Additionally, this embedding is jointly trained to regress accuracy and parameter count in order to incorporate information about the architecture's effectiveness on the dataset. During the compression phase, we first encode the network and then perform gradient descent in continuous space to optimize a compression objective function that maximizes accuracy and minimizes parameter count. The final continuous feature is then mapped to a discrete architecture using the decoder. We demonstrate the merits of this approach on visual recognition tasks such as CIFAR-10, CIFAR-100, Fashion-MNIST and SVHN and achieve a greater than 20x compression on CIFAR-10.

**2019-02-11**

[1] Action Prediction文章

论文题目：Skeleton-Based Online Action Prediction Using Scale Selection Network

作者：Jun Liu, Amir Shahroudy, Gang Wang, Ling-Yu Duan, Alex C. Kot

文章链接：https://arxiv.org/abs/1902.03084

摘要：Action prediction is to recognize the class label of an ongoing activity when only a part of it is observed. In this paper, we focus on online action prediction in streaming 3D skeleton sequences. A dilated convolutional network is introduced to model the motion dynamics in temporal dimension via a sliding window over the temporal axis. Since there are significant temporal scale variations in the observed part of the ongoing action at different time steps, a novel window scale selection method is proposed to make our network focus on the performed part of the ongoing action and try to suppress the possible incoming interference from the previous actions at each step. An activation sharing scheme is also proposed to handle the overlapping computations among the adjacent time steps, which enables our framework to run more efficiently. Moreover, to enhance the performance of our framework for action prediction with the skeletal input data, a hierarchy of dilated tree convolutions are also designed to learn the multi-level structured semantic representations over the skeleton joints at each frame. Our proposed approach is evaluated on four challenging datasets. The extensive experiments demonstrate the effectiveness of our method for skeleton-based online action prediction.

[2] 3D Human Pose Estimation文章

论文题目：3D Human Pose Estimation from Deep Multi-View 2D Pose

作者：Steven Schwarcz, Thomas Pollard

文章链接：https://arxiv.org/abs/1902.02841

摘要：Human pose estimation - the process of recognizing a human's limb positions and orientations in a video - has many important applications including surveillance, diagnosis of movement disorders, and computer animation. While deep learning has lead to great advances in 2D and 3D pose estimation from single video sources, the problem of estimating 3D human pose from multiple video sensors with overlapping fields of view has received less attention. When the application allows use of multiple cameras, 3D human pose estimates may be greatly improved through fusion of multi-view pose estimates and observation of limbs that are fully or partially occluded in some views. Past approaches to multi-view 3D pose estimation have used probabilistic graphical models to reason over constraints, including per-image pose estimates, temporal smoothness, and limb length. In this paper, we present a pipeline for multi-view 3D pose estimation of multiple individuals which combines a state-of-art 2D pose detector with a factor graph of 3D limb constraints optimized with belief propagation. We evaluate our results on the TUM-Campus and Shelf datasets for multi-person 3D pose estimation and show that our system significantly out-performs the previous state-of-the-art with a simpler model of limb dependency.

[3] 单目标跟踪文章

论文题目：SiamVGG: Visual Tracking using Deeper Siamese Networks

作者：Yuhong Li, Xiaofan Zhang

文章链接：https://arxiv.org/abs/1902.02804

摘要：Recently, we have seen a rapid development of Deep Neural Network (DNN) based visual tracking solutions. Some trackers combine the DNN-based solutions with Discriminative Correlation Filters (DCF) to extract semantic features and successfully deliver the state-of-the-art tracking accuracy. However, these solutions are highly compute-intensive, which require long processing time, resulting unsecured real-time performance. To deliver both high accuracy and reliable real-time performance, we propose a novel tracker called SiamVGG. It combines a Convolutional Neural Network (CNN) backbone and a cross-correlation operator, and takes advantage of the features from exemplary images for more accurate object tracking. 
The architecture of SiamVGG is customized from VGG-16, with the parameters shared by both exemplary images and desired input video frames. 
We demonstrate the proposed SiamVGG on OTB-2013/50/100 and VOT 2015/2016/2017 datasets with the state-of-the-art accuracy while maintaining a decent real-time performance of 50 FPS running on a GTX 1080Ti. Our design can achieve 2% higher Expected Average Overlap (EAO) compared to the ECO and C-COT in VOT2017 Challenge.



**2019-02-08**

[1] 全景分割文章

论文题目：Single Network Panoptic Segmentation for Street Scene Understanding

作者：Daan de Geus, Panagiotis Meletis, Gijs Dubbelman

论文链接：https://arxiv.org/abs/1902.02678

摘要: In this work, we propose a single deep neural network for panoptic segmentation, for which the goal is to provide each individual pixel of an input image with a class label, as in semantic segmentation, as well as a unique identifier for specific objects in an image, following instance segmentation. Our network makes joint semantic and instance segmentation predictions and combines these to form an output in the panoptic format. This has two main benefits: firstly, the entire panoptic prediction is made in one pass, reducing the required computation time and resources; secondly, by learning the tasks jointly, information is shared between the two tasks, thereby improving performance. Our network is evaluated on two street scene datasets: Cityscapes and Mapillary Vistas. By leveraging information exchange and improving the merging heuristics, we increase the performance of the single network, and achieve a score of 23.9 on the Panoptic Quality (PQ) metric on Mapillary Vistas validation, with an input resolution of 640 x 900 pixels. On Cityscapes validation, our method achieves a PQ score of 45.9 with an input resolution of 512 x 1024 pixels. Moreover, our method decreases the prediction time by a factor of 2 with respect to separate networks.

[2] 自动驾驶中的交通锥检测文章

论文题目：Real-time 3D Traffic Cone Detection for Autonomous Driving

作者：Ankit Dhall, Dengxin Dai, Luc Van Gool

论文链接：https://arxiv.org/abs/1902.02394

项目地址：http://people.ee.ethz.ch/~tracezuerich/TrafficCone/

摘要: Considerable progress has been made in semantic scene understanding of road scenes with monocular cameras. It is, however, mainly related to certain classes such as cars and pedestrians. This work investigates traffic cones, an object class crucial for traffic control in the context of autonomous vehicles. 3D object detection using images from a monocular camera is intrinsically an ill-posed problem. In this work, we leverage the unique structure of traffic cones and propose a pipelined approach to the problem. Specifically, we first detect cones in images by a tailored 2D object detector; then, the spatial arrangement of keypoints on a traffic cone are detected by our deep structural regression network, where the fact that the cross-ratio is projection invariant is leveraged for network regularization; finally, the 3D position of cones is recovered by the classical Perspective n-Point algorithm. Extensive experiments show that our approach can accurately detect traffic cones and estimate their position in the 3D world in real time. The proposed method is also deployed on a real-time, critical system. It runs efficiently on the low-power Jetson TX2, providing accurate 3D position estimates, allowing a race-car to map and drive autonomously on an unseen track indicated by traffic cones. With the help of robust and accurate perception, our race-car won both Formula Student Competitions held in Italy and Germany in 2018, cruising at a top-speed of 54 kmph. Visualization of the complete pipeline, mapping and navigation can be found on our project page.

[3] 讨论CNN中FC必要性的文章

论文题目：Impact of Fully Connected Layers on Performance of Convolutional Neural Networks for Image Classification

作者：S H Shabbeer Basha, Shiv Ram Dubey, Viswanath Pulabaigari, Snehasis Mukherjee

论文链接：https://arxiv.org/abs/1902.02771

代码：https://github.com/shabbeersh/Impact-of-FC-layers

摘要: The Convolutional Neural Networks (CNNs), in domains like computer vision, mostly reduced the need for handcrafted features due to its ability to learn the problem-specific features from the raw input data. However, the selection of dataset-specific CNN architecture, which mostly performed by either experience or expertise is a time-consuming and error-prone process. To automate the process of learning a CNN architecture, this letter attempts at finding the relationship between Fully Connected (FC) layers with some of the characteristics of the datasets. The CNN architectures, and recently data sets also, are categorized as deep, shallow, wide, etc. This letter tries to formalize these terms along with answering the following questions. (i) What is the impact of deeper/shallow architectures on the performance of the CNN w.r.t FC layers?, (ii) How the deeper/wider datasets influence the performance of CNN w.r.t FC layers?, and (iii) Which kind of architecture (deeper/ shallower) is better suitable for which kind of (deeper/ wider) datasets. To address these findings, we have performed experiments with three CNN architectures having different depths. The experiments are conducted by varying the number of FC layers. We used four widely used datasets including CIFAR-10, CIFAR-100, Tiny ImageNet, and CRCHistoPhenotypes to justify our findings in the context of the image classification problem. 

[4] 鱼眼镜头中的人脸检测数据集

论文题目：FDDB-360: Face Detection in 360-degree Fisheye Images

作者：Jianglin Fu, Saeed Ranjbar Alvar, Ivan V. Bajic, Rodney G. Vaughan

论文链接：https://arxiv.org/abs/1902.02777

摘要: 360-degree cameras offer the possibility to cover a large area, for example an entire room, without using multiple distributed vision sensors. However, geometric distortions introduced by their lenses make computer vision problems more challenging. In this paper we address face detection in 360-degree fisheye images. We show how a face detector trained on regular images can be re-trained for this purpose, and we also provide a 360-degree fisheye-like version of the popular FDDB face detection dataset, which we call FDDB-360.


**2019-02-07**

[1] 用对抗样本攻击NMS算法的文章

论文题目：Daedalus: Breaking Non-Maximum Suppression in Object Detection via Adversarial Examples

作者：Derui Wang, Chaoran Li, Sheng Wen, Surya Nepal, Yang Xiang

论文链接：https://arxiv.org/abs/1902.02067

摘要: We demonstrated that Non-Maximum Suppression (NMS), which is commonly used in object detection tasks to filter redundant detection results, is no longer secure. NMS has always been an integral part of object detection algorithms. Currently, Fully Convolutional Network (FCN) is widely used as the backbone architecture of object detection models. Given an input instance, since FCN generates end-to-end detection results in a single stage, it outputs a large number of raw detection boxes. These bounding boxes are then filtered by NMS to make the final detection results. 
In this paper, we propose an adversarial example attack which triggers malfunctioning of NMS in the end-to-end object detection models. Our attack, namely Daedalus, manipulates the detection box regression values to compress the dimensions of detection boxes. Henceforth, NMS will no longer be able to filter redundant detection boxes correctly. And as a result, the final detection output contains extremely dense false positives. This can be fatal for many object detection applications such as autonomous vehicle and smart manufacturing industry. Our attack can be applied to different end-to-end object detection models. Furthermore, we suggest crafting robust adversarial examples by using an ensemble of popular detection models as the substitutes. Considering that model reusing is commonly seen in real-world object detection scenarios, Daedalus examples crafted based on an ensemble of substitutes can launch attacks without knowing the details of the victim models. Our experiments demonstrate that our attack effectively stops NMS from filtering redundant bounding boxes. As the evaluation results suggest, Daedalus increases the false positive rate in detection results to 99.9% and reduces the mean average precision scores to 0, while maintaining a low cost of distortion on the original inputs.

[2] ICRA-19 SLAM文章

论文题目：GEN-SLAM: Generative Modeling for Monocular Simultaneous Localization and Mapping

作者：Punarjay Chakravarty, Praveen Narayanan, Tom Roussel

论文链接：https://arxiv.org/abs/1902.02086

摘要: We present a Deep Learning based system for the twin tasks of localization and obstacle avoidance essential to any mobile robot. Our system learns from conventional geometric SLAM, and outputs, using a single camera, the topological pose of the camera in an environment, and the depth map of obstacles around it. We use a CNN to localize in a topological map, and a conditional VAE to output depth for a camera image, conditional on this topological location estimation. We demonstrate the effectiveness of our monocular localization and depth estimation system on simulated and real datasets.

[3] 数据关联文章

论文题目：CLEAR: A Consistent Lifting, Embedding, and Alignment Rectification Algorithm for Multi-Agent Data Association

作者：Kaveh Fathian, Kasra Khosoussi, Parker Lusk, Yulun Tian, Jonathan P. How

论文链接：https://arxiv.org/abs/1902.02256

摘要: A fundamental challenge in many robotics applications is to correctly synchronize and fuse observations across a team of sensors or agents. Instead of solely relying on pairwise matches among observations, multi-way matching methods leverage the notion of cycle consistency to (i) provide a natural correction mechanism for removing noise and outliers from pairwise matches; (ii) construct an efficient and low-rank representation of the data via merging the redundant observations. To solve this computationally challenging problem, state-of-the-art techniques resort to relaxation and rounding techniques that can potentially result in a solution that violates the cycle consistency principle. Hence, losing the aforementioned benefits. In this work, we present the CLEAR algorithm to address this issue by generating solutions that are, by construction, cycle consistent. Through a novel spectral graph clustering approach, CLEAR fuses the techniques in the multi-way matching and the spectral clustering literature and provides consistent solutions, even in challenging high-noise regimes. Our resulting general framework can provide significant improvement in the accuracy and efficiency of existing distributed multi-agent learning, collaborative SLAM, and multiobject tracking pipelines, which traditionally use pairwise (but potentially inconsistent) correspondences.

**2019-02-06**

[1] 帕累托最优的网络架构搜索文章（code已开源）

论文题目：DVOLVER: Efficient Pareto-Optimal Neural Network Architecture Search

作者：Guillaume Michel, Mohammed Amine Alaoui, Alice Lebois, Amal Feriani, Mehdi Felhi

论文链接：https://arxiv.org/abs/1902.01654

代码链接：https://github.com/guillaume-michel/dvolver

摘要: Automatic search of neural network architectures is a standing research topic. In addition to the fact that it presents a faster alternative to hand-designed architectures, it can improve their efficiency and for instance generate Convolutional Neural Networks (CNN) adapted for mobile devices. In this paper, we present a multi-objective neural architecture search method to find a family of CNN models with the best accuracy and computational resources tradeoffs, in a search space inspired by the state-of-the-art findings in neural search. Our work, called Dvolver, evolves a population of architectures and iteratively improves an approximation of the optimal Pareto front. Applying Dvolver on the model accuracy and on the number of floating points operations as objective functions, we are able to find, in only 2.5 days, a set of competitive mobile models on ImageNet. Amongst these models one architecture has the same Top-1 accuracy on ImageNet as NASNet-A mobile with 8% less floating point operations and another one has a Top-1 accuracy of 75.28% on ImageNet exceeding by 0.28% the best MobileNetV2 model for the same computational resources.

[2] 6D Object Pose Estimation文章

论文题目：6D Object Pose Estimation without PnP

论文链接：https://arxiv.org/abs/1902.01728

摘要: In this paper, we propose an efficient end-to-end algorithm to tackle the problem of estimating the 6D pose of objects from a single RGB image. Our system trains a fully convolutional network to regress the 3D rotation and the 3D translation in region layer. On this basis, a special layer, Collinear Equation Layer, is added next to region layer to output the 2D projections of the 3D bounding boxs corners. In the back propagation stage, the 6D pose network are adjusted according to the error of the 2D projections. In the detection phase, we directly output the position and pose through the region layer. Besides, we introduce a novel and concise representation of 3D rotation to make the regression more precise and easier. Experiments show that our method outperforms base-line and state of the art methods both at accuracy and efficiency. In the LineMod dataset, our algorithm achieves less than 18 ms/object on a GeForce GTX 1080Ti GPU, while the translational error and rotational error are less than 1.67 cm and 2.5 degree.

[3] face detection文章

论文题目：Revisiting a single-stage method for face detection

论文链接：https://arxiv.org/abs/1902.01559

摘要: Although accurate, two-stage face detectors usually require more inference time than single-stage detectors do. This paper proposes a simple yet effective single-stage model for real-time face detection with a prominently high accuracy. We build our single-stage model on the top of the ResNet-101 backbone and analyze some problems with the baseline single-stage detector in order to design several strategies for reducing the false positive rate. The design leverages the context information from the deeper layers in order to increase recall rate while maintaining a low false positive rate. In addition, we reduce the detection time by an improved inference procedure for decoding outputs faster. The inference time of a VGA (640×480) image was only approximately 26 ms with a Titan X GPU. The effectiveness of our proposed method was evaluated on several face detection benchmarks (Wider Face, AFW, Pascal Face, and FDDB). The experiments show that our method achieved competitive results on these popular datasets with a faster runtime than the current best two-stage practices.

[4] 6-DOF Pose Estimation文章

论文题目：SASSE: Scalable and Adaptable 6-DOF Pose Estimation

论文链接：https://arxiv.org/abs/1902.01549

摘要: Visual localization has become a key enabling component of many place recognition and SLAM systems. Contemporary research has primarily focused on improving accuracy and precision-recall type metrics, with relatively little attention paid to a system's absolute storage scaling characteristics, its flexibility to adapt to available computational resources, and its longevity with respect to easily incorporating newly learned or hand-crafted image descriptors. Most significantly, improvement in one of these aspects typically comes at the cost of others: for example, a snapshot-based system that achieves sub-linear storage cost typically provides no metric pose estimation, or, a highly accurate pose estimation technique is often ossified in adapting to recent advances in appearance-invariant features. In this paper, we present a novel 6-DOF localization system that for the first time simultaneously achieves all the three characteristics: significantly sub-linear storage growth, agnosticism to image descriptors, and customizability to available storage and computational resources. The key features of our method are developed based on a novel adaptation of multiple-label learning, together with effective dimensional reduction and learning techniques that enable simple and efficient optimization. We evaluate our system on several large benchmarking datasets and provide detailed comparisons to state-of-the-art systems. The proposed method demonstrates competitive accuracy with existing pose estimation methods while achieving better sub-linear storage scaling, significantly reduced absolute storage requirements, and faster training and deployment speeds.

[5] Vehicle Re-ID文章

论文题目：A Two-Stream Siamese Neural Network for Vehicle Re-Identification by Using Non-Overlapping Cameras

作者：Icaro O. de Oliveira, Keiko V. O. Fonseca, Rodrigo Minetto

论文链接：https://arxiv.org/abs/1902.01496

代码链接：https://github.com/icarofua/siamese-two-stream

摘要: We describe in this paper a novel Two-Stream Siamese Neural Network for vehicle re-identification. The proposed network is fed simultaneously with small coarse patches of the vehicle shape's, with 96 x 96 pixels, in one stream, and fine features extracted from license plate patches, easily readable by humans, with 96 x 48 pixels, in the other one. Then, we combined the strengths of both streams by merging the Siamese distance descriptors with a sequence of fully connected layers, as an attempt to tackle a major problem in the field, false alarms caused by a huge number of car design and models with nearly the same appearance or by similar license plate strings. In our experiments, with 2 hours of videos containing 2982 vehicles, extracted from two low-cost cameras in the same roadway, 546 ft away, we achieved a F-measure and accuracy of 92.6% and 98.7%, respectively. We show that the proposed network, available at this https URL, outperforms other One-Stream architectures, even if they use higher resolution image features.

[6] 

论文题目：TrackNet: Simultaneous Object Detection and Tracking and Its Application in Traffic Video Analysis

作者：Chenge Li, Gregory Dobler, Xin Feng, Yao Wang

论文链接：https://arxiv.org/abs/1902.01466

摘要: Object detection and object tracking are usually treated as two separate processes. Significant progress has been made for object detection in 2D images using deep learning networks. The usual tracking-by-detection pipeline for object tracking requires that the object is successfully detected in the first frame and all subsequent frames, and tracking is done by associating detection results. Performing object detection and object tracking through a single network remains a challenging open question. We propose a novel network structure named trackNet that can directly detect a 3D tube enclosing a moving object in a video segment by extending the faster R-CNN framework. A Tube Proposal Network (TPN) inside the trackNet is proposed to predict the objectness of each candidate tube and location parameters specifying the bounding tube. The proposed framework is applicable for detecting and tracking any object and in this paper, we focus on its application for traffic video analysis. The proposed model is trained and tested on UA-DETRAC, a large traffic video dataset available for multi-vehicle detection and tracking, and obtained very promising results.

**2019-02-05**

[1] ECCV-18 MOT文章

论文题目：Online Multi-Object Tracking with Dual Matching Attention Networks

论文链接：https://arxiv.org/abs/1902.00749

摘要: In this paper, we propose an online Multi-Object Tracking (MOT) approach which integrates the merits of single object tracking and data association methods in a unified framework to handle noisy detections and frequent interactions between targets. Specifically, for applying single object tracking in MOT, we introduce a cost-sensitive tracking loss based on the state-of-the-art visual tracker, which encourages the model to focus on hard negative distractors during online learning. For data association, we propose Dual Matching Attention Networks (DMAN) with both spatial and temporal attention mechanisms. The spatial attention module generates dual attention maps which enable the network to focus on the matching patterns of the input image pair, while the temporal attention module adaptively allocates different levels of attention to different samples in the tracklet to suppress noisy observations. Experimental results on the MOT benchmark datasets show that the proposed algorithm performs favorably against both online and offline trackers in terms of identity-preserving metrics.


[2] 汽车碰撞预测系统

论文题目：Real-time Prediction of Automotive Collision Risk from Monocular Video

论文链接：https://arxiv.org/abs/1902.01293

摘要: Many automotive applications, such as Advanced Driver Assistance Systems (ADAS) for collision avoidance and warnings, require estimating the future automotive risk of a driving scene. We present a low-cost system that predicts the collision risk over an intermediate time horizon from a monocular video source, such as a dashboard-mounted camera. The modular system includes components for object detection, object tracking, and state estimation. We introduce solutions to the object tracking and distance estimation problems. Advanced approaches to the other tasks are used to produce real-time predictions of the automotive risk for the next 10 s at over 5 Hz. The system is designed such that alternative components can be substituted with minimal effort. It is demonstrated on common physical hardware, specifically an off-the-shelf gaming laptop and a webcam. We extend the framework to support absolute speed estimation and more advanced risk estimation techniques.

[3] object detection and 6D pose estimation文章

论文题目：Implicit 3D Orientation Learning for 6D Object Detection from RGB Images

论文链接：https://arxiv.org/abs/1902.01275

代码链接：https://github.com/DLR-RM/AugmentedAutoencoder

摘要: We propose a real-time RGB-based pipeline for object detection and 6D pose estimation. Our novel 3D orientation estimation is based on a variant of the Denoising Autoencoder that is trained on simulated views of a 3D model using Domain Randomization. This so-called Augmented Autoencoder has several advantages over existing methods: It does not require real, pose-annotated training data, generalizes to various test sensors and inherently handles object and view symmetries. Instead of learning an explicit mapping from input images to object poses, it provides an implicit representation of object orientations defined by samples in a latent space. Experiments on the T-LESS and LineMOD datasets show that our method outperforms similar model-based approaches and competes with state-of-the art approaches that require real pose-annotated images.

[4] Crowd Counting文章

论文题目：Dual Path Multi-Scale Fusion Networks with Attention for Crowd Counting

论文链接：https://arxiv.org/abs/1902.01115

摘要: The task of crowd counting in varying density scenes is an extremely difficult challenge due to large scale variations. In this paper, we propose a novel dual path multi-scale fusion network architecture with attention mechanism named SFANet that can perform accurate count estimation as well as present high-resolution density maps for highly congested crowd scenes. The proposed SFANet contains two main components: a VGG backbone convolutional neural network (CNN) as the front-end feature map extractor and a dual path multi-scale fusion networks as the back-end to generate density map. These dual path multi-scale fusion networks have the same structure, one path is responsible for generating attention map by highlighting crowd regions in images, the other path is responsible for fusing multi-scale features as well as attention map to generate the final high-quality high-resolution density maps. SFANet can be easily trained in an end-to-end way by dual path joint training. We have evaluated our method on four crowd counting datasets (ShanghaiTech, UCF CC 50, UCSD and UCF-QRNF). The results demonstrate that with attention mechanism and multi-scale feature fusion, the proposed SFANet achieves the best performance on all these datasets and generates better quality density maps compared with other state-of-the-art approaches.

[5] AAAI-19 Scene Generation with GANs文章

论文题目：A Layer-Based Sequential Framework for Scene Generation with GANs

论文链接：https://arxiv.org/abs/1902.00671

摘要: Visual compatibility is critical for fashion analysis, yet is missing in existing fashion image synthesis systems. In this paper, we propose to explicitly model visual compatibility through fashion image inpainting. To this end, we present Fashion Inpainting Networks (FiNet), a two-stage image-to-image generation framework that is able to perform compatible and diverse inpainting. Disentangling the generation of shape and appearance to ensure photorealistic results, our framework consists of a shape generation network and an appearance generation network. More importantly, for each generation network, we introduce two encoders interacting with one another to learn latent code in a shared compatibility space. The latent representations are jointly optimized with the corresponding generation network to condition the synthesis process, encouraging a diverse set of generated results that are visually compatible with existing fashion garments. In addition, our framework is readily extended to clothing reconstruction and fashion transfer, with impressive results. Extensive experiments with comparisons with state-of-the-art approaches on fashion synthesis task quantitatively and qualitatively demonstrate the effectiveness of our method.

[6] 二值化网络文章

论文题目：Self-Binarizing Networks

论文链接：https://arxiv.org/abs/1902.00730

摘要: We present a method to train self-binarizing neural networks, that is, networks that evolve their weights and activations during training to become binary. To obtain similar binary networks, existing methods rely on the sign activation function. This function, however, has no gradients for non-zero values, which makes standard backpropagation impossible. To circumvent the difficulty of training a network relying on the sign activation function, these methods alternate between floating-point and binary representations of the network during training, which is sub-optimal and inefficient. We approach the binarization task by training on a unique representation involving a smooth activation function, which is iteratively sharpened during training until it becomes a binary representation equivalent to the sign activation function. Additionally, we introduce a new technique to perform binary batch normalization that simplifies the conventional batch normalization by transforming it into a simple comparison operation. This is unlike existing methods, which are forced to the retain the conventional floating-point-based batch normalization. Our binary networks, apart from displaying advantages of lower memory and computation as compared to conventional floating-point and binary networks, also show higher classification accuracy than existing state-of-the-art methods on multiple benchmark datasets.

[7] 商品识别文章

论文题目：Domain invariant hierarchical embedding for grocery products recognition

论文链接：https://arxiv.org/abs/1902.00760

摘要: Recognizing packaged grocery products based solely on appearance is still an open issue for modern computer vision systems due to peculiar challenges. Firstly, the number of different items to be recognized is huge (i.e., in the order of thousands) and rapidly changing over time. Moreover, there exist a significant domain shift between the images that should be recognized at test time, taken in stores by cheap cameras, and those available for training, usually just one or a few studio-quality images per product. We propose an end-to-end architecture comprising a GAN to address the domain shift at training time and a deep CNN trained on the samples generated by the GAN to learn an embedding of product images that enforces a hierarchy between product categories. At test time, we perform recognition by means of K-NN search against a database consisting of just one reference image per product. Experiments addressing recognition of products present in the training datasets as well as different ones unseen at training time show that our approach compares favourably to state-of-the-art methods on the grocery recognition task and generalize fairly well to similar ones.

[8] Dense Depth Completion文章

论文题目：DFuseNet: Deep Fusion of RGB and Sparse Depth Information for Image Guided Dense Depth Completion

论文链接：https://arxiv.org/abs/1902.00761

摘要: In this paper we propose a convolutional neural network that is designed to upsample a series of sparse range measurements based on the contextual cues gleaned from a high resolution intensity image. Our approach draws inspiration from related work on super-resolution and in-painting. We propose a novel architecture that seeks to pull contextual cues separately from the intensity image and the depth features and then fuse them later in the network. We argue that this approach effectively exploits the relationship between the two modalities and produces accurate results while respecting salient image structures. We present experimental results to demonstrate that our approach is comparable with state of the art methods and generalizes well across multiple datasets.

[9] background model estimation 文章

论文题目：DeepPBM: Deep Probabilistic Background Model Estimation from Video Sequences

论文链接：https://arxiv.org/abs/1902.00820

摘要: This paper presents a novel unsupervised probabilistic model estimation of visual background in video sequences using a variational autoencoder framework. Due to the redundant nature of the backgrounds in surveillance videos, visual information of the background can be compressed into a low-dimensional subspace in the encoder part of the variational autoencoder, while the highly variant information of its moving foreground gets filtered throughout its encoding-decoding process. Our deep probabilistic background model (DeepPBM) estimation approach is enabled by the power of deep neural networks in learning compressed representations of video frames and reconstructing them back to the original domain. We evaluated the performance of our DeepPBM in background subtraction on 9 surveillance videos from the background model challenge (BMC2012) dataset, and compared that with a standard subspace learning technique, robust principle component analysis (RPCA), which similarly estimates a deterministic low dimensional representation of the background in videos and is widely used for this application. Our method outperforms RPCA on BMC2012 dataset with 23% in average in F-measure score, emphasizing that background subtraction using the trained model can be done in more than 10 times faster.

[10] 模型压缩文章：MICIK

论文题目：MICIK: MIning Cross-Layer Inherent Similarity Knowledge for Deep Model Compression

论文链接：https://arxiv.org/abs/1902.00918

摘要: State-of-the-art deep model compression methods exploit the low-rank approximation and sparsity pruning to remove redundant parameters from a learned hidden layer. However, they process each hidden layer individually while neglecting the common components across layers, and thus are not able to fully exploit the potential redundancy space for compression. To solve the above problem and enable further compression of a model, removing the cross-layer redundancy and mining the layer-wise inheritance knowledge is necessary. In this paper, we introduce a holistic model compression framework, namely MIning Cross-layer Inherent similarity Knowledge (MICIK), to fully excavate the potential redundancy space. The proposed MICIK framework simultaneously, (1) learns the common and unique weight components across deep neural network layers to increase compression rate; (2) preserves the inherent similarity knowledge of nearby layers and distant layers to minimize the accuracy loss and (3) can be complementary to other existing compression techniques such as knowledge distillation. Extensive experiments on large-scale convolutional neural networks demonstrate that MICIK is superior over state-of-the-art model compression approaches with 16X parameter reduction on VGG-16 and 6X on GoogLeNet, all without accuracy loss.

[11] Depthwise Convolution is All You Need

论文题目：Depthwise Convolution is All You Need for Learning Multiple Visual Domains

论文链接：https://arxiv.org/abs/1902.00927

摘要: There is a growing interest in designing models that can deal with images from different visual domains. If there exists a universal structure in different visual domains that can be captured via a common parameterization, then we can use a single model for all domains rather than one model per domain. A model aware of the relationships between different domains can also be trained to work on new domains with less resources. However, to identify the reusable structure in a model is not easy. In this paper, we propose a multi-domain learning architecture based on depthwise separable convolution. The proposed approach is based on the assumption that images from different domains share cross-channel correlations but have domain-specific spatial correlations. The proposed model is compact and has minimal overhead when being applied to new domains. Additionally, we introduce a gating mechanism to promote soft sharing between different domains. We evaluate our approach on Visual Decathlon Challenge, a benchmark for testing the ability of multi-domain models. The experiments show that our approach can achieve the highest score while only requiring 50% of the parameters compared with the state-of-the-art approaches.

[12] 表情识别文章

论文题目：Deep-Emotion: Facial Expression Recognition Using Attentional Convolutional Network

论文链接：https://arxiv.org/abs/1902.01019

摘要: Facial expression recognition has been an active research area over the past few decades, and it is still challenging due to the high intra-class variation. 
Traditional approaches for this problem rely on hand-crafted features such as SIFT, HOG and LBP, followed by a classifier trained on a database of images or videos. 
Most of these works perform reasonably well on datasets of images captured in a controlled condition, but fail to perform as good on more challenging datasets with more image variation and partial faces. 
In recent years, several works proposed an end-to-end framework for facial expression recognition, using deep learning models. 
Despite the better performance of these works, there still seems to be a great room for improvement. 
In this work, we propose a deep learning approach based on attentional convolutional network, which is able to focus on important parts of the face, and achieves significant improvement over previous models on multiple datasets, including FER-2013, CK+, FERG, and JAFFE. 
We also use a visualization technique which is able to find important face regions for detecting different emotions, based on the classifier's output. 
Through experimental results, we show that different emotions seems to be sensitive to different parts of the face.

[13] ECCV-18行人检测比赛参赛方案

论文题目：Towards Pedestrian Detection Using RetinaNet in ECCV 2018 Wider Pedestrian Detection Challenge

论文链接：https://arxiv.org/abs/1902.01031

代码链接：https://github.com/miltonbd/ECCV_2018_pedestrian_detection_challenege

摘要: The main essence of this paper is to investigate the performance of RetinaNet based object detectors on pedestrian detection. Pedestrian detection is an important research topic as it provides a baseline for general object detection and has a great number of practical applications like autonomous car, robotics and Security camera. Though extensive research has made huge progress in pedestrian detection, there are still many issues and open for more research and improvement. Recent deep learning based methods have shown state-of-the-art performance in computer vision tasks such as image classification, object detection, and segmentation. Wider pedestrian detection challenge aims at finding improve solutions for pedestrian detection problem. In this paper, We propose a pedestrian detection system based on RetinaNet. Our solution has scored 0.4061 mAP.

[14] 单目标跟踪文章FF-Siam

论文题目：End-to-end feature fusion siamese network for adaptive visual tracking

论文链接：https://arxiv.org/abs/1902.01057

摘要: According to observations, different visual objects have different salient features in different scenarios. Even for the same object, its salient shape and appearance features may change greatly from time to time in a long-term tracking task. Motivated by them, we proposed an end-to-end feature fusion framework based on Siamese network, named FF-Siam, which can effectively fuse different features for adaptive visual tracking. The framework consists of four layers. A feature extraction layer is designed to extract the different features of the target region and search region. The extracted features are then put into a weight generation layer to obtain the channel weights, which indicate the importance of different feature channels. Both features and the channel weights are utilized in a template generation layer to generate a discriminative template. Finally, the corresponding response maps created by the convolution of the search region features and the template are applied with a fusion layer to obtain the final response map for locating the target. Experimental results demonstrate that the proposed framework achieves state-of-the-art performance on the popular Temple-Color, OTB50 and UAV123 benchmarks.


[15] SfM文章

论文题目：Jumping Manifolds: Geometry Aware Dense Non-Rigid Structure from Motion

论文链接：https://arxiv.org/abs/1902.01077

摘要: Given dense image feature correspondences of a non-rigidly moving object across multiple frames, this paper proposes an algorithm to estimate its 3D shape for each frame. To solve this problem accurately, the recent state-of-the-art algorithm reduces this task to set of local linear subspace reconstruction and clustering problem using Grassmann manifold representation \cite{kumar2018scalable}. Unfortunately, their method missed on some of the critical issues associated with the modeling of surface deformations, for e.g., the dependence of a local surface deformation on its neighbors. Furthermore, their representation to group high dimensional data points inevitably introduce the drawbacks of categorizing samples on the high-dimensional Grassmann manifold \cite{huang2015projection, harandi2014manifold}. Hence, to deal with such limitations with \cite{kumar2018scalable}, we propose an algorithm that jointly exploits the benefit of high-dimensional Grassmann manifold to perform reconstruction, and its equivalent lower-dimensional representation to infer suitable clusters. To accomplish this, we project each Grassmannians onto a lower-dimensional Grassmann manifold which preserves and respects the deformation of the structure w.r.t its neighbors. These Grassmann points in the lower-dimension then act as a representative for the selection of high-dimensional Grassmann samples to perform each local reconstruction. In practice, our algorithm provides a geometrically efficient way to solve dense NRSfM by switching between manifolds based on its benefit and usage. Experimental results show that the proposed algorithm is very effective in handling noise with reconstruction accuracy as good as or better than the competing methods.

[16] 去雾文章

论文题目：End-to-End Single Image Fog Removal using Enhanced Cycle Consistent Adversarial Networks

论文链接：https://arxiv.org/abs/1902.01374

摘要: Single image defogging is a classical and challenging problem in computer vision. Existing methods towards this problem mainly include handcrafted priors based methods that rely on the use of the atmospheric degradation model and learning based approaches that require paired fog-fogfree training example images. In practice, however, prior-based methods are prone to failure due to their own limitations and paired training data are extremely difficult to acquire. Inspired by the principle of CycleGAN network, we have developed an end-to-end learning system that uses unpaired fog and fogfree training images, adversarial discriminators and cycle consistency losses to automatically construct a fog removal system. Similar to CycleGAN, our system has two transformation paths; one maps fog images to a fogfree image domain and the other maps fogfree images to a fog image domain. Instead of one stage mapping, our system uses a two stage mapping strategy in each transformation path to enhance the effectiveness of fog removal. Furthermore, we make explicit use of prior knowledge in the networks by embedding the atmospheric degradation principle and a sky prior for mapping fogfree images to the fog images domain. In addition, we also contribute the first real world nature fog-fogfree image dataset for defogging research. Our multiple real fog images dataset (MRFID) contains images of 200 natural outdoor scenes. For each scene, there are one clear image and corresponding four foggy images of different fog densities manually selected from a sequence of images taken by a fixed camera over the course of one year. Qualitative and quantitative comparison against several state-of-the-art methods on both synthetic and real world images demonstrate that our approach is effective and performs favorably for recovering a clear image from a foggy image.

[17] 3D点云文章

论文题目：3D point cloud registration with shape constraint

论文链接：https://arxiv.org/abs/1902.01061

摘要: In this paper, a shape-constrained iterative algorithm is proposed to register a rigid template point-cloud to a given reference point-cloud. The algorithm embeds a shape-based similarity constraint into the principle of gravitation. The shape-constrained gravitation, as induced by the reference, controls the movement of the template such that at each iteration, the template better aligns with the reference in terms of shape. This constraint enables the alignment in difficult conditions indtroduced by change (presence of outliers and/or missing parts), translation, rotation and scaling. We discuss efficient implementation techniques with least manual intervention. The registration is shown to be useful for change detection in the 3D point-cloud. The algorithm is compared with three state-of-the-art registration approaches. The experiments are done on both synthetic and real-world data. The proposed algorithm is shown to perform better in the presence of big rotation, structured and unstructured outliers and missing data.

**2019-02-04**

[1] ACM Multimedia 2018 图像检索oral文章

论文题目：Deep Triplet Quantization

论文链接：https://arxiv.org/abs/1902.00153

摘要: Deep hashing establishes efficient and effective image retrieval by end-to-end learning of deep representations and hash codes from similarity data. We present a compact coding solution, focusing on deep learning to quantization approach that has shown superior performance over hashing solutions for similarity retrieval. We propose Deep Triplet Quantization (DTQ), a novel approach to learning deep quantization models from the similarity triplets. To enable more effective triplet training, we design a new triplet selection approach, Group Hard, that randomly selects hard triplets in each image group. To generate compact binary codes, we further apply a triplet quantization with weak orthogonality during triplet training. The quantization loss reduces the codebook redundancy and enhances the quantizability of deep representations through back-propagation. Extensive experiments demonstrate that DTQ can generate high-quality and compact binary codes, which yields state-of-the-art image retrieval performance on three benchmark datasets, NUS-WIDE, CIFAR-10, and MS-COCO.

[2] ICLR compressed NAS文章

论文题目：Learnable Embedding Space for Efficient Neural Architecture Compression

论文链接：https://arxiv.org/abs/1902.00383

摘要: We propose a method to incrementally learn an embedding space over the domain of network architectures, to enable the careful selection of architectures for evaluation during compressed architecture search. Given a teacher network, we search for a compressed network architecture by using Bayesian Optimization (BO) with a kernel function defined over our proposed embedding space to select architectures for evaluation. We demonstrate that our search algorithm can significantly outperform various baseline methods, such as random search and reinforcement learning (Ashok et al., 2018). The compressed architectures found by our method are also better than the state-of-the-art manually-designed compact architecture ShuffleNet (Zhang et al., 2018). We also demonstrate that the learned embedding space can be transferred to new settings for architecture search, such as a larger teacher network or a teacher network in a different architecture family, without any training.

[3] ciFAIR数据集（无重复样本的CIFAR）

论文题目：Do we train on test data? Purging CIFAR of near-duplicates

论文链接：https://arxiv.org/abs/1902.00423

代码链接：https://cvjena.github.io/cifair/

摘要: We find that 3.3% and 10% of the images from the CIFAR-10 and CIFAR-100 test sets, respectively, have duplicates in the training set. This may incur a bias on the comparison of image recognition techniques with respect to their generalization capability on these heavily benchmarked datasets. To eliminate this bias, we provide the "fair CIFAR" (ciFAIR) dataset, where we replaced all duplicates in the test sets with new images sampled from the same domain. The training set remains unchanged, in order not to invalidate pre-trained models. We then re-evaluate the classification performance of various popular state-of-the-art CNN architectures on these new test sets to investigate whether recent research has overfitted to memorizing data instead of learning abstract concepts. Fortunately, this does not seem to be the case yet. The ciFAIR dataset and pre-trained models are available at this https URL, where we also maintain a leaderboard.

[4] 行人轨迹数据集

论文题目：Top-view Trajectories: A Pedestrian Dataset of Vehicle-Crowd Interaction from Controlled Experiments and Crowded Campus

论文链接：https://arxiv.org/abs/1902.00487

摘要: Predicting the collective motion of a group of pedestrians (a crowd) under the vehicle influence is essential for the development of autonomous vehicles to deal with mixed urban scenarios where interpersonal interaction and vehicle-crowd interaction (VCI) are significant. This usually requires a model that can describe individual pedestrian motion under the influence of nearby pedestrians and the vehicle. This study proposed two pedestrian trajectory dataset, CITR dataset and DUT dataset, so that the pedestrian motion models can be further calibrated and verified, especially when vehicle influence on pedestrians plays an important role. CITR dataset consists of experimentally designed fundamental VCI scenarios (front, back, and lateral VCIs) and provides unique ID for each pedestrian, which is suitable for exploring a specific aspect of VCI. DUT dataset gives two ordinary and natural VCI scenarios in crowded university campus, which can be used for more general purpose VCI exploration. The trajectories of pedestrians, as well as vehicles, were extracted by processing video frames that come from a down-facing camera mounted on a hovering drone as the recording equipment. The final trajectories were refined by a Kalman Filter, in which the pedestrian velocity was also estimated. The statistics of the velocity magnitude distribution demonstrated the validity of the proposed dataset. In total, there are approximate 340 pedestrian trajectories in CITR dataset and 1793 pedestrian trajectories in DUT dataset. The dataset is available at GitHub.










