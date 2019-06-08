# 3D-segmentation

In this project i use the cnn to do the semantic segmentation in 2d image, and then use the results to do 3d reconstruction.

As you can see there is lots of errors caused by segmentation, some points which are far away from the object are also recognized as part of object, I think this is because that the information of object in one image is often incomplete and  CNN cannot use the information from other images(other viewpoints), but in 3d scene it’s easy to distinguish these error points. So, I feel that semantic segmentation in 2D and 3D scene reconstruction can be an iterative process used to improve the performance of segmentation.  I am still working on it. 

![](https://github.com/william-in-kit/3D-segmentation/blob/master/joinMap/color(origin)/1.png)
![](https://github.com/william-in-kit/3D-segmentation/blob/master/joinMap/color/1.jpg)
![](https://github.com/william-in-kit/3D-segmentation/blob/master/1.png)
