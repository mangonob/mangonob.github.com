---
layout: post
title:  "使用Sketch绘制svg图标"
date:   2016-02-21 23:45 +0800

thumb: https://raw.githubusercontent.com/mangonob/image/master/src/thumb/2016-02-21-sketch-banner.png

img: https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-sketch-banner.png

categories: jekyll update
---

![图片]({{ page.img }})


## 本文是一篇OSX使用Sketch绘制一枚svg格式的Github矢量图标的教程，
* 关于Sketch：Sketch是OSX平台下为人称道的轻量级的设计工具，相对于**Adobe**公司出品的两款软件———针对平面设计的Photoshop，以及矢量插画软件Adobe illustrator，Sketch拥有更为清新的界面；更主要的是对于现代交互设计更为专注，更具有针对性的功能，希望通过这篇教程能让没接触过Sketch的读者对它有更多的了解。
* 闲话少说教程开始
	1. 首先没安装Sketch的可以先去[官网](http://www.sketchapp.com/)下载安装，安装过程很简单，不再赘述。软件图标是一个土豪金的钻石，不要弄错哟！
	2. 打开软件我们可以看到软件的主界面主要分为四个区域，位于顶部的工具栏，中央最大的工作区域，左侧的边栏可以以列表的形式选择对象，右侧的边栏可以进行设置对象的属性等工作，我们最多的拖移，绘制动作发生在中央的工作区当中。
	![][img1]
	3. 点击工具栏最左边的“＋”号，展开列表中选择“Shape”->"Oval"，添加一个椭圆，用鼠标单击选中这个椭圆，再到右边栏中设置属性，设置Width，Height相等，成为一个圆形，返回到工作区，按住Shift键的同时，拖动对象四角的铆点，可以保持横纵比例的情况下对其进行大小的调整，有过photoshop使用经验的话这一点应该不陌生，调整到合适的大小就可以了（因为是矢量图，其实大小都无所谓，不过方便我们操作，调整到一个合适的大小是有必要的）
	![][img2]
	![][img3]
	![][img4]
	4. 同样的点击左上角的“＋”，这次我们添加一个“Verctor”，使用“钢笔工具”绘制出github的小章鱼的左半边身子，为了避免干扰，可以在左边栏，点击第3步中添加的椭圆右边的小眼睛，就可以将其隐藏，当我们处理的图像太多时，使用这种方式避免干扰是很基本的技巧，好了现在选中绘制的Verctor，然后按快捷键Cmd+C，Cmd＋V，复制粘贴一份，点选路径的副本，在右边栏找出Flip选项，第一个像一个风帆的就是水平镜像按钮，点击它，副本就翻转过来了。
	![][img5]
	![][img6]
	![][img7]	
	5. 按住Shift在工作区中先后选中两个路径就可以进行多选，选中的对象会呈现蓝色的边框，然后在顶部的工具栏找到集合运算（Union合并，Subtract减去，Intersect交集，Difference差分），点击其中的Union合并两个路径，这样我们就得到了一支完整的章鱼猫（之所以合并两部分而不是直接绘制，是因为人工绘制难免有误差，不可能保证两边对称，使用翻转的方式更为妥当）
	![][img8]
	![][img9]
	6. 上一步用到了Union的集合操作，这次我们用另外一个，Subtract也就是减去操作，点击小眼睛把椭圆显示出来，选取椭圆和第五步得到的联合路径，进行减去操作后得到一个“挖空了一部分的椭圆”，这样大体上的绘制过程就完成了。
	![][img10]
	![][img11]
	7. 接下来基本是，同样的操作，添加一个Vector，绘制出章鱼爪的形状，然后跟不完整的椭圆做减去操作，会得到最终我们想要的形状。
	![][img12]
	![][img13]
	8. 最后一步导出动作，需选中最后得到的图形，然后点击界面右上角的export按钮，在右边栏会出现相关的项目，选择格式svg，然后点击下面的“Export 文件名”的按钮即可完成导出，最终得到想要的svg图标
	![asdf][img14]
	9. 那么说了半天，svg究竟是啥呢！？，svg是万维网联盟公布的一套矢量图形标准，全称是——可伸缩矢量图形 (Scalable Vector Graphics)，说多了都是泪，不如用文本编辑器打开看看吧！～～
	
	

	





[img1]:https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-img1.png
[img2]:https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-img2.png
[img3]:https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-img3.png
[img4]:https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-img4.png
[img5]:https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-img5.png
[img6]:https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-img6.png
[img7]:https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-img7.png
[img8]:https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-img8.png
[img9]:https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-img9.png
[img10]:https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-img10.png
[img11]:https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-img11.png
[img12]:https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-img12.png
[img13]:https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-img13.png
[img14]:https://raw.githubusercontent.com/mangonob/image/master/src/2016-02-21-img14.png

