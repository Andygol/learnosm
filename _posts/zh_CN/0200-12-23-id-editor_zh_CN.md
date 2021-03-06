---
layout: doc
title: iD编辑器
permalink: /zh_CN/beginner/id-editor/
lang: zh_CN
category: beginner
---

iD编辑器
=============


- TOC
{:toc}

iD编辑器是基于浏览器的事实标准OpenStreetMap编辑器。iD编辑器快速、易用，可以借助来自诸如卫星或航空影像、GPS、Field Papers或Mapillary等多种数据源的数据绘图。

在一些不需要JOSM(一个更进阶的地图编辑器)的高级功能的微小改动中，使用ID编辑器是个更好的方法。本章阐述使用iD编辑器编辑的一些基础知识。 

启动iD编辑器
----------------------
-  iD编辑器需要持续有效的互联网连接。
-  打开浏览器，前往OpenStreetMap网站 [http://www.openstreetmap.org](http://www.openstreetmap.org)。
-  用你的OpenStreetMap账户**登录**
-  将地图平移并缩放到想要编辑的区域。平移的方法是按住鼠标左键，拖动到想要的区域。  
-  点击**编辑**旁边的小箭头，然后点击 **使用iD (浏览器内编辑器) 编辑**。

![image1][]


iD编辑器用户界面
-------------------------
![image2][]

1. **编辑要素面板:** 该面板显示图中所选对象的标签。你可以在该面板上添加或编辑标签。 
2. **工具:** 该面板显示基本的编辑工具： 
	- 画点(节点, node)，*快捷键* **1**  
 	![image3][]  


	- 画线(路径,way)， *快捷键* **2**  
 	![image4][]  


 	- 画面(多边形polygon)， *快捷键* **3**  
 	![image5][]  


 	- 撤销， *快捷键* **Ctrl+Z**   
 	![image6][]

 	- 重做，*快捷键* **Ctrl+Y**   
 	![image7][]  


 	- 保存修改, *快捷键* **Ctrl+S**   
 	![image8][]  



3. **地图面板:** 该面板显示各配置功能：
  	- 放大， *快捷键* **+**   
 	![image9][]  


 	- 缩小， *快捷键* **-**   
 	![image10][]  


 	- 显示我的位置
 	![image11][]  


 	- 配置底图图层， *快捷键* **B**   
 	![image12][]

 	- 地图数据， *快捷键* **F**   
 	![Map Data][]  


 	- 帮助， *快捷键* **H**   
 	![image13][]  



4. **信息面板:** 该面板显示一些信息，例如比例尺、向此地图贡献过的用户。 

配置底图图层
--------------------------------
开始编辑前，要先修改底图图层。

-  点击**背景设置**按钮或按下*快捷键* **B**。
![image14][]  


-  你会看到如下面板：
![image15][]  

 
-  你可以通过点击这些方框中的一个来调整**亮度等级**：
![image16][]  

-  有4种不同的亮度级别——100%、75%、50%、25%。逐个点击看看它们的差异。
-  你还可以根据自己喜爱的瓦片提供者来**修改底图图层**（默认是必应航空影像）。可以从以下列表中尝试不同的选项。
-  可以通过点击**自定义**按钮添加自定义瓦片底图。
-  例如，你要**添加一张Field Paper**作为底图，可以点击**自定义**然后点击放大镜(搜索) 图标打开如下窗口：-  
![image17][]

然后输入你的**FieldPaper快照网址**，形式大致如下： <http://fieldpapers.org/snapshot.php?id=cqhmf2v9#18/37.80593/-122.22715>  



-  你可以**显示本地计算机的GPS轨迹**(GPX格式)。也可以将GPX文件拖曳并放入iD编辑器。
-  你可以打开**OpenStreetMap GPS轨迹**图层，这样可以显示此地区的公共GPS轨迹。在下面的图片中，公共GPS轨迹用不同颜色表示，颜色代表着运行的方向。

![osm gps traces][]

-  如果有[影像偏移](/zh/josm/aerial-imagery)，你可以通过点击修复对齐来**纠正影像偏移**。
![image18][]  


- 点击方向按钮可以移动影像，点击重置按钮可以恢复到默认位置。  
![image20][]  


iD基本编辑操作
----------------------
现在我们来联系使用iD编辑器。

### 添加点
-  要添加一个新点，点击**点**按钮。

![image3][]

-  你的鼠标指针将变成一个加(+)号。现在，点击一个你知道的地点标出其位置。例如，你知道你附近有个医院，那就在医院大楼的位置点击鼠标。

![image21][]

-  这是一个新的点已经被添加。与此同时，左侧面板会变成一个表单，里边可以选择对象的属性。点击**医院**把该点标记为医院。

![image22][]

-  你可以在表单中填写所画地点的详细信息，例如医院名称、地址和其他附加信息。注意每类要素都有不同的选项，这取决于你从要素面板给地物选择的标签。 
-  如果你标错了，比如位置放偏了，可以通过在你的点上按住鼠标左键并拖动来移动其位置。如果是想删除你的点，就在你的点上点击鼠标左键然后再点类似于垃圾箱的按钮。

![image23][]

在iD编辑器中创建的“点”实际上是一个有一系列“标签”的独立“节点(node)”。

### 画线
-  要添加新的线，点击**线**按钮。

![image4][]

-  你的鼠标指针将变成加(+)号。在地图上找一条还没被画过的道路描绘出来。在路段开始的地方点击鼠标画一个点，移动鼠标并通过点击添加其他关键点，通过双击结束画线。注意左侧的面板。

![image24][]

-  和画点时一样，画完线后也要给线选择合适的标签。
-  你可以通过在已有点上点击鼠标左键来选中并拖动它。
-  你还可以移动整条线。先选中整条线，然后选择**移动工具**，最后把线拖动到新位置。

![image30][]

-  当你在线上的单个节点(node)上点击鼠标左键时，会有如下工具： 

	- 从线中删除点
	![image23][]
	- 从线中断开点
	![image26][]
	- 从选中点处将该线打断成两条
	![image27][]

-  当你在线上(注意不是在某个点上)点击鼠标左键时，会有如下工具：

	- 删除线
	![image23][]
	- 将线调整为圆形(仅当线是封闭的时可用)
	![image29][]
	- 移动线
	![image30][]{: height="24px"}
	- 将线调整为方形(仅当线是封闭的时可用)
	![image31][]
	- 反转线的方向(用于河流和单行道)
	![image32][]

在iD编辑器中创建的“线”实际上是一个有一系列“标签”的“路径(way)”。

> 关于**删除**的特别说明：一般情况下你不应该删除别人的线，如果你只是要改进这条线的话。你可以删除自己画错的内容，但是对于已由别人绘制但需要改动的对象，你应该尽量*调整*。这样做可以在OSM数据库中保留对象的历史记录，体现出对绘图伙伴的尊重。如果你确实认为该删，可以考虑先征求原作者意见，或者在OSM邮件列表中询问大家。

### 画面(多边形)
-  要添加新的多边形，点击**面**按钮。

![image34][]

-  你的鼠标指针会变成一个加(+)号。试着以影像为参照勾绘一栋建筑。
-  你会发现你的面的颜色将随你给它指定的属性而变化。

![image35][]

-  当你选中一个面时可用的工具和线的工具差不多。

在iD编辑器中创建的“多边形”实际上是一个有标签的“封闭路径(closed way)”。

保存你的更改
--------------------
-  当你想把你的编辑保存到OpenStreetMap时，请点击**保存**
	按钮。左侧的面板会显示上传面板。

![image36][]

-  输入对你编辑的注释并点击**保存**。


附加信息与自定义标签
---------------------------------------
-  当你在编辑一个对象时，你会看到属性面板底部有一条图标。你可以通过点击这些图标添加附加信息：

	- 添加高程
 	![image37][]
 	- 添加注释
 	![image38][]
 	- 添加联系方式或电话号码
 	![image39][]
 	- 添加来源标签
 	![image40][]
 	- 添加网站
 	![image41][]
 	- 添加残疾人可达性信息(轮椅通道)
 	![image42][]
 	- 添加维基百科链接
 	![image43][]

-  或者通过点击**所有标签**添加自定义标签。

![image44][]

-  这里会显示所有添加到要素的标签。

![image45][]

-  点击加号(+)添加键值对，点击垃圾桶图标删除标签。

iD vs. JOSM 对比
---------------
iD适用于…… 

-  简单编辑  
-  网速快时加载影像和保存编辑  
-  想要遵从简单一致的标签模式  
-  正在使用的计算机安装程序受限

JOSM更适于…… 

-  添加大量建筑物(参见buildings_tool插件)
-  编辑大量已经存在的线或面
-  网络连接不稳定或无网络时
-  使用特定标签模式或自定义预设组合


[image1]: /images/beginner/id-editor_image1.png
[image2]: /images/beginner/id-editor_image2.png
[image3]: /images/beginner/id-editor_image3.png
[image4]: /images/beginner/id-editor_image4.png
[image5]: /images/beginner/id-editor_image5.png
[image6]: /images/beginner/id-editor_image6.png
[image7]: /images/beginner/id-editor_image7.png
[image8]: /images/beginner/id-editor_image8.png
[image9]: /images/beginner/id-editor_image9.png
[image10]: /images/beginner/id-editor_image10.png
[image11]: /images/beginner/id-editor_image11.png
[image12]: /images/beginner/id-editor_image12.png
[Map Data]: /images/beginner/id-editor_map_data.png
[image13]: /images/beginner/id-editor_image13.png
[image14]: /images/beginner/id-editor_image14.png
[image15]: /images/beginner/id-editor_image15.png
[image16]: /images/beginner/id-editor_image16.png
[image17]: /images/beginner/id-editor_image17.png
[image18]: /images/beginner/id-editor_image18.png
[image19]: /images/beginner/id-editor_image19.png
[image20]: /images/beginner/id-editor_image20.png
[image21]: /images/beginner/id-editor_image21.png
[image22]: /images/beginner/id-editor_image22.png
[image23]: /images/beginner/id-editor_image23.png
[image24]: /images/beginner/id-editor_image24.png
[image25]: /images/beginner/id-editor_image25.png
[image26]: /images/beginner/id-editor_image26.png
[image27]: /images/beginner/id-editor_image27.png
[image28]: /images/beginner/id-editor_image28.png
[image29]: /images/beginner/id-editor_image29.png
[image30]: /images/beginner/id-editor_image30.png
[image31]: /images/beginner/id-editor_image31.png
[image32]: /images/beginner/id-editor_image32.png
[image33]: /images/beginner/id-editor_image33.png
[image34]: /images/beginner/id-editor_image34.png
[image35]: /images/beginner/id-editor_image35.png
[image36]: /images/beginner/id-editor_image36.png
[image37]: /images/beginner/id-editor_image37.png
[image38]: /images/beginner/id-editor_image38.png
[image39]: /images/beginner/id-editor_image39.png
[image40]: /images/beginner/id-editor_image40.png
[image41]: /images/beginner/id-editor_image41.png
[image42]: /images/beginner/id-editor_image42.png
[image43]: /images/beginner/id-editor_image43.png
[image44]: /images/beginner/id-editor_image44.png
[image45]: /images/beginner/id-editor_image45.png
[osm gps traces]: /images/beginner/id-editor_gps_public.png
