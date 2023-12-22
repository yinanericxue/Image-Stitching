
# Image Stitching

# RANSAC - Random Sample Consensus

### Use Case and Theory
#### https://www.mathworks.com/discovery/ransac.html
#### https://medium.com/@saurabh.dasgupta1/nearest-neighbour-distance-metric-approach-to-determine-the-ransac-threshold-f0213562a196
#### https://medium.com/mlearning-ai/outlier-detection-using-the-ransac-algorithm-de52670adb4a

# Homogeneous Coordinates / Projective Coordinates
#### https://yasenh.github.io/post/homogeneous-coordinates/
#### https://www.javatpoint.com/computer-graphics-homogeneous-coordinates
<img width="594" alt="Screen Shot 2023-12-21 at 8 14 35 PM" src="https://github.com/yinanericxue/Image-Stitching/assets/102645083/5471cc8b-da06-413b-af47-f1cdcad19b23">

![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/7c813d47-095e-485e-a661-14a4b533496a)

![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/60819124-ad77-4cfa-9ce9-7ac62c4d4b59)

![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/8df3ec8f-bf9a-4cdb-8c26-994dee07dd68)

![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/c5612e76-919e-451f-804c-df2c3c7e6ff6)

#### Rotate
![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/d3d98b19-8998-4075-8ca7-8a02625851be)

#### Translate
![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/1ccf9c40-cf8f-43cb-ac77-f2024ce030c2)

#### Rotate and Translate in Homogeneous Coordinates
![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/8e87e48c-e8bc-4365-9f71-8db1ebf80797)
![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/537d09ce-978d-4f0a-aa72-a2c2c9f05d7a)

# Homography Matrix
#### https://docs.opencv.org/4.x/d9/dab/tutorial_homography.html
#### https://mattmaulion.medium.com/homography-transform-image-processing-eddbcb8e4ff7

![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/05ca5017-525a-43a5-92cd-58f254fc0adf)


#### (x1,y1) (x2,y2) (x3,y3) (x4,y4)  ->  (x1',y1') (x2',y2') (x3',y3') (x4',y4')   (4 source points, 4 destination points)

#### 8 parameters require 8 different functions

#### Two ways to deal with many outliers
####	1) Find the least squared estimation and find a new function
####  2) RANSAC, find the inliers, preferably only a couple

![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/38ba4728-8f37-4e35-9210-60cff71be38c)

![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/9877c06f-3563-4a89-ae7c-521ee9fe6e79)

![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/2f214bc8-c53a-4347-a970-6dd9d7ab1c3e)






