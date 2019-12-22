## 一、 选题名称

**中文题名**：YOLOv3在车辆检测的应用  
**英文题名**：Application of YOLOv3 in vehicle detection

## 二、选题思路

### 1、选题背景
目前计算机视觉领域的目标检测方案分为两派：网格类检测、区域类检测，而2016年的YOLO(v1)可谓是网格类检测的开山鼻祖，凭速度之优势摘下当时实时检测的桂冠，但在精度方面存在局限。为解决准确率低的短板，2016年底YOLO合并coco训练集，推出YOLOv2；再增加输出类别，推出YOLO9000。再至2018年，YOLOv3进击而来，不论是小物体识别、紧凑密集和高度重叠的检测、模型的泛化能力、速度、准确度，都可谓是网格类检测目标检测的巅峰之作。最新版本的YOLOv3的算法速度相当出色，非常适合用于计算机视觉的实时目标检测、目标追踪，譬如工业影像检测、智能驾驶的行人检测与车辆检测等应用场景；一经发布就使业界每每惊艳、一致赞叹强推，并由此产出数量可观的期刊论文与成果，是当下相当值得进行研究的目标检测领域热点。

### 2、选题调整情况
#### 选题原因1：
大三第一学期，从刘晓翔老师了解到一项YOLOv3应用相关的课题。YOLOv3是YOLO系列算法的最新发布版本，我希望通过文献检索与利用这门课，更深入地了解YOLOv3的技术背景、整体的发布历程和应用前景，准备以“YOLO系列算法的应用”为选题。
#### 选题调整过程1：
2016年5月，YOLO(YOLO系列的v1版)发表论文《You Only Look Once: Unified, Real-Time Object Detection》，可谓是用回归做物体检测的开山力作。自2016年至今，YOLO系列已发生了两次速度精度上的更迭：2016年底的YOLOv2与YOLO9000，2018年4月的YOLOv3。
CNKI测试：[SU='YOLO' AND YE BETWEEN ('2016','2020')，返回201条期刊论文，返回20条会议论文]。WoS测试：[TS=("YOLO") AND PY=(2016-2020)，精炼依据: 研究领域: ( SCIENCE TECHNOLOGY )，返回460条结果]。经过这次选题初步检索发现，YOLO系列每次更新发布之后都紧接着大量基于YOLO的各版本的应用和期刊论文，发展快，产出多，期刊论文数量多，需要作出限制。
#### 选题原因2：
YOLO系列在物体检测相关的应用范围广，譬如工业影像检测、行人检测等，其中YOLOv3在智能驾驶领域的车辆检测方面精度与速度齐飞，效果相当出色。第一方面，理工类研究重视时效指标，另一方面为了本课程能有效正反馈于本学期的项目，所以确定选题为“YOLOv3在车辆检测的应用”。
#### 选题调整过程2：
CNKI测试：[SU=('车辆检测'+'车辆识别'+'车辆目标检测'+'车辆目标识别')*('YOLOv3'+'YOLO') ，返回25条期刊论文结果]。WoS测试：[TS=("YOLOv3" OR "YOLO v3") AND TS=("vehicle detection" OR "detecting vehicle" OR "car detection" OR "detecting cars")，返回18条结果]。从应用领域进行限制，由模糊不做限制应用领域调整到车辆检测这一应用领域，通过CNKI测试与WoS测试得到的检索结果数量合适，选题范围合适，所以最终确定研究课题为“YOLOv3在车辆检测的应用” ，可以继续检索相关文献，学术论文、学位论文、会议文献等进行进一步研究。

### 3、综述检索与阅读情况
#### （1）、综述检索过程
以YOLO、YOLOv3、车辆检测、车辆识别、车辆目标检测、车辆目标识别等为中文检索词，查找国内综述；以YOLO、YOLOv3、vehicle detection, car detection, detecting vehicle, detecting cars等为英文检索词，查找国外综述，进一步了解“YOLOv3在车辆检测的应用”的理论体系。

