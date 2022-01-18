# Weapon Detection with Transfer Learning
In this project we attempt to use a pretrained YOLOv5 model to detect weapons in various scenarios.  
We use Transfer-Learning by training only the last layers on the new dataset to achieve this task.  
Class project as part of ee046211 - Deep Learning course @ Technion.  
In collaboration with Alon Nemirovsky.  


- [Weapon Detection with Transfer Learning](#Weapon%20Detection%20with%20Transfer%20Learning)
  * [Dataset](#Dataset)  


## Dataset
We use the [ari-dasci/OD-WeaponDetection](https://github.com/ari-dasci/OD-WeaponDetection) dataset, mainly 'Knife Detection' and 'Pistol Detection'.  
**Image examples from the dataset:**  
<img src="repository_images/armas%20(107).jpg" height="200" >
<img src="repository_images/armas%20(2070).jpg" height="200">
<img src="repository_images/armas%20(1101).jpg" height="200">  
<img src="repository_images/DSC_00481.JPG" height="200">
<img src="repository_images/knife_48.jpg" height="200">
<img src = "repository_images/KravMagaKnifeDefenseTechniques249.jpg" height="200">

**Annotation examples from the dataset: (matching the images above)**  
[0 0.378 0.387 0.205 0.332]   
[0 0.531 0.536 0.179 0.326]   
[0 0.501 0.506 0.424 0.364]  
[1 0.351 0.669 0.163 0.105]  
[1 0.521 0.449 0.647 0.601]  
[1 0.618 0.297 0.116 0.081]  


## File Descriptions

Both file are well documented. just follow the documentation and you will be fine :)

|File name         | Description |
|----------------------|------|
|`file name 1`| File 1 Description|
|`file name 2`| File 2 Description|


# Sources

Dataset source: https://www.kaggle.com/c/cassava-leaf-disease-classification  
> Description 1: url 1

> Description 2: url 2
