# Uncertainty-Aware Fast Curb Detection Using\\ Convolutional Networks in Point Clouds
## **Introduction**
Younghwa Jung, Mingu Jeon, Chan Kim, Seung-Woo Seo, and Seong-Woo Kim, "Uncertainty-Aware Fast Curb Detection Using Convolutional Networks in Point Clouds," accepted for IEEE International Conference on Robotics and Automation (ICRA), Xi'an, China, 2021.
## Data set
```
├── Total_data_set_line
│   ├── Training (4,724 frame)
│   │   ├── input_data
│   │   │             ├──density_map 
│   │   │             └──heights_map            
│   │   ├── labels
│   │   ├── top_view_raw
│   │   └── pcd_file
│   │
│   └── test (500 frame)
│       ├── input_data
│       │            ├──density_map 
│       │            └──heights_map
│       ├── labels            
│       ├── top_view_raw
│       └── pcd_file
│
│
└── Total_data_set_point
│   ├── Training (4,820 frame)
│   │   ├── input_data
│   │   │             ├──density_map 
│   │   │             └──heights_map            
│   │   ├── labels
│   │   ├── top_view_raw
│   │   └── pcd_file
│   │
│   └── test (2,000 frame)
│       ├── input_data
│       │            ├──density_map 
│       │            └──heights_map
│       ├── labels            
│       ├── top_view_raw
│       └── pcd_file

```
Data description
* The number of total frame in Total_data_set_line is 5,524.
* The number of total frame in Total_data_set_point is 6,820.
* The reason why the number of total frame in two folder is diffent is that we cannot draw lines from the points in some areas. 

Folder descrption
* Total_data_set_line : The label format is lines in 2D image domain.
* Total_data_set_point : The label format is points in 2D image domain.
* input_data : It consists of two folders; density_map and height_maps
* labels : 2D image(320x416). The pixel values for curb area are one. The others area are zero.
* top_view_raw : The bird's eye view image of 3D point cloud for visualization.
* pcd_file : 3D raw point cloud.

The link for dataset is https://drive.google.com/file/d/1wWIfqSJWXSlpD9BlSobL69fhABNJe9tX/view?usp=sharing

## Label Extraction from Semantic Map

[![Watch the video](https://drive.google.com/uc?export=view&id=1uM0ZzE4l2KcD10db5l6jWYRP02sbAiYr)](https://youtu.be/2d28cw9zb-0)


### Requirements
* Python 3.5
* Tensorflow 1.11

## Cite
If you think this work is useful in your research, please consider cite our paper:
```
@INPROCEEDINGS {jung2021curb,
    AUTHOR = {Younghwa Jung, Mingu Jeon, Chan Kim, Seung-Woo Seo, and Seong-Woo Kim},
    TITLE = {Uncertainty-Aware Fast Curb Detection Using Convolutional Networks in Point Clouds },
    BOOKTITLE = {Proceedings of the IEEE International Conference on Robotics and Automation (ICRA) },
    YEAR = {2021},
    MONTH = {May},
    ADDRESS = {Xian},
    NOTE = {Accepted. To appear.},
}

```