**CNKI方法**：SU=('车辆检测' + '车辆识别' + '车辆目标检测' + '车辆目标识别')*'YOLO' and TI='述评'+'综述'+'现状'+'展望'+'概况'+'进展'，返回1条结果。  
1.	卞山峰,张庆辉.车辆实时检测研究综述[J].电子质量,2019(02):4-8. 

**WOS方法1**：TS=("YOLO" OR "YOLOv3") AND TS=("vehicle detection" OR "detecting vehicle" OR "car detection" OR "detecting cars")，返回39条结果，但含有文献类型为REVIEW数目为0条。所以将检索范围稍作调整，将车辆检测范围扩大至检测范围，有以下WOS方法2。 

**WOS方法2**：TS=("YOLO" OR "YOLOv3") AND TS=("detection" OR "detecting")，返回501条结果，限定文献类型: REVIEW，返回3条综述结果。    
1.	Koirala A, Walsh K B, Wang Z, et al. Deep learning–Method overview and review of use for fruit detection and yield estimation[J]. Computers and Electronics in Agriculture, 2019, 162: 219-234.  
2.	Yao Qunli, Hu Xian, Lei Hong. Application of deep convolutional neural network in object detection [J]. Computer Engineering and Application, 2018 (17): 1.  
3.	Wu Shuai, Xu Yong, Zhao Dongning. Survey of Object Detection Based on Deep Convolutional Network [J]. Pattern Recognition and Artificial Intelligence, 2018, 31(4): 335-346.  

#### （2）、综述阅读笔记（300汉字以内）
阅读《车辆实时检测研究综述》全文，了解到近年来车辆实时检测领域的应用算法的递进发展过程：

传统车辆实时检测方法通常采用滑动窗口的提取方法，主要使用光流法、帧差法、背景差分法、匹配法的识别方法；然而滑动窗口的特征制作困难，以上识别方法在噪声、光源、对象的运动速度、背景场景等制约下的输出效果不佳。随着深度学习的在车辆实时检测领域的发展应用，卷积神经网络成为较好的检测方案，车辆实时检测算法从RCNN、FastRCNN、FasterRCNN，发展到基于CNN的YOLOv2实现，检测速度和精度大幅提升，实验测试条件下速度达到实时性的要求，但其准确性仍存在局限性：譬如，在遮挡、光照和车辆形态变换等因素的影响下常常不能达到很好的检测效果。在YOLOv3算法研究火热的当下，有望将YOLOv3与其他算法优势互补结合，使车辆实时检测技术往更智能、更实用的方向发展。

## 三、检索词（中英文）
**中文检索词1**：YOLOv3、YOLO  
**英文检索词1**：YOLOv3、YOLO  
**中文检索词2**：车辆检测，车辆识别，车辆目标检测，车辆目标识别  
**英文检索词2**：vehicle detection, car detection, detecting vehicle, detecting cars

## 四、围绕课题需求，开展信息检索
### （1）、中文图书检索
**备注**：由于选题YOLO算法的优质开源特性，具有很高的更迭效率和应用频度，不支持稳定成稿出版，通过检索语句[WRD = YOLOv3 AND (车辆检测 OR 车辆识别 OR 车辆目标检测 OR 车辆目标识别)，返回0条记录]；因此对此步的中文图书检索，调整为选择其上层课题：目标追踪、目标检测而进行检索。  
**数据库1**：中国国家图书馆联机公共目录查询系统  
**检索语句**： WRD = ( 目标追踪 OR 目标检测 ) 限定资料类型为图书，限定2016-?（至今）  
**检索记录数**：5  
**主要相关文献（1-3条题录）**：  
[1]	焦建彬.视觉目标检测与跟踪[M].北京:科学出版社,2016.  
[2]	(波)Boguslaw Cyganek著.数字图像目标检测与识别:理论与实践[M].宋晓炜,杨蕾,瞿博阳译. 北京:电子工业出版社,2016.  
[3]	陈哲,王慧斌.图像目标检测技术及应用[M].北京:人民邮电出版社, 2016.

