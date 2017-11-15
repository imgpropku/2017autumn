<!-- page_number: true -->
<!--$theme: gaia-->

　
# 遥感数字图像处理实验课
## - 图像增强
<br/><br/>
崔家梁  
(cuijialiang@pku.edu.cn)  
2017年11月

---
# 图像的直方图
![150%](https://docs.opencv.org/3.0-beta/_images/histogram_sample.jpg)

---
# 直方图均衡化-算法

![140%](https://docs.opencv.org/3.0-beta/_images/histogram_equalization.png)

![](https://docs.opencv.org/3.0-beta/_images/histeq_numpy2.jpg)

---
# 直方图均衡化-效果

![50%](figures/hist_equal1.png)![50%](figures/hist_equal2.png)
![120%](https://docs.opencv.org/3.0-beta/_images/equalization_opencv.jpg)

---
# 频域滤波

- 高通滤波
  通过高频信息(边界,噪声等)
- 低通滤波
  通过低频信息(物体大致形状等)

---
# 高通与低通滤波
![80%](figures/Xpass_filters.png)

---
# 低通滤波
- 去除噪声,图像平滑

高斯低通滤波:
![](figures/lowpass-gauss.png)

---
# 高通滤波
- 噪声提取,图像锐化

![70%](figures/highpass-gauss.png)

---
~~## 作业1-实现直方图均衡化~~
~~- 对一张图片实现直方图均衡化;~~
  ~~- 可以随意调用.~~ 
## 作业2-实现高通,低通滤波
- 对一张图片实现高斯高通,低通滤波;
- 要求使用Tensorflow实现(tf.nn.conv2d);

请于本周五(11月17日)10:00前提交至  cuijialiang@pku.edu.cn

---
# 遥感数字图像处理实验课
## - 大作业
<br/><br/>
崔家梁
(cuijialiang@pku.edu.cn)  

---
# 可供选题1-图像拼接

![](https://upload.wikimedia.org/wikipedia/commons/thumb/2/2c/Alcatraz03182006.jpg/1700px-Alcatraz03182006.jpg)

![](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a0/Rochester_NY.jpg/700px-Rochester_NY.jpg)

---
# 可供选题2-图像特征提取与匹配
![](http://opencv-python-tutroals.readthedocs.io/en/latest/_images/sift_keypoints.jpg)
- 至少实现一种图像特征提取算法(SIFT,SURF,ORB,FAST,BRIEF等)

---
# 可供选题3-人脸检测/识别
![](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ef/Face_detection.jpg/440px-Face_detection.jpg)![66.5%](https://docs.opencv.org/3.3.0/face.jpg)

---
# 可供选题4-图像分割
![60%](https://upload.wikimedia.org/wikipedia/commons/thumb/a/aa/Polarlicht_2.jpg/600px-Polarlicht_2.jpg)![60%](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c5/Polarlicht_2_kmeans_16_large.png/600px-Polarlicht_2_kmeans_16_large.png)

![70%](https://devblogs.nvidia.com/parallelforall/wp-content/uploads/2016/11/figure4.png)

---
## 分组要求
- 4~5人一组,选出组长.

## 作业要求
- 可以选择我推荐的选题,可以重复,也可以自己选之后告诉我.
- 要有一定代码量,不能直接调用高级函数.
- 需要提交源代码,文档等.
- 学期末会有一次课上演示,需要展示结果,讲解算法并答疑.

11月17日上课前分好组,选好组长.