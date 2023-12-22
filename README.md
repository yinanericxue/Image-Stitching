
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

# Image Stitching

#### BFMatcher - Brute-Force Matching
#### https://docs.opencv.org/4.x/dc/dc3/tutorial_py_matcher.html

#### knnMatch
#### https://docs.opencv.org/4.x/db/d39/classcv_1_1DescriptorMatcher.html#a378f35c9b1a5dfa4022839a45cdf0e89
#### https://opencv24-python-tutorials.readthedocs.io/en/latest/py_tutorials/py_feature2d/py_matcher/py_matcher.html!

#### findHomography
#### https://stackoverflow.com/questions/60264322/which-inliers-is-the-ransac-algorithm-using-in-cv2-findhomography-to-find-the-ho
#### https://docs.opencv.org/2.4/modules/calib3d/doc/camera_calibration_and_3d_reconstruction.html#findhomography
![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/aee2d8d6-fa4e-4017-8f67-51b6b77cc239)

#### warpPerspective
#### https://docs.opencv.org/4.x/da/d54/group__imgproc__transform.html#gaf73673a7e8e18ec6963e3774e6a94b87
#### https://blog.csdn.net/qq_18343569/article/details/47953843
#### https://www.cnblogs.com/philip-tell-truth/p/8034019.html
![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/dfb277e0-3fbd-446c-8ecb-43349e79fdc5)
#### Transform the right image by using the H-Matrix:
![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/3b2345b7-dfe2-4554-aaf4-172e3f4ec6bc)
![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/18f78cd9-1567-47bc-991c-bd2b04d2de93)
![image](https://github.com/yinanericxue/Image-Stitching/assets/102645083/2f1782f8-725f-4676-a2a5-3b9e73459576)



