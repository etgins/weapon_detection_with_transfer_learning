# Weapon Detection with Transfer Learning
In this project we attempt to use a pretrained YOLOv5 model to detect weapons in various scenarios.  
We use Transfer-Learning by additional training on a pre-trained network using the new dataset to achieve this task.  
Class project as part of ee046211 - Deep Learning course @ Technion.  
<p align="center">
    <a href="https://www.linkedin.com/in/itamar-ginsberg/">Itamar Ginsberg</a>  •  
    <a href="https://il.linkedin.com/in/alon-nemirovsky-3082651b4">Alon Nemirovsky</a>
</p>

- [Weapon Detection with Transfer Learning](#Weapon%20Detection%20with%20Transfer%20Learning)
  * [Background](#Background)  
  * [Dataset](#Dataset)  
  * [Model](#Model)  
  * [Files in the repository](#Files%20in%20the%20repository)
  * [Sources](#Sources)

## Background
To ensure citizen's safety, we want to enable security cameras to detect a person carrying a weapon, so security services can be quickly alerted and can decide on the best course of action, thus dramatically reducing response time to save lives. 
For this purpose, take advantage of an advanced neural-network architecture utilized for detection tasks in other domains through the technique of transfer-learning.

## Dataset
We use the [ari-dasci/OD-WeaponDetection](https://github.com/ari-dasci/OD-WeaponDetection) dataset, mainly 'Knife Detection' and 'Pistol Detection'.  
The data includes 3000 pistol images and 2078 knife images.  
**Image examples from the dataset:**  

<p align="center">
<img src="repository_images/armas%20(107).jpg" height="200" > <img src="repository_images/armas%20(2070).jpg" height="200"> <img src="repository_images/armas%20(1101).jpg" height="200">  </p>
<p align="center">
<img src="repository_images/DSC_00481.JPG" height="200"> <img src="repository_images/knife_48.jpg" height="200"> <img src = "repository_images/KravMagaKnifeDefenseTechniques249.jpg" height="200"> </p>

**Annotation examples from the dataset: (matching the images above)**  
 [0 0.378 0.387 0.205 0.332]  
 [0 0.531 0.536 0.179 0.326]  
 [0 0.501 0.506 0.424 0.364]  
 [1 0.351 0.669 0.163 0.105]  
 [1 0.521 0.449 0.647 0.601]  
 [1 0.618 0.297 0.116 0.081]  

Each file includes the class number of the detect object (0 - pistol, 1 - knife) and 4 points (normalized) indicating the object bounding box.

## Model
<p align="center">
<img src="repository_images/YOLOv5%20Structure.png" width="600" >
</p>

YOLO (You Only Look Once) divides an image into a grid system, and each grid detects objects within itself. It is a very fast algorithm that can be used for *real-time* object detection based on data streams, while requiring very few computational resources.
*TODO - add information about YOLO and YOLOv5

<p align="center">
<img src="repository_images/YOLOv5%20models.png" width="600" >
</p>
*TODO - add information about the different YOLOv5 models

## Files in the repository

*TODO - fill in file descriptions
|File name         | Description |
|----------------------|------|
|`file name 1`| File 1 Description|
|`file name 2`| File 2 Description|

## Results
*TODO - fill in results and screenshot

## Presentation
*TODO - links to youtube and slides
- [Recording](URL) of in-class project presentation (Hebrew only)
- Slides can be found [here](https://docs.google.com/presentation/d/1YwvSj-yY5Msszw83hv6qB6qxPFPEGPw6swNo3wLiULk/edit?usp=sharing)

## Sources  
*TODO - more resources  
[1] ari-dasci/[OD-WeaponDetection](https://github.com/ari-dasci/OD-WeaponDetection) full dataset  
[2] Ultralytics [YOLOv5 repository](https://github.com/ultralytics/yolov5)   
[3] Ultralytics [YOLOv5 documentation](https://docs.ultralytics.com/)  
[4] Bochkovskiy, A., Wang, C.Y. and Liao, H.Y.M., 2020. [Yolov4: Optimal speed and accuracy of object detection](https://arxiv.org/abs/2004.10934) (arXiv preprint arXiv:2004.10934.)  
[5] analytics-vidhya (Medium): [Object Detection Algorithm — YOLO v5 Architecture](https://medium.com/analytics-vidhya/object-detection-algorithm-yolo-v5-architecture-89e0a35472ef)
