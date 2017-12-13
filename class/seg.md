<!-- page_number: true -->
<!--$theme: gaia-->

　
# 遥感数字图像处理实验课
## - 图像分割之分水岭算法
<br/><br/>
崔家梁
(cuijialiang@pku.edu.cn)  

---
# 伯克利的图像分割与基准数据集
https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/bsds/

- .m格式的分割groundtruth

---
# 分水岭算法

---
# 盆地与分水岭
![250%](https://cn.mathworks.com/content/mathworks/cn/zh/company/newsletters/articles/the-watershed-transform-strategies-for-image-segmentation/jcr:content/mainParsys/image_1.adapt.full.high.jpg/1480512444309.jpg) ![180%](https://cn.mathworks.com/content/mathworks/cn/zh/company/newsletters/articles/the-watershed-transform-strategies-for-image-segmentation/jcr:content/mainParsys/image_2.adapt.full.high.gif/1480512444319.gif)

---
### 对于一张灰度图片(通常为要分割的图像的梯度图)
![](http://cmm.ensmp.fr/~beucher/ima1.gif)![](http://cmm.ensmp.fr/~beucher/ima2.gif)  
将其想象成一个DEM(右图为加了一个光照的渲染效果)

---
# 填充过程
![100%](http://cmm.ensmp.fr/~beucher/lpe1.gif)![](http://cmm.ensmp.fr/~beucher/ima3.gif)  
从最低处开始填充,可以得到盆地和分水岭.

---
# 分水岭算法-基本思路
![](http://cmm.ensmp.fr/~beucher/ima6.gif)  

左上-原图
右上-梯度图
左下-梯度图的分水岭
右下-将分水岭分割结果显示在原图上

---
# 分水岭算法的问题-分割过细
![](http://cmm.ensmp.fr/~beucher/ima7.gif)![](http://cmm.ensmp.fr/~beucher/ima7b.gif)

---
# 分水岭算法的改进算法
- 基于标记的分水岭算法
- 多级分水岭算法

---
# 基于标记的分水岭算法

![](http://cmm.ensmp.fr/~beucher/ex1a.gif)![](http://cmm.ensmp.fr/~beucher/ex1b.gif)

---
# 多级分割算法-瀑布变换
![80%](http://cmm.ensmp.fr/~beucher/hier1.gif)![80%](http://cmm.ensmp.fr/~beucher/hier2.gif)
![80%](http://cmm.ensmp.fr/~beucher/hier3.gif)![80%](http://cmm.ensmp.fr/~beucher/hier4.gif)
http://cmm.ensmp.fr/~beucher/wtshed.html

---
# P算法
http://cmm.ensmp.fr/~beucher/publi/P-Algorithm_SB_BM.pdf

---
# 作业
- 打开一张黑白图片;
- 实现一种图像分割(可以调用库);
- 显示分割结果;

12.20日(下周三)10:00前交至cuijialiang@pku.edu.cn

---

# References  
- CMM的分水岭介绍 http://cmm.ensmp.fr/~beucher/wtshed.html

- Matlab官网的分水岭介绍 https://cn.mathworks.com/company/newsletters/articles/the-watershed-transform-strategies-for-image-segmentation.html
- 多级分割
http://www.seascapesoft.org/about-seascape/hierarchical-segmentation

---
- 深度学习的图像分割算法总结(2017)
http://blog.qure.ai/notes/semantic-segmentation-deep-learning-review