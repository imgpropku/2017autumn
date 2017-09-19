<!-- page_number: true -->
<!--$theme: gaia-->

　
# 遥感数字图像处理实验课
## - 0 关于课程
<br/><br/>
崔家梁
(cuijialiang@pku.edu.cn)  

---
# 课程简介

《遥感数字图像处理原理(赵红颖副教授)》课程的**实验课**

两周一次

#### 课程主页(课件&demo)
https://github.com/imgpropku/2017autumn

---
# 实验课需要先修的内容

- 计算概论、数据结构与算法、程序设计原理等计算机基础课  
- 掌握python语言基本操作

---

# 课程内容

1-图像处理基本操作  
2-图像傅里叶变换  
3-角点检测  
4-模板操作  
5-深度学习图像处理简介(待定)  
6-深度学习工具简介(待定)   
7-深度学习图像处理示例(待定)  

#### 本课程注重算法的实现

---
# 开发环境-上课demo


python 3(amd64) 及该版本下的pip工具链;  

jupyter-notebook(安装方式:pip install notebook)

### 推荐作业采用与以上相同的开发环境

---
# 提交作业可选的开发环境:
- Python3 或 jupyter-nb(py3) (推荐):smiley:;  
- C++(gcc:smiley: 或 clang:smiley:, **拒绝  VC&.NET**:imp:);  
- Matlab (接受但不推荐):expressionless:.  

---
# 作业
- 小作业  
  - 个人  
  - 编程实现简单的图像处理算法  
  - **每节课都有**  
- 大作业  
  - 多人合作  
  - 实现一个较为复杂的图像处理算法  
---

# 小作业提交格式:

按照作业提交示例.  

作业提交DDL,下一次实验课上课前一天的23:59分之前.

---
# 自我介绍
<br/><br/>
### **崔家梁**  

遥感专业2016硕,GIS班12本  
研究方向：图像、视频处理  
实验室：遥感楼505  
手机&微信：18811324609  
邮箱：cuijialiang@pku.edu.cn(作业提交到这)

---
# 问题？
### 之后请随时提问

---
# 遥感数字图像处理实验课
### - 1 图像处理基本操作
<br/><br/>
崔家梁
(cuijialiang@pku.edu.cn)  

---
# 位图文件(Bitmap)
**二进制文件**

常见的位图文件：BMP,PNG,GIF,TIFF...
编码方式：灰度图(黑白),RGB,CMYK...

![80%](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3b/Rgb-raster-image.svg/368px-Rgb-raster-image.svg.png)通常使用8位五符号整形存储

---
# 位图文件(Bitmap)
其实就是一个数组,**按顺序**对应所有像素.  
gray image:[v(0,0),v(0,1),v(0,2)...v(1,0)...]   
color image:[r(0,0),g(0,0),b(0,0),r(0,1),...]

![150%](http://www.scan2cad.com/wp-content/uploads/2016/09/how-bitmap-images-are-stored.png)

---
# 位图打开方式
#### 1.直接从二进制文件打开,读取元数据、数据数组
- 需要预先知道结构信息

**有兴趣的同学可以尝试一下**(不要求)

#### 2.利用已有的库(如pillow,opencv),直接打开到一个结构体
```
# python code
from PIL import Image
im_PIL = Image.open("../img/horse.jpeg")
im_PIL.show() #显示图片
```

---
# 操作演示
- 环境配置
  - 推荐工具:choco(windows)
  https://chocolatey.org/install
- jupyter notebook基本操作
  - pip(pip3) install jupyter
  http://jupyter.org/install.html
- Pillow与numpy处理图像操作
- opencv图像基本操作

---
# 作业1-图片的基本操作
#### 编程实现以下内容:
- 打开一张**彩色**图片;  
- 将其红蓝波段对调,得到假彩色合成结果并显示;  
- 将上一步得到的结果旋转45度并显示(选作);  
- 将最终得到的结果保存成文件. 
<br/>
请于2017年9月27日北京时间上午10点之前提交至 cuijialiang@pku.edu.cn,收到回复为准.