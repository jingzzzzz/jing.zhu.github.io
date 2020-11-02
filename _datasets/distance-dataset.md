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
If you are using any part of our Object-specific Distance dataset(s), please add a reference to our paper. All the original data (i.e., object annoations, RGB images, LiDAR point clouds) is from [KITTT](http://www.cvlibs.net/datasets/kitti/eval_object.php?obj_benchmark=3d) or [NuScenes](https://www.nuscenes.org) datasets. Please cite their paper(s) as well. 


> @inproceedings{zhu2019learning, \\
>   title={Learning object-specific distance from a monocular image}, \\
>   author={Zhu, Jing and Fang, Yi}, \\
>   booktitle={Proceedings of the IEEE International Conference on Computer Vision}, \\
>   pages={3839--3848}, \\
>   year={2019} \\
> }


License
--------
Please notice that this dataset is made availbale for academic research purpose only. The copyright of the original data (i.e., object annotaion, images, LiDAR point clouds) belongs to the original owners (KITTI or NuScenes team). 


Data overview
-----
*KIITI-based annotation
**

  #Values    Name      		Description
  --------------------------------------------------------------------------------
     1    type          		Describes the type of object: 'Car', 'Van', 'Truck',
                            'Pedestrian', 'Person_sitting', 'Cyclist', 'Tram',
                            'Misc' or 'DontCare'
     1    truncated     		Float from 0 (non-truncated) to 1 (truncated), where
                            truncated refers to the object leaving image boundaries
     1    occluded      		Integer (0,1,2,3) indicating occlusion state:
                            0 = fully visible, 1 = partly occluded
                            2 = largely occluded, 3 = unknown
     1    alpha         		Observation angle of object, ranging [-pi..pi]
     4    bbox          		2D bounding box of object in the image (0-based index):
                            contains left, top, right, bottom pixel coordinates, xmin, ymin, xmax, ymax
     3    dimensions    		3D object dimensions: height, width, length (in meters)
     3    location      		3D object location x,y,z in camera coordinates (in meters)
     1    rotation_y    		Rotation ry around Y-axis in camera coordinates [-pi..pi]
     1    forward_dist  		The object-specific distance value, ranged from 0 to 80 meters
     1    lateral_dist  		The object-specific distance value, ranged from -43 to 41 meters
     1    lateral_posit 		The position of the object (bb) center, left:-1, right: 1, middle: 0
     2    forward_keypoint    image plane x, y of the selected (10%) lidar point for forward distance computation
     2    lateral_keypoint    image plane x, y of the selected (10%) lidar point for lateral distance computation


Download
--------
[KITTI-based Distance Dataset]()

[NuScenes-based Distance Dataset]()



