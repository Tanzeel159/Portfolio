---
title: "Real Time Object Detection"
description: "Object detection"
dateString: Sep 2018
draft: false
tags: ["Tensorflow Toolkit", "TensorBoard", "Protobuf", "LabellMG", "Python", "Anaconda","Tensorflow"]
showToc: false
weight: 405
cover:
    image: "/projects/real-time-object-detection/120095122-bf36b280-c141-11eb-8fbe-380d0a813ad9.jpeg"
---

🔗 [Github](https://github.com/Tanzeel159/Real-Time-Object-detection)

## Description

When we're shown an image, our brain instantly recognizes the objects contained in it. On the other hand, it takes a lot of time and training data for a machine to identify these objects.The processing of visual data happens in the ventral visual stream.Humans can easily recognize different sized objects and put them in the same category. Object detection refers to the capability of computer and software systems to locate objects in an image/scene and identify each object. In this project we try to implement Object Detection using Single Shot Multibox Detector.Object detection has been widely used for face detection, vehicle detection, pedestrian counting, web images, security systems and driverless cars. Major features of SSD include object localization and classification in single step, bounding boxes to detect objects and detector.

## Algorithm

1) Pass the image through a series of convolutional layers
2) For each location in each of these feature maps, use a 3x3 convolutional filter to evaluate a small set of default bounding boxes.
3) For each box, simultaneously predict the bounding box offset and the class probabilities
4) During training, match the ground truth box with these predicted boxes based on IoU(Intersection over union).
5) Instead of using all the negative examples, sort the results using the highest confidence loss for each default box and pick the top ones so that the ratio between the negatives and positives is at most 3:1.

![Alt text](/projects/real-time-object-detection/image1.png)

## Implementation

![SSD Model](/projects/real-time-object-detection/image.png)

## Training

![training](/projects/real-time-object-detection/training.png)

## Labelling

![Gathering image](/projects/real-time-object-detection/image_gather.png)

## Results

<video src="/projects/real-time-object-detection/Object_Detector.mp4" controls title="Title" width="705"></video>