### （2）、外文图书检索
**数据库1**：Google Books  
**检索语句**：(YOLOv3) AND ((vehicle detection) OR (car detection) OR (detecting vehicle) OR (detecting cars))  
**检索记录数**：12  
**主要相关文献（1-3条题录）**：  
[1]	Bebis G. Advances in Visual Computing: 14th International Symposium on Visual Computing, ISVC 2019, Lake Tahoe, NV, USA, October 7–9, 2019, Proceedings, Part I[M]. Springer Nature, 2019  
[2]	JH Lai, CL Liu, X Chen, J Zhou, T Tan, N Zheng, H Zha. Pattern Recognition and Computer Vision: First Chinese Conference, PRCV 2018, Guangzhou, China, November 23-26, 2018, Proceedings[M]. Springer, 2018.  
[3]	Y Wang, Q Huang, Y Peng. Image and Graphics Technologies and Applications: 14th Conference on Image and Graphics Technologies and Applications, IGTA 2019, Beijing, China, April 19–20, 2019, Revised Selected Papers[M]. Springer, 2019. 

### （3）、中文期刊论文检索
**数据库1**：CNKI中国知网：期刊数据库  
**检索语句**：SU=('车辆检测'+'车辆识别'+'车辆目标检测'+'车辆目标识别')*('YOLOv3'+'YOLO')  
**检索记录数**：25  
**主要相关文献（1-3条题录）**：  
[1]	王宇宁,庞智恒,袁德明.基于YOLO算法的车辆实时检测[J].武汉理工大学学报,2016,38(10):41-46.  
[2]	张富凯,杨峰,李策.基于改进YOLOv3的快速车辆检测方法[J].计算机工程与应用,2019,55(02):12-20.  
[3]	刘军,后士浩,张凯,张睿,胡超超.基于增强Tiny YOLOV3算法的车辆实时检测与跟踪[J].农业工程学报,2019,35(08):118-125.

### （4）、外文期刊论文检索
**数据库1**：Science Citation Index Expanded (SCI-EXPANDED)  
**检索语句**：TS=("YOLOv3" OR "YOLO v3") AND TS=("vehicle detection" OR "car detection" OR "detecting vehicle" OR "detecting cars")  
**检索记录数**：10  
**主要相关文献（1-3条题录）**：  
[1]	Kim K J, Kim P K, Chung Y S, et al. Multi-Scale Detector for Accurate Vehicle Detection in Traffic Surveillance Data[J]. IEEE Access, 2019, 7: 78311-78319.  
[2]	Wang H, Yu Y, Cai Y, et al. A Comparative Study of State-of-the-Art Deep Learning Algorithms for Vehicle Detection[J]. IEEE Intelligent Transportation Systems Magazine, 2019, 11(2): 82-95.  
[3]	Han G, Su J, Zhang C. A method based on Multi-Convolution layers Joint and Generative Adversarial Networks for Vehicle Detection[J]. KSII Transactions on Internet & Information Systems, 2019, 13(4).

**数据库2**：EI (Engineering Village2)  
**检索语句**：((("YOLOv3" OR "YOLO v3") AND ("vehicle detection" OR "car detection" OR "detecting vehicle" OR "detecting cars")))  
**检索记录数**：21  
**主要相关文献（1-3条题录）**：  
[1]	Liu Jun, Hou Shihao, Zhang Kai, et al. Real-time vehicle detection and tracking based on enhanced Tiny YOLOV3 algorithm[J]. Nongye Gongcheng Xuebao/Transactions of the Chinese Society of Agricultural Engineering, v 35, n 8, p 118-125, 2019  
[2]	Li X, Liu Y, Zhao Z, et al. A Deep Learning Approach of Vehicle Multitarget Detection from Traffic Video[J]. Journal of Advanced Transportation, 2018, 2018.

