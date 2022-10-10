# Nvidia Jetson Nano Guidance
Jetson Nano is our toys in TBI lol :)). We will working with this little but powerfull machine. You can check detail of Jetson Nano [here](https://developer.download.nvidia.com/assets/embedded/secure/jetson/Nano/docs/JetsonNano_DataSheet_DS09366001v1.1.pdf?Z0rNAR7mzYEvRE7l18gq1b3B4LE7ah__hD-mlwNLIE6R_xaijBKvycjrEXB29A1K_2QLik0HuYLCpCXM6FOLG5LpxOW54rSjc1Moq3DoOcb9G6H2RTdUbxO8K1x3CZu6-tL44aW4Io4N36jTBh1kn1FX9jniA8CWWWfh-ZkOe5fQFKeduj4l3-qaLxCyNQ&t=eyJscyI6ImdzZW8iLCJsc2QiOiJodHRwczpcL1wvd3d3Lmdvb2dsZS5jb21cLyJ9). Jetson Nano commonly will work with deep learning algorithm, so we set it up OpenCV CUDA enabled. 

### Outline
- Jetson Case
- Power Supply
- Installation
- Running YOLOv5

*It's not easy and need hours just for installation. Make it fun!!!!!*

## Case and Fan

Case is so important for Jetson Nano, it's prevent evil things happen to this litter machine. It also easier to carry the Jetson. I found a lot of 3d models for Jetson Nano. I selected one and printed it out. You can check it out in [3d folder](https://github.com/kangyolo/get-started-jetson-nano/tree/main/3d)

You also need a cooling fan to control the heat. I bought litte cooling fan for Jetson Nano [here](https://shopee.co.id/Dedicated-Cooling-Fan-for-Jetson-Nano-5V-3PIN-Reverse-proof-i.27499686.7977315796)

## Power Supply

Power supply is one of the most important things when playing with Jetson. 

Do not use 5V 2A power supply throught USB cable, it's suck. Use 5V 4A with jack cable. Read full article about power supply [here](https://jetsonhacks.com/2019/04/10/jetson-nano-use-more-power/)

I bought power supply [here](https://shopee.co.id/Power-Supply-5V-4A-Applicable-for-Jetson-Nano-i.27499686.7677332255)

![power supply](/doc/psu.PNG)


## Installation

Jetson Nano required Jetpack running on Linux operating system. Image file that needed to be flashed to the SD card. The official image that provided by Nvidia is not stable at all. There are multipe custom image files that provided by the comunity. 

[Here](https://github.com/Qengineering/Jetson-Nano-image) is image file that installed Linux Ubuntu 20.04. A Jetson Nano image with OpenCV, TensorFlow and Pytorch. With this image file, it is not necesary to set up the environment from the scratch.

### Running JTOP
JTOP stand for Jetson-Stat, it's a program to monitor Jetson Nano status

just run this command on terminal:

```
jtop
```

## Running YOLOv5

Clone the official YOLOv5 repository with git

```
git clone https://github.com/ultralytics/yolov5.git
```

Make sure the python3 and pip3 is python3.8 version. If it's not, you need to install it and set up the python3 variabel.

*Written by: Oki Aryawan*
