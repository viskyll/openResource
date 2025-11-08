
# 目标识别与位姿估计

- [目标识别(Target Regnition)](#目标识别target-regnition)
  - [多模态视觉融合(Multimodal visual fusion)](#多模态视觉融合multimodal-visual-fusion)
  - [目标检测与分割(Object Detection and Segmentation)](#目标检测与分割object-detection-and-segmentation)
  - [迁移学习与少样本学习(Transfer Learning and Few-Shot Learning)](#迁移学习与少样本学习transfer-learning-and-few-shot-learning)
- [位姿估计(Pose Estimation)](#位姿估计)
  - [直接回归(Direct regression)](#直接回归direct-regression)
  - [关键点检测(Keypoint Detection)](#关键点检测keypoint-detection)
  - [无监督及域自适应(Unsupervised and Domain Adaptation)](#无监督及域自适应unsupervised-and-domain-adaptation)
- [综述(Survey)](#综述survey)
- [数据集(Dataset)](#数据集dataset)
- [评估指标(Evaluation Metric)](#评估指标evaluation-metric)
  - [目标识别评估指标(Target regnition evaluation metric)](#目标识别评估指标target-regnition-evaluation-metric)
  - [位姿估计评估指标(Pose estimation evaluation metric)](#位姿估计评估指标evaluation-metric-for-pansharpening)


## 目标识别(Target Regnition)
### 多模态视觉融合(Multimodal visual fusion)
<table>
    <thead>
      <tr>
        <th>网络模型</th>
        <th>标题</th>
        <th>论文</th>
        <th>代码</th>
        <th>发表期刊或会议</th>
        <th>基础框架</th>
        <th>发表年份</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>LCNN-DMT</td>
        <td>A space non-cooperative target recognition method for multi-satellite cooperative observation systems</td>
        <td><a href="https://www.mdpi.com/2072-4292/16/18/3368">Paper</a></td>
        <td>无</td>
        <td>Remote Sensing</td>
        <td>CNN</td>
        <td>2024</td>
      </tr>
      <tr>
        <td>CNN-Transformer</td>
        <td>Revisiting monocular satellite pose estimation with transformer</td>
        <td><a href="https://ieeexplore.ieee.org/document/9743649/">Paper</a></td>
        <td>无</td>
        <td>IEEE Transactions on Aerospace and Electronic Systems</td>
        <td>Transformer</td>
        <td>2022</td>
      </tr>
      <tr>
        <td>ResNet/改进的PointNet++</td>
        <td>Grasping position recognition of spatial non-cooperative targets based on active light detection</td>
        <td><a href="https://dx.doi.org/10.1088/1742-6596/2029/1/012130">Paper</a></td>
        <td></td>
        <td>Journal of Physics: Conference Series</td>
        <td>PointNet++</td>
        <td>2021</td>
      </tr>
    </tbody>
    </table>
    

### 目标检测与分割(Object Detection and Segmentation)
<table>
    <thead>
      <tr>
        <th>网络模型</th>
        <th>标题</th>
        <th>论文</th>
        <th>代码</th>
        <th>发表期刊或会议</th>
        <th>基础框架</th>
        <th>年份</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>多层Transformer</td>
        <td>Deep learning-based target pose estimation using LiDAR measurements in active debris removal operations</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/8009769/">Paper</a></td>
        <td></td>
        <td>IEEE Transactions on Aerospace and Electronic Systems</td>
        <td>Transformer</td>
        <td>2023</td>
      </tr>
      <tr>
        <td>SCNN-Lite</td>
        <td>Target localization method of non-cooperative spacecraft on on-orbit service</td>
        <td><a href="https://www.sciencedirect.com/science/article/pii/S1000936122000668">Paper</a></td>
        <td>无</td>
        <td>Chinese Journal of Aeronautics</td>
        <td>CNN</td>
        <td>2022</td>
      </tr>
      <tr>
        <td>YOLOv3</td>
        <td>基于改进YOLOv3的空间非合作目标部件识别算法</td>
        <td><a href="https://kns.cnki.net/KCMS/detail/detail.aspx?dbcode=CJFQ&dbname=CJFDLAST2022&filename=JSJA2022S1056">Paper</a></td>
        <td>无</td>
        <td>计算机科学</td>
        <td>YOLO</td>
        <td>2022</td>
      </tr>
      <tr>
        <td>YOLO-GMB</td>
        <td>Lightweight CNN-based method for spacecraft component detection</td>
        <td><a href="https://www.mdpi.com/2226-4310/9/12/761">Paper</a></td>
        <td>无</td>
        <td>Aerospace</td>
        <td>CNN</td>
        <td>2022</td>
      </tr>
      <tr>
        <td>YOLOX_L</td>
        <td>Detection and recognition of spatial non-cooperative objects based on improved YOLOX_L</td>
        <td><a href="https://www.mdpi.com/1424-8220/20/8/2169">Paper</a></td>
        <td>无</td>
        <td>Electronics</td>
        <td>YOLO</td>
        <td>2022</td>
      </tr>
      <tr>
        <td>CNN-YOLOv3</td>
        <td>Utilization of FPGA for onboard inference of landmark localization in CNN-based spacecraft pose estimation</td>
        <td><a href="https://www.mdpi.com/2226-4310/7/11/159">Paper</a></td>
        <td>无</td>
        <td>Aerospace</td>
        <td>CNN</td>
        <td>2020</td>
      </tr>
      <tr>
        <td>YSCRM</td>
        <td>Improved lightweight YOLOv5 using attention mechanism for satellite components recognition</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/9961213">Paper</a></td>
        <td>无</td>
        <td>IEEE Sensors Journal</td>
        <td>YOLO</td>
        <td>2023</td>
      </tr>
      <tr>
        <td>NCDN</td>
        <td>非合作目标局部特征识别轻量化特征融合网络设计</td>
        <td><a href="https://kns.cnki.net/KCMS/detail/detail.aspx?dbcode=CJFQ&dbname=CJFDLAST2020&filename=HWYJ202007034">Paper</a></td>
        <td>无</td>
        <td>红外与激光工程</td>
        <td>SSD</td>
        <td>2020</td>
      </tr>
      <tr>
        <td>HCNN-PSI</td>
        <td>HCNN-PSI: A hybrid CNN with partial semantic information for space target recognition</td>
        <td><a href="https://linkinghub.elsevier.com/retrieve/pii/S0031320320303344">Paper</a></td>
        <td>无</td>
        <td>Pattern Recognition</td>
        <td>CNN</td>
        <td>2020</td>
      </tr>
      <tr>
        <td>Cascade R-CNN</td>
        <td>Spacecraft-DS: A spacecraft dataset for key components detection and segmentation via hardware-in-the-loop capture</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/10380525">Paper</a></td>
        <td><a href="https://github.com/spacecraftds/Spacecraft-DS">Code</a></td>
        <td>IEEE Sensors Journal</td>
        <td>CNN</td>
        <td>2024</td>
      </tr>
      <tr>
        <td>FGBNN</td>
        <td>Space debris detection with fast grid-based learning</td>
        <td><a href="https://ieeexplore.ieee.org/document/9332372/">Paper</a></td>
        <td>无</td>
        <td>IICSPI</td>
        <td>CNN</td>
        <td>2020</td>
      </tr>
      <tr>
        <td>RSD</td>
        <td>R-CNN-based satellite components detection in optical images</td>
        <td><a href="https://www.hindawi.com/journals/ijae/2020/8816187/">Paper</a></td>
        <td>无</td>
        <td>International Journal of Aerospace Engineering</td>
        <td>R-CNN</td>
        <td>2020</td>
      </tr>
      <tr>
        <td>EfficientDet</td>
        <td>Localization and classification of space objects using EfficientDet detector for space situational awareness</td>
        <td><a href="https://www.nature.com/articles/s41598-022-25859-y">Paper</a></td>
        <td>无</td>
        <td>Scientific Reports</td>
        <td>EfficientDet/td>
        <td>2022</td>
      </tr>
    </tbody>
    </table>
    

### 迁移学习与少样本学习(Transfer Learning and Few-Shot Learning)
<table>
    <thead>
      <tr>
        <th>方法</th>
        <th>标题</th>
        <th>论文</th>
        <th>代码</th>
        <th>发表期刊或会议</th>
        <th>基础框架</th>
        <th>年份</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>NOPRN</td>
        <td>Classification and recognition method of non-cooperative object based on transfer learning</td>
        <td><a href="https://www.sciencedirect.com/science/article/pii/S0030399223008988">Paper</a></td>
        <td>无</td>
        <td>Optics & Laser Technology</td>
        <td>ResNet50</td>
        <td>2024</td>
      </tr>
      <tr>
        <td>D2N4</td>
        <td>D2N4: A discriminative deep nearest neighbor neural network for few-shot space target recognition</td>
        <td><a href="https://ieeexplore.ieee.org/document/8949701/">Paper</a></td>
        <td>无</td>
        <td>IEEE Transactions on Geoscience and Remote Sensing</td>
        <td>DCNN</td>
        <td>2020</td>
      </tr>
      <tr>
        <td>DCNN</td>
        <td>Space target recognition based on deep learning</td>
        <td><a href="http://ieeexplore.ieee.org/document/8009786/">Paper</a></td>
        <td>无</td>
        <td>Fusion</td>
        <td>DCNN</td>
        <td>2017</td>
      </tr>
      <tr>
        <td>MWCNN</td>
        <td>A multi-frame super-resolution reconstruction method based on optical flow for space noncooperative objects</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/10883991">Paper</a></td>
        <td>无</td>
        <td>IEEE Access</td>
        <td>CNN</td>
        <td>2020</td>
      </tr>
    </tbody>
    </table>
 
## 位姿估计
### 直接回归(Direct regression)
<table>
    <thead>
      <tr>
        <th>方法</th>
        <th>标题</th>
        <th>论文</th>
        <th>代码</th>
        <th>发表期刊或会议</th>
        <th>基础框架</th>
        <th>年份</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>LSTM</td>
        <td>Parameter precise estimation technology of active segment of non-cooperative targets based on long short-term memory</td>
        <td><a href="https://spj.science.org/doi/full/10.34133/space.0150">Paper</a></td>
        <td>无</td>
        <td>Space: Science & Technology</td>
        <td>LSTM</td>
        <td>2024</td>
      </tr>
      <tr>
        <td>CNN</td>
        <td>CNN-based pose estimation of a non-cooperative spacecraft with symmetries from lidar point clouds</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/10801205">Paper</a></td>
        <td>无</td>
        <td>IEEE Transactions on Aerospace and Electronic Systems</td>
        <td>CNN</td>
        <td>2024</td>
      </tr>
      <tr>
        <td>Dual Transformer</td>
        <td>An efficient pose estimation algorithm for non-cooperative space objects based on dual-channel transformer</td>
        <td><a href="https://www.mdpi.com/2072-4292/15/22/5278">Paper</a></td>
        <td></td>
        <td>Remote Sensing</td>
        <td>Transformer</td>
        <td>2023</td>
      </tr>
      <tr>
        <td>PVSPE</td>
        <td>PVSPE: A pyramid vision multitask transformer network for spacecraft pose estimation</td>
        <td><a href="https://linkinghub.elsevier.com/retrieve/pii/S0273117724004368">Paper</a></td>
        <td>无</td>
        <td>Advances in Space Research</td>
        <td>Transformer</td>
        <td>2024</td>
      </tr>
      <tr>
        <td>DSOAE-Net</td>
        <td>Deep-learning-based direct attitude estimation for uncooperative known space objects</td>
        <td><a href="https://ieeexplore.ieee.org/document/10288068/">Paper</a></td>
        <td>无</td>
        <td>IEEE Transactions on Aerospace and Electronic Systems</td>
        <td>CNN</td>
        <td>2024</td>
      </tr>
      <tr>
        <td>CNN</td>
        <td>End-to-end monocular pose estimation for uncooperative spacecraft based on direct regression network</td>
        <td><a href="https://ieeexplore.ieee.org/document/10068522/">Paper</a></td>
        <td>无</td>
        <td>IEEE Transactions on Aerospace and Electronic Systems</td>
        <td>CNN</td>
        <td>2023</td>
      </tr>
      <tr>
        <td>Swin-Transformer</td>
        <td>Non-cooperative target attitude estimation method based on deep learning of ground and space access scene radar images</td>
        <td><a href="https://www.mdpi.com/2227-7390/11/3/745">Paper</a></td>
        <td>无</td>
        <td>Mathematics</td>
        <td>Transformer</td>
        <td>2023</td>
      </tr>
      <tr>
        <td>DNN</td>
        <td>Deep-neural-network-based angles-only relative orbit determination for space non-cooperative target</td>
        <td><a href="https://www.sciencedirect.com/science/article/pii/S0094576522004891">Paper</a></td>
        <td>无</td>
        <td>Acta Astronautica</td>
        <td>DNN</td>
        <td>2023</td>
      </tr>
      <tr>
        <td>SU-net</td>
        <td>SU-net: Pose estimation network for non-cooperative spacecraft on-orbit</td>
        <td><a href="https://www.nature.com/articles/s41598-023-38974-1">Paper</a></td>
        <td><a href="https://github.com/Tombs98/SU-Net">Code</a></td>
        <td>Scientific Reports</td>
        <td>U-Net</td>
        <td>2023</td>
      </tr>
      <tr>
        <td>EfficientNet-B0+FPN</td>
        <td> An end-to-end pose estimation network for multiscale space non-cooperative objects</td>
        <td><a href="https://ieeexplore.ieee.org/document/10155575">Paper</a></td>
        <td>无</td>
        <td>ICCRE</td>
        <td>EfficientNet</td>
        <td>2023</td>
      </tr>
      <tr>
        <td>PSA-ResNet/td>
        <td>结合极化自注意力机制的空间目标位姿估计</td>
        <td><a href="https://doi.org/10.16804/j.cnki.issn1006-3242.2023.04.011">Paper</a></td>
        <td>无</td>
        <td>航天控制</td>
        <td>ResNet</td>
        <td>2023</td>
      </tr>
      <tr>
        <td>URSONet-Imp</td>
        <td>Autonomous control of the large-angle spacecraft maneuvers in a non-cooperative mission</td>
        <td><a href="https://www.mdpi.com/1424-8220/22/22/8586">Paper</a></td>
        <td>无</td>
        <td>Sensors</td>
        <td>ResNet</td>
        <td>2022</td>
      </tr>
      <tr>
        <td>scSE-LHRNet</td>
        <td>Pose Estimation Method for Non-Cooperative Target Based on Deep Learning</td>
        <td><a href="https://www.mdpi.com/2226-4310/9/12/770">Paper</a></td>
        <td>无</td>
        <td>Aerospace</td>
        <td>HRNet</td>
        <td>2022</td>
      </tr>
      <tr>
        <td>三个并行子网络</td>
        <td>Non-model-based monocular pose estimation network for uncooperative spacecraft using convolutional neural network</td>
        <td><a href="https://ieeexplore.ieee.org/document/9548929/">Paper</a></td>
        <td>无</td>
        <td>IEEE Sensors Journal</td>
        <td>ResNet</td>
        <td>2021</td>
      </tr>
      <tr>
        <td>GoogLeNet</td>
        <td> Vision-based spacecraft pose estimation via a deep convolutional neural network for noncooperative docking operations</td>
        <td><a href="https://www.mdpi.com/2226-4310/7/9/126">Paper</a></td>
        <td>无</td>
        <td>Aerospace</td>
        <td>CNN</td>
        <td>2022</td>
      </tr>
    </tbody>
    </table>

 ### 关键点检测(Keypoint Detection)
 <table>
<thead>
  <tr>
    <th>方法</th>
    <th>标题</th>
    <th>论文</th>
    <th>代码</th>
    <th>发表期刊或会议</th>
    <th>基础框架</th>
    <th>年份</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CSPDarknet53/td>
    <td>Uncooperative spacecraft pose estimation with normalized segmentation coordinate space</td>
    <td><a href="https://ieeexplore.ieee.org/abstract/document/10682976">Paper</a></td>
    <td>无</td>
    <td>IEEE/ASME Transactions on Mechatronics</td>
    <td>YOLO</td>
    <td>2024</td>
  </tr>
  <tr>
    <td>PVSAR</td>
    <td>Pose estimation for cross-domain non-cooperative spacecraft based on spatial-aware keypoints regression</td>
    <td><a href="https://www.mdpi.com/2226-4310/11/11/948">Paper</a></td>
    <td><a href="https://github.com/indigo1973/PVSAR">Code</a></td>
    <td>Aerospace</td>
    <td>PVSAR</td>
    <td>2024</td>
  </tr>
  <tr>
    <td>Lite-HRNet</td>
    <td>Non-cooperative target pose estimation from monocular images based on lightweight neural network</td>
    <td><a href="https://www.sciopen.com/article/10.7527/S1000-6893.2024.30248">Paper</a></td>
    <td>无</td>
    <td>Acta Aeronautica Et Astronautica Sinica</td>
    <td>HRNet</td>
    <td>2024</td>
  </tr>
  <tr>
    <td>YOLO-w6-pose</td>
    <td>Spacecraft homography pose estimation with single-stage deep convolutional neural network</td>
    <td><a href="https://www.mdpi.com/1424-8220/24/6/1828">Paper</a></td>
    <td><a href="https://github.com/pedropro/UrsoNet?tab=readme-ov-file">Code</a></td>
    <td>Sensors</td>
    <td>YOLO</td>
    <td>2024</td>
  </tr>
  <tr>
    <td>HRFORMER</td>
    <td>Transformer Network-Aided Relative Pose Estimation for Non-cooperative Spacecraft Using Vision Sensor</td>
    <td><a href="https://link.springer.com/10.1007/s42405-023-00703-3">Paper</a></td>
    <td>无</td>
    <td>International Journal of Aeronautical and Space Sciences</td>
    <td>Transformer</td>
    <td>2024</td>
  </tr>
  <tr>
    <td>CNN</td>
    <td>Domain randomisation and CNN-based keypoint-regressing pose initialisation for relative navigation with uncooperative finite-symmetric spacecraft targets using monocular camera images</td>
    <td><a href="https://linkinghub.elsevier.com/retrieve/pii/S0273117723001436">Paper</a></td>
    <td>无</td>
    <td>Advances in Space Research</td>
    <td>CNN</td>
    <td>2023</td>
  </tr>
  <tr>
    <td>SLN+LRN</td>
    <td>Monocular relative pose estimation pipeline for uncooperative resident space objects</td>
    <td><a href="https://doi.org/10.2514/1.I011064">Paper</a></td>
    <td>无</td>
    <td>Journal of Aerospace Information Systems</td>
    <td>CNN</td>
    <td>2022</td>
  </tr>
  <tr>
    <td>SDN+KDN</td>
    <td>Learning-based pose estimation of non-cooperative spacecrafts with uncertainty prediction</td>
    <td><a href="https://www.mdpi.com/2226-4310/9/10/592">Paper</a></td>
    <td>无</td>
    <td>Aerospace</td>
    <td>FPN</td>
    <td>2022</td>
  </tr>
  <tr>
    <td>Hourglass-CNN</td>
    <td>Evaluation of tightly- and loosely-coupled approaches in CNN-based pose estimation systems for uncooperative spacecraft</td>
    <td><a href="https://linkinghub.elsevier.com/retrieve/pii/S0094576521000461">Paper</a></td>
    <td>无</td>
    <td>Acta Astronautica</td>
    <td>CNN</td>
    <td>2021</td>
  </tr>
  <tr>
    <td>Improved HRNet</td>
    <td>An improved deep keypoint detection network for space targets pose estimation</td>
    <td><a href="https://www.mdpi.com/2072-4292/12/23/3857">Paper</a></td>
    <td>无</td>
    <td>Remote Sensing</td>
    <td>HRNet</td>
    <td>2020</td>
  </tr>
  <tr>
    <td>Tiny-YOLOv3</td>
    <td>Fast and accurate spacecraft pose estimation from single shot space imagery using box reliability and keypoints existence judgments</td>
    <td><a href="https://ieeexplore.ieee.org/abstract/document/9272988">Paper</a></td>
    <td>无</td>
    <td>IEEE Access</td>
    <td>YOLO</td>
    <td>2020</td>
  </tr>
</tbody>
</table>

## 无监督及域自适应(Unsupervised and Domain Adaptation)
<table>
    <thead>
      <tr>
        <th>方法</th>
        <th>标题</th>
        <th>论文</th>
        <th>代码</th>
        <th>发表期刊或会议</th>
        <th>基础框架</th>
        <th>年份</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>SPNv2/td>
        <td>Robust multi-task learning and online refinement for spacecraft pose estimation across domain gap</td>
        <td><a href="https://www.sciencedirect.com/science/article/pii/S0273117723002284">Paper</a></td>
        <td><a href="https://github.com/tpark94/spnv2">Code</a></td>
        <td>Advances in Space Research</td>
        <td>SPN</td>
        <td>2024</td>
      </tr>
      <tr>
        <td>Transformer</td>
        <td>Bridging the domain gap in satellite pose estimation: A self-training approach based on geometrical constraints </td>
        <td><a href="https://ieeexplore.ieee.org/document/10057169/">Paper</a></td>
        <td>无</td>
        <td>IEEE Transactions on Aerospace and Electronic Systems</td>
        <td>Transformer</td>
        <td>2024</td>
      </tr>
      <tr>
        <td>STN</td>
        <td> A vision-based pose estimation of a non-cooperative target based on a self-supervised transformer network </td>
        <td><a href="https://www.mdpi.com/2226-4310/10/12/997">Paper</a></td>
        <td>无</td>
        <td>Aerospace</td>
        <td>CNN-Transformer</td>
        <td>2023</td>
      </tr>
      <tr>
        <td>Hourglass-CNN</td>
        <td>Spacecraft pose estimation based on unsupervised domain adaptation and on a 3D-guided loss combination</td>
        <td><a href="https://arxiv.org/pdf/2212.13415">Paper</a></td>
        <td><a href="https://github.com/JotaBravo/spacecraft-uda">Code</a></td>
        <td>ECCV</td>
        <td>CNN</td>
        <td>2023</td>
      </tr>
      <tr>
        <td>DSF-VLM</td>
        <td>Position awareness network for noncooperative spacecraft pose estimation based on point cloud</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/9798772">Paper</a></td>
        <td>无</td>
        <td>IEEE Transactions on Aerospace and Electronic Systems</td>
        <td>PANet</td>
        <td>2023</td>
      </tr>
      <tr>
        <td>HRNet</td>
        <td>On-ground validation of a CNN-based monocular pose estimation system for uncooperative spacecraft: Bridging domain shift in rendezvous scenarios</td>
        <td><a href="https://linkinghub.elsevier.com/retrieve/pii/S0094576522001515">Paper</a></td>
        <td>无</td>
        <td>Acta Astronautica</td>
        <td>HRNet</td>
        <td>2022</td>
      </tr>
      <tr>
        <td>SegFormer-MiT-B5</td>
        <td>Robust pose estimation for non-cooperative space objects based on multichannel matching method</td>
        <td><a href="https://www.nature.com/articles/s41598-025-89544-6">Paper</a></td>
        <td>无</td>
        <td>Scientific Reports</td>
        <td>SegFormer</td>
        <td>2025</td>
      </tr>
      <tr>
        <td>DenseFusion</td>
        <td>基于改进DenseFusion的卫星6D位姿估计方法</td>
        <td><a href="https://doi.org/10.14016/j.cnki.jgzz.2025.03.161">Paper</a></td>
        <td>无</td>
        <td>激光杂志</td>
        <td>DenseFusion</td>
        <td>2025</td>
      </tr>
      <tr>
        <td>MSFT</td>
        <td>Configuration optimization method of cooperative target for pose estimation with monocular vision</td>
        <td><a href="https://www.spiedigitallibrary.org/journals/optical-engineering/volume-63/issue-2/023102/Configuration-optimization-method-of-cooperative-target-for-pose-estimation-with/10.1117/1.OE.63.2.023102.full">Paper</a></td>
        <td>无</td>
        <td>Optical Engineering</td>
        <td>Transformer</td>
        <td>2024</td>
      </tr>
      <tr>
        <td>Mask R-CNN+GICP+PCR-GAN</td>
        <td>Vision-based relative position and attitude determination of non-cooperative spacecraft using a generative model architecture</td>
        <td><a href="https://www.sciencedirect.com/science/article/pii/S0094576524004077">Paper</a></td>
        <td>无</td>
        <td>Acta Astronautica</td>
        <td>GAN</td>
        <td>2024</td>
      </tr>
      <tr>
        <td>YOLOv5</td>
        <td>基于深度学习目标识别的航天员训练场景理解技术</td>
        <td><a href="https://doi.org/10.16329/j.cnki.zrht.2023.02.006">Paper</a></td>
        <td>无</td>
        <td>载人航天</td>
        <td>YOLO</td>
        <td>2023</td>
      </tr>
      <tr>
        <td>PointNet++</td>
        <td>Deep-learning-based satellite relative pose estimation using monocular optical images and 3D structural information</td>
        <td><a href="https://www.mdpi.com/2226-4310/9/12/768">Paper</a></td>
        <td><a href="https://github.com/erfect2020/DecompositionForFusion">Code</a></td>
        <td>Aerospace</td>
        <td>PointNet++</td>
        <td>2022</td>
      </tr>
      <tr>
        <td>Siamese CNN</td>
        <td>Deep-learning-based satellite relative pose estimation using monocular optical images and 3D structural information</td>
        <td><a href="https://www.mdpi.com/2226-4310/9/12/768">Paper</a></td>
        <td>无</td>
        <td>Aerospace Science and Technology</td>
        <td>CNN</td>
        <td>2022</td>
      </tr>
      <tr>
        <td>CNN+LSTM</td>
        <td>ChiNet: deep recurrent convolutional learning for multimodal spacecraft pose estimation</td>
        <td><a href="http://arxiv.org/abs/2108.10282">Paper</a></td>
        <td>无</td>
        <td>预印本</td>
        <td>CNN</td>
        <td>2022</td>
      </tr>
    </tbody>
</table>

## 综述(Survey)
<table>
<thead>
  <tr>
    <th>标题</th>
    <th>论文</th>
    <th>发表期刊或会议</th>
    <th>年份</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>A survey on deep learning-based monocular spacecraft pose estimation: Current state, limitations and prospects</td>
    <td><a href="https://www.sciencedirect.com/science/article/pii/S0094576523003995">Paper</a></td>
    <td>Acta Astronaut</td>
    <td>2023</td>
  </tr>
  <tr>
    <td>基于深度学习的航天器位姿估计研究进展</td>
    <td><a href="https://kns.cnki.net/kcms2/article/abstract?v=HbazLCXbuSXpKi7sytq7Bp7EBPrUs4bZwUpqbu-sszF6JB95AzjU3w15V5n0Aby6j4lRBwWbnhReYJBtUs8AhMAOuX2eMnC7oQnHQtRrW47wash3vMh-CQTYenGxmkprRYhesnclgKaYHPcQPrZuLPLWOq-kzCA7KAncu9rK4gDXF6XntwDx5vH1ecqZDANc&uniplatform=NZKPT&language=CHS">Paper</a></td>
    <td>宇航学报</td>
    <td>2023</td>
  </tr>
  <tr>
    <td>位姿视觉测量方法及应用综述</td>
    <td><a href="http://www.opticsjournal.net/Articles/OJe2e12a67711b91ab/FullText">Paper</a></td>
    <td>激光与光电子学进展</td>
    <td>2023</td>
  </tr>
</tbody>
</table>

## 数据集(Dataset)
<table>
<thead>
  <tr>
    <th>数据集</th>
    <th>下载链接</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>SPEED</td>
    <td><a href="https://purl.stanford.edu/dz692fn7184">https://purl.stanford.edu/dz692fn7184</a></td>
  </tr>
  <tr>
    <td>SPEED+</td>
    <td><a href="https://kelvins.esa.int/pose-estimation-2021/">https://kelvins.esa.int/pose-estimation-2021/</a></td>
  </tr>
  <tr>
    <td>URSO</td>
    <td><a href="https://zenodo.org/records/3279632">https://zenodo.org/records/3279632</a></td>
  </tr>
  <tr>
    <td>SPARK</td>
    <td><a href="https://cvi2.uni.lu/spark2022/registration/">https://cvi2.uni.lu/spark2022/registration/</a></td>
  </tr>
  <tr>
    <td>Minerva-II2</td>
    <td><a href="https://github.com/spaceguy-price/Synthetic-Minerva-II2">https://github.com/spaceguy-price/Synthetic-Minerva-II2</a></td>
  </tr>
  <tr>
    <td>SwissCube</td>
    <td><a href="https://huggingface.co/datasets/EPFL-CVLAB-SPACECRAFT/SwissCube">https://huggingface.co/datasets/EPFL-CVLAB-SPACECRAFT/SwissCube</a></td>
  </tr>
  <tr>
    <td>SHIRT</td>
    <td><a href="https://taehajeffpark.com/shirt/">https://taehajeffpark.com/shirt/</a></td>
  </tr>
  <tr>
    <td>BUAA-SID-POSE 1.0</td>
    <td><a href="https://www.kaggle.com/datasets/qiaosijia/buaa-sid-pose10">https://www.kaggle.com/datasets/qiaosijia/buaa-sid-pose10</a></td>
  </tr>
  <tr>
    <td>Cygnus</td>
    <td><a href="https://github.com/brickmack/Blender-Spaceflight-models">https://github.com/brickmack/Blender-Spaceflight-models</a></td>
  </tr>
  <tr>
    <td>AKM</td>
    <td><a href="https://zenodo.org/records/7043325">https://zenodo.org/records/7043325</a></td>
  </tr>
</tbody>
</table>

## 评估指标(Evaluation Metric)
### 目标识别评估指标(Target regnition evaluation metric)
评估指标位于： https://blog.csdn.net/wzk4869/article/details/127879761
### 位姿估计评估指标(Evaluation metric for pansharpening)
评估指标位于： https://blog.csdn.net/m0_38139098/article/details/109532318