**数据库3**：IEEE/IET Electronic Library  
**检索语句**：((YOLOv3) OR (YOLO v3)) AND ((vehicle detection) OR (car detection) OR (detecting vehicle) OR (detecting cars))  
**检索记录数**：46  
**主要相关文献（1-3条题录）**：  
[1]	Benjdira B, Khursheed T, Koubaa A, et al. Car detection using unmanned aerial vehicles: Comparison between faster r-cnn and yolov3[C]//2019 1st International Conference on Unmanned Vehicle Systems-Oman (UVS). IEEE, 2019: 1-6.  
[2]	Du L, Chen W, Fu S, et al. Real-time Detection of Vehicle and Traffic Light for Intelligent and Connected Vehicles Based on YOLOv3 Network[C]//2019 5th International Conference on Transportation Information and Safety (ICTIS). IEEE, 2019: 388-392.  
[3]	Zhang X, Zhu X. Vehicle Detection in the Aerial Infrared Images via an Improved Yolov3 Network[C]//2019 IEEE 4th International Conference on Signal and Image Processing (ICSIP). IEEE, 2019: 372-376.

### （5）、中文学位论文检索
**数据库1**：CNKI中国知网：博硕士论文数据库  
**检索语句**：SU=('车辆检测'+'车辆识别'+'车辆目标检测'+'车辆目标识别')*('YOLOv3'+'YOLO')  
**检索记录数**：36  
**主要相关文献（1-3条题录）**：  
[1]	唐诗. 基于车载视频的道路车辆及行人检测[D].电子科技大学,2018.  
[2]	张雲轲. 基于深度学习的车辆检测算法研究及系统实现[D].电子科技大学,2018.  
[3]	张建. 基于无人机图像的车辆目标识别方法研究与实现[D].电子科技大学,2019.

### （6）、外文学位论文检索
**数据库1**：ProQuest学位论文全文库  
**检索语句**：(YOLO) AND (vehicle OR car OR traffic)  
**检索记录数**：40  
**主要相关文献（1-3条题录）**：  
[1]	Chiddarwar A. Application Of Computer Vision Algorithms For Uninterrupted Traffic Monitoring Based On Aerial Images And Videos[D]. University of Cincinnati, 2019.  
[2]	Li Y. Study of Identifying Jaywalkers by Analyzing Camera Data[D]. Purdue University, 2018.  
[3]	Weill E. Edge-Computing Deep Learning-Based Computer Vision Systems[D]. Clemson University, 2018.

**数据库2**：DDS学位论文集成发现系统  
**检索语句**：(YOLO) AND (detection)  
**检索记录数**：8  
主要相关文献（1-3条题录）：  
[1]	Siddharth Kumar. Robust Lightweight Object Detection[D]. San Jose State University, 2019

## 五、分析检索结果，筛选核心资源
### （1）、本课题的中文、英文重要期刊

|期刊名称  |  ISSN号  |  是否A类  |  最新影响因子|
| ---------- | :-----------:  | :-----------:  | :-----------: |
|激光与光电子学进展  |  1006-4125  |  B  |  复合IF：1.685  综合IF：1.395|
|交通运输工程学报  |  1671-1637  |  B  |  复合IF：1.930  综合IF：1.134|
|IEEE ACCESS  |  2169-3536  |  A1  |  2018IF：4.098|
|SENSORS  |  1424-8220  |  A2  |  2018IF：3.031|

### （2）、列出本课题的国内、国外核心著者和机构
|主要著者  |  机构单位|
| ---------- | :-----------:  |
|王宇宁  |  武汉理工大学|
|李珣  |  西安工程大学电子信息学院|
|Kwang-Ju Kim  |  Electronics and Telecommunications Research Institute, Daegu, South Korea|
|PyongKun Kim  |  Electronics and Telecommunication Research Institute Dalseong-gun Daegu, Korea|

