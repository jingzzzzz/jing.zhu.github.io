---
title: "Object-specific Distance Dataset"
collection: datasets
type: "Datasets"
permalink: /datasets/distance-dataset
#date: 2014-01-01
---

Datasets constructed based on KITTI and NuScenes object detection datasets. For each object in the RGB image, we calculate a object-specific distance (in meters) from a set of LiDAR point clouds. For more details, please refer to [our paper](https://openaccess.thecvf.com/content_ICCV_2019/papers/Zhu_Learning_Object-Specific_Distance_From_a_Monocular_Image_ICCV_2019_paper.pdf). 

<img src="/images/DistanceDataset.png" alt="drawing" align="left" width="600" height="350"/>  




Citation
--------
If you are using any part of our Object-specific Distance dataset(s) or codes, please add a reference to our paper. All the original data (i.e., object annoations, RGB images, LiDAR point clouds) is from [KITTT](http://www.cvlibs.net/datasets/kitti/eval_object.php?obj_benchmark=3d) or [NuScenes](https://www.nuscenes.org) datasets. Please cite their paper(s) as well. 


> @inproceedings{zhu2019learning, \\
>   title={Learning object-specific distance from a monocular image}, \\
>   author={Zhu, Jing and Fang, Yi}, \\
>   booktitle={Proceedings of the IEEE International Conference on Computer Vision}, \\
>   pages={3839--3848}, \\
>   year={2019} \\
> }



License
--------
Please notice that this dataset is made availbale for **academic research purpose** only. The copyright of the original data (i.e., object annotaion, images, LiDAR point clouds) belongs to the original owners (KITTI or NuScenes team). 



Download
--------
* KITTI-based 
  * [Distance Dataset]()
  * [Code to calculate distance annotation]()

* NuScenes-based Distance Dataset(*to be released*)







