# 小车识别及方向检测


## 简介

山东大学 2020级数据科学与人工智能班计算机视觉项目第一部分：小车识别与方向检测

单目摄像头实现小车识别和方向检测，小车识别部分使用PP-YOLOv2，朝向检测使用我们自己搭建的网络，均在百度飞桨AI Studio完成模型训练，并进行本地化部署。

## 复现

### 小车识别

我们在百度AI Studio基于PP-YOLOv2训练了小车识别模型，详见[[百度AI Studio]基于PP-YOLOv2的小车识别](https://aistudio.baidu.com/projectdetail/8234915)

### 方向检测

我们在百度AI Studio基于自己搭建的网络训练了朝向检测模型，详见[[百度AI Studio]小车方向检测](https://aistudio.baidu.com/projectdetail/8234948)

## 本地部署

### 环境

- Python＞=3.7
- paddlepaddle-gpu==2.3.2
- PaddleDetection==2.5
- CUDA >= 10.2
- cuDNN >= 7.6
- opencv-python==3.4

关于如何安装PaddleDetection，请参考[PaddleDetection Installation](https://github.com/PaddlePaddle/PaddleDetection/blob/release/2.5/docs/tutorials/INSTALL.md).

### 安装依赖

- 克隆本项目

```
git clone https://github.com/leonardeee/RL-Auto-Parking-.git
```

- 进入项目目录

```
cd Car-Direction-Detection
```

- 安装环境

```
pip install -r requirements.txt
```

### 下载模型

可以下载AI Studio项目中提供的模型，也可以在AI Studio中fork项目并训练你自己的模型

### 运行模型

```
python Car_Orientation_Dtection.py
```

## 结果

<center>
 <img src=".\images\Orientation Detection.png">
</center>

<center>
 <img src=".\images\Orientation Detection and Automatic Driving.png">
</center>