### （3）、核心资源引文检索过程
**被引著者、被引文献（1条题录）**：王宇宁,庞智恒,袁德明.基于YOLO算法的车辆实时检测[J].武汉理工大学学报,2016,38(10):41-46.  
**数据库名称**：CNKI  
**检索式**：RF=基于YOLO算法的车辆实时检测  
**引用著者、引用文献（1条题录）**：龚静,曹立,亓琳,李良荣.基于YOLOv2算法的运动车辆目标检测方法研究[J].电子科技,2018,31(06):5-8+12.

### （4）、核心资源参考文献回溯过程
**文献原文（1条题录）**：Kim K J, Kim P K, Chung Y S, et al. Multi-Scale Detector for Accurate Vehicle Detection in Traffic Surveillance Data[J]. IEEE Access, 2019, 7: 78311-78319.  
**参考文献（1条题录）**：Bottou L. Large-scale machine learning with stochastic gradient descent[M]//Proceedings of COMPSTAT'2010. Physica-Verlag HD, 2010: 177-186.

### （5）、列出本课题重要网络资源（如研究机构、专业论坛等学术网站，1-3个网站）：
1.	[GitHub平台的yolov3相关项目](https://github.com/search?q=yolov3)  
2.	[MXNet/Gluon论坛（目标检测模型：YOLO 讨论区）](https://discuss.gluon.ai/t/topic/6279)

## 六、根据检索结果，进行信息研究，撰写综述（500汉字以上）
### 一、国内外已有哪些相关研究以及研究水平
在基于区域的CNN提出后，DNN开始在目标检测领域普及，FasterCNN将整个目标检测过程合成在一个统一的深度网络框架上，随后YOLO等目标检测框架的提出使目标检测效率得到提升。YOLO系列目标检测算法框架将目标检测任务归结为目标区域预测和类预测的回归问题，将包围盒回归和目标类预测整合到单个卷积神经网络中，实现了准确率较高情况下的快速目标检测，非常适合实时检测场景<sup>[1]</sup>。

在One-stage性能测试下，YOLO算法网络结构简单、检测速度快，适用于快速目标检测；YOLOv2算法通过多尺度训练，进一步提升检测精度，适用于快速目标检测；YOLOv3算法利用深度残差网络提取图像特征<sup>[2]</sup>，引入多尺度特征结构，改善检测精度，适用于多尺度目标检测<sup>[3][4]</sup>，但由于最小特征图尺寸偏大<sup>[2]</sup>，对中等或较大尺寸的物体检测效果不好, 会产生误检、漏检或重复检测的问题<sup>[5][6]</sup>。目前也有项目提出YOLOv3改进模型，譬如DF-YOLOv3<sup>[2]</sup>（深度残差网络提取车辆特征、多尺度网络预测车辆、锚点机制预测车辆边界框、深度网络训练），实验得到更高的均值平均精度 (mAP)；对YOLOv3增进遮挡的空间金字塔池方法的多尺度车辆检测<sup>[7]</sup>；根据目标场景和交通流变化的需要适用于行进道路的YOLO-vocRV结构<sup>[8]</sup>。
### 二、目前的研究中尚有哪些问题有待解决
#### 问题1
车辆跟踪算法通常利用初始化的车辆位置估计车辆状态或者建立表观模型预测在连续视频帧中该车辆出现的位置, 降低了每帧车辆检测的耗时, 而面对复杂多变的交通环境, 如车辆的快速移动、光照变化、道路环境干扰以及车辆在不同距离时的尺度变化等, 使得车辆跟踪发生目标“掉帧”<sup>[9]</sup>，算法的鲁棒性面临挑战<sup>[10]</sup>。
#### 问题2
深度网络模型消耗大量存储空间，限制了在移动端应用<sup>[1]</sup>；车辆检测算法的复杂性往往需要利用昂贵的计算资源才可以实现实时检测<sup>[6]</sup>；这些问题使其在嵌入式实现时困难重重,难以到达车辆检测任务的实时性要求,且过高的硬件实现成本使其难以在短时间内在车辆检测领域达到应用级要求<sup>[11]</sup>。压缩目标检测模型，提高检测效率<sup>[1]</sup>，是目前在车辆目标检测乃至整个深度学习领域都亟待解决的难点。
### 三、国内外研究的动向和主攻点
#### （1）算法联调融合
基于候选窗口的目标检测算法通常检测准确率较高，而基于回归窗口的目标检测方法在检测效率上结果较好，目前也有方法试图在这两类之间建立联系，譬如RON网络就试图利用RPN 建立目标先验以提升回归模型的检测效率<sup>[1]</sup>。
#### （2）多层网络特征融合结构
目标检测是进行场景内容理解等高级视觉任务的前提，静态图像的目标检测存在诸多难点，如物体形变、物体遮挡及小目标检测等<sup>[12]</sup>。为解决这些问题，将基于功能性子网络的目标检测研究<sup>[1]</sup>上针对物体形变、遮挡等难点的有效目标检测方法引入深度网络，增加深度网络处理这些特殊问题的能力，提升目标检测性能。
#### （3）与图像分割技术的结合
一些研究者已经开始将图像分割与对象检测相结合，例如Mask R-CNN结合了检测和实例分割训练方法来提高分割和检测的准确性，从而实现像素级检测<sup>[8]</sup>。

## 参考文献
[1]	Wu Shuai, Xu Yong, Zhao Dongning. Survey of Object Detection Based on Deep Convolutional Network [J]. Pattern Recognition and Artificial Intelligence, 2018, 31(4):  
[2]	张富凯,杨峰,李策.基于改进YOLOv3的快速车辆检测方法[J].计算机工程与应用,2019,55(02):12-20.  
[3]	Du L, Chen W, Fu S, et al. Real-time Detection of Vehicle and Traffic Light for Intelligent and Connected Vehicles Based on YOLOv3 Network[C]//2019 5th International Conference on Transportation Information and Safety (ICTIS). IEEE, 2019: 388-392.  
[4]	Benjdira B, Khursheed T, Koubaa A, et al. Car detection using unmanned aerial vehicles: Comparison between faster r-cnn and yolov3[C]//2019 1st International Conference on Unmanned Vehicle Systems-Oman (UVS). IEEE, 2019: 1-6.  
[5]	Yao Qunli, Hu Xian, Lei Hong. Application of deep convolutional neural network in object detection [J]. Computer Engineering and Application, 2018 (17): 1.  
[6]	王宇宁,庞智恒,袁德明.基于YOLO算法的车辆实时检测[J].武汉理工大学学报,2016,38(10):41-46.  
[7]	Kim K J, Kim P K, Chung Y S, et al. Multi-Scale Detector for Accurate Vehicle Detection in Traffic Surveillance Data[J]. IEEE Access, 2019, 7: 78311-78319.  
[8]	Li X, Liu Y, Zhao Z, et al. A Deep Learning Approach of Vehicle Multitarget Detection from Traffic Video[J]. Journal of Advanced Transportation, 2018, 2018.  
[9]	唐诗. 基于车载视频的道路车辆及行人检测[D].电子科技大学,2018.  
[10]	刘军,后士浩,张凯,张睿,胡超超.基于增强Tiny YOLOV3算法的车辆实时检测与跟踪[J].农业工程学报,2019,35(08):118-125.   
[11]	张雲轲. 基于深度学习的车辆检测算法研究及系统实现[D].电子科技大学,2018.  
[12]	卞山峰,张庆辉.车辆实时检测研究综述[J].电子质量,2019(02):4-8.  
[13]	Wang H, Yu Y, Cai Y, et al. A Comparative Study of State-of-the-Art Deep Learning Algorithms for Vehicle Detection[J]. IEEE Intelligent Transportation Systems Magazine, 2019, 11(2): 82-95.
