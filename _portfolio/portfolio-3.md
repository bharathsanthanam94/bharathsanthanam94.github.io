---
title: "Tracking crops and weeds with Nvidia Jetson Orin"
excerpt: " Trained an object detector to detect crops and weeds and track the detected objects over frames. Deployed in Nvidia Jetson AGX Orin for real-time inference<br/><img src='/images/tracker_weeds.gif'>"
collection: portfolio
---
### Overview

We train and deploy an object detector and tracker for real-life agricultural fields that detects crops and weeds, tracking them over time. By harnessing the power of the NVIDIA Jetson AGX Orin, coupled with TensorRT, a high-performance deep learning inference optimizer, we efficiently deploy our model to achieve real-time inference.


### Training and Inference

- Train a YOLO based object detector ( we experimented with YOLOV5, V8 and YOLOX) and export the pytorch checkpoint
- Convert the pytorch model to ONNX format
- Create a tensorrt engine on Nvidia Jetson using the above ONNX format
- Perform inference for detection and pass the output to tracker (ByteTrack) to get unique ID for each detected bounding box


![Tracker](/images/tracker_weeds.gif)


### Code :

This project is part of proprietary code developed at the University of Bonn. A prototype version of the code is shared [here](https://github.com/bharathsanthanam94/crop_tracker)

[
]()
