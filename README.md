
# Social Distancing Detector Using Deep Learning 

This application is 
developed to give alerts to people for maintaining social distance in crowded places. By 
using pre-recorded video as input and the open-source object detection pretrained model 
using the YOLOv3 algorithm We can tell if people are following social distancing or not and 
based on that we are creating red or green bounding boxes over it. It is also working on web 
cameras, CCTV, etc, and can detect people in real-time. This may help authorities to redesign 
the layout of public places or to take precautionary actions to mitigate high-risk zones.it can 
be used in other fields also like autonomous vehicles, human action recognition, crowd 
analysis.

</br>

Detect the social distance violations in real time using OpenCV and deep learning

> ## ***"Social distancing is the only way to counter Covid-19"***

**Requirements**
- Python
- Numpy
- OpenCV
- Scipy
- Object Detection models (Mobilenet or Googlenet or YOLO)

***Steps***
1. Input the video stream using OpenCV
2. Detect the people in the video stream using any of the object detection models
3. Find the centroids of the identified people and calculate the distance between the centroids
4. Check if the distance calculated above is lesser than the minimum value (in pixels) and consider it as violation
5. Draw the bounding boxes in red color around the person if violating, green color box if the person is following the norms


_💻 Install the dependencies on command line:_

```sh
$ pip3 install -r requirement.txt
```

_💻 To run the program on command line:_

```sh
$ python3 sdd.py
```

</br>

### 🎬 Output example:

| ![outputimage](/images/TownCentre_new.gif) |
| ------------------------------------------ |


**Frame 10 to 500:**

| ![outputimage](/images/data/frame10.jpg) | ![outputimage](/images/data/frame100.jpg) | ![outputimage](/images/data/frame200.jpg) |
| :-----------------------------------------: | :------------------------------------------: | :------------------------------------------: |
|                **FRAME 10**                 |                **FRAME 100**                 |                **FRAME 200**                 |

| ![outputimage](/images/data/frame300.jpg) | ![outputimage](/images/data/frame400.jpg) | ![outputimage](/images/data/frame500.jpg) |
| :------------------------------------------: | :------------------------------------------: | :------------------------------------------: |
|                **FRAME 300**                 |                **FRAME 400**                 |                **FRAME 500**                 |

### 🎯 Accuracy for person detection:

| Dataset            | TP  | TN  | FP  | FN  | %    |
| ------------------ | --- | --- | --- | --- | ---- |
| Oxford Town Centre | 29  | 0   | 0   | 11  | 72.5 |

### 🎯 Accuracy for social distance violation detection:

| Dataset            | TP  | TN  | FP  | FN  | %   |
| ------------------ | --- | --- | --- | --- | --- |
| Oxford Town Centre | NA  | NA  | NA  | NA  | NA  |



### ⏳ Future upgrades:

| Features                                              | Status                                                                |
| ----------------------------------------------------- | --------------------------------------------------------------------- |
| Camera calibration for intrinsic parameter (distance) | ![STATUS](https://img.shields.io/badge/camera_calibration-passed-brightgreen) |
| Add facemask detection                                | ![STATUS](https://img.shields.io/badge/face_mask-TBD-orange) |
| upgrade to YOLO v4                                    | ![STATUS](https://img.shields.io/badge/build-passed-brightgreen) |

---

## Kindly check out below links:

**Download YOLO Pre-Trained Model** </br>
[![YOLO](https://img.shields.io/badge/YOLO-Darknet-YELLOW)](https://drive.google.com/file/d/1yRnBkjpWjClZtKUaOgRSblgA8i0OiAXD/view?usp=share_link)


