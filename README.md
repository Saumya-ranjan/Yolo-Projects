## Intro
You only look once (YOLO) is a state-of-the-art, real-time object detection system. On a Pascal Titan X it processes images at 30 FPS and has a mAP of 57.9% on COCO test-dev.

## How It Works
Prior detection systems repurpose classifiers or localizers to perform detection. They apply the model to an image at multiple locations and scales. High scoring regions of the image are considered detections.

It uses a totally different approach. It apply a single neural network to the full image. This network divides the image into regions and predicts bounding boxes and probabilities for each region. These bounding boxes are weighted by the predicted probabilities.

Real-time object detection and classification. Paper: [version 1](https://arxiv.org/pdf/1506.02640.pdf), [version 2](https://arxiv.org/pdf/1612.08242.pdf).

Read more about YOLO (in darknet) and download weight files [here](http://pjreddie.com/darknet/yolo/).

## Dependencies
Python3, tensorflow 1.0, numpy, opencv 3.

## My Internship Work:
```sh
1] Label and annotate Images 
2] Getting .txt files for each image with classes.txt and zipping the folder
3] Putting zip folder into darknet and running the algorithm --usually first time it takes more than 6 hour
4] So after training and testing using darknet detector to see yolo predictions for images given by Us
5] Submitting zip folder to organization.
```


