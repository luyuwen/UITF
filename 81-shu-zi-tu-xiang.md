#8.1 数字图像

<div align="center"><iframe frameborder="0" width="640" height="498" src="https://v.qq.com/txp/iframe/player.html?vid=p0875fuemch" allowFullScreen="true"></iframe></div>
<div align="center"><p style="font-size:20px; font-weight:bold">教学微视频</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;数字图像又称数码图像，以数字的形式进行获取、处理、输出和保存，可以直观的表现信息，应用非常广泛。本节主要介绍数字图像的基础知识以及Photoshop的常用操作。

##8.1.1 数字图像的基础知识

###1.矢量图和位图

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;矢量图也叫向量图，它的元素，例如点、线、圆等，是通过数学公式获得的，如图8-1所示。矢量图的优点是文件小，图像轮廓易修改并且不管对图像进行怎样的缩放操作，不管按照何种分辨率打印，都不会影响图像的清晰度和细节展示，如图8-2所示；缺点是难以绘制色彩层次丰富的图片，并且绘制出的图像不是特别逼真。

<div align="center"><img src="/images/8-1.jpg"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-1 矢量图</p></div> 

<div align="center"><img src="/images/8-2-1.png"><img src="/images/8-2-2.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-2 矢量图原图像与放大图像对比</p></div>  

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;位图又称为像素图、点阵图，它的最小信息单元是像素，每个像素都具有特定的位置和颜色值。将位图图像放至最大，可以发现图片上出现了许多小方块，这些小方块就是像素，如图8-3所示。位图的优点是易于表现色彩层次丰富的图像，产生逼真的效果；缺点是放大到一定程度后图片会变得模糊，存储位图就是存储所有像素点的颜色数据等信息，因此位图存储占用的空间相对较大，一般情况下，为利于存储和传输，我们会对位图进行适当的压缩。

<div align="center"><img src="/images/8-3.jpg"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-3 位图原图像与放大图像对比</p></div> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;像素、分辨率和颜色深度是位图图像的三个基本要素。

####（1）像素

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;位图图像是由许多小方块组成的，这些小方块就是像素，它们在各自的位置记录着图片的颜色信息。一张图片的像素越多，图片的质量就越好，与此同时，图像所占的存储空间也就越大。
####（2）分辨率

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;分辨率可以分为显示分辨率和图像分辨率。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;显示分辨率是指显示器屏幕能够显示的像素量有多少，显示器可显示的像素越多，那么显示器显示的图像就越清晰细腻，如图8-4所示。显示分辨率的表达方式为“水平像素数×垂直像素数”，例如1024×768、1600×900。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;图像分辨率是指位图图像内存储的数据量，图像中的数据越多，那么图像就越细腻，细节就越清晰，同时图像所占的存储空间就越大。若图像包含的数据不够充分，图像看起来就比较粗糙，放大时可能会出现失真的状况。与显示分辨率的表示方式相同，图像分辨率也可以用“水平像素数×垂直像素数”进行表示，例如800×600；在平面设计中，分辨率的单位为像素每英寸（pixel per inch，ppi），因此也可用每英寸的像素个数以及图像的长宽进行表示，例如100ppi，16in×12in。

<div align="center"><img src="/images/8-4.jpg"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-4 不同分辨率的显示效果</p></div>

####（3）颜色深度

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在计算机中所有的信息都使用二进制表示，位图也不例外，颜色深度是指存储每个像素所用的二进制位数，简单来说就是最多可以显示多少种颜色。颜色深度为1的图像，可以包含21种颜色，即黑和白，这样的图像称为单色图像，如图8-5（a）所示；若图像的颜色深度为8，那么图像最多可以包含28种颜色；若图像的颜色深度为24，那么图像最多可以包含224种颜色，超过了人眼可以辨别的颜色数量，这样的图像称为真彩色图像，如图8-5（b）所示。

<div align="center"><img src="/images/8-5(a).png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">（a）</p><img src="/images/8-5(b).png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">（b）</p><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-5 单色图像与真彩色图像</p></div>  
               
###2.图像的文件格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;常见的矢量图像格式有CGM、SVG、WMF、DXF、U3D等；常见的位图图像格式有BMP、JPEG、PNG、TIFF等。此处简单介绍几个位图图像的文件格式。

####（1）BMP格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;BMP（Bitmap）是Windows系统中的标准图像文件格式，与设备无关，Windows中的所有图像处理软件都支持BMP格式，随着Windows的普及，BMP格式也广为人知，得到了广泛的应用。BMP格式的图像可以选择颜色深度，但不进行任何压缩，因此它所占用的存储空间相对较大。

####（2）JPEG格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;JPEG(Joint Photographic Expects Group)是一种常见的图片格式，文件扩展名为“.jpg”或“.jpeg”，它采用的压缩技术属于有损压缩，会将大量重复的部分或肉眼无法识别的部分删除，只保留重要的信息。目前，JPEG格式的图片在互联网上较为流行，它可以产生很高的压缩比，但对色彩信息保留较好，可以展示生动逼真的图像，但若压缩比过高，图像质量就会变差。

####（3）PNG格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PNG(Portable Network Graphics)是一种无损压缩的图片格式，由于体积小，常用于网页或JAVA程序中。PNG格式支持透明效果，可以使图像的边缘与任何背景平滑的融合在一起，而不会产生边缘锯齿。

####（4）TIFF格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TIFF（Tagged Image File Format）是一种可移植的图像格式，最初是由Aldus公司与微软公司一起开发出来的。TIFF不依赖具体的硬件，支持多种压缩方案和颜色模式，目前广泛应用于高质量图像的存储、输出和转换。

###3.数字图像的获取

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;获取数字图像的途径多种多样，此处简单介绍几种常见的数字图像获取方式。

####（1）利用制图软件创作

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;常见的制图软件有CorelDRAW、Painter、illustrator、Auto CAD等，利用这些制图软件可以制作出质量较高的图像。

####（2）通过数字设备获取

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过生活中我们常用的数字设备也可以获取数字图像，例如利用手机、数码相机的拍摄功能可以拍摄各种画面得到数字图像；也可以利用扫描仪将纸质图片的信息采集到计算机当中，获得数字图像。

####（3）屏幕抓图

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过一些专业抓图软件或键盘上的“PrintScreen”键可以对部分信息进行截图，得到数字图像。只按“PrintScreen”键是对整个屏幕进行截图，若同时按下“Alt”键和“PrintScree”键则是对当前窗口进行截图。

####（4）网络资源获取

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;互联网上存在着大量的数字图像，必要时，我们可以通过网络获取相关数字图像。

##8.1.2 Photoshop的常用操作

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;现实生活中，获取的数字图像往往不能直接使用，需要经过一定的处理才可以呈现在大众面前。数字图像处理是指将图像信号转为数字信号并对其进行修改的过程，表8-1展示了常见的图像处理软件，其中Adobe公司的Photoshop是目前使用较多、功能非常强大的图像处理软件，广泛应用在广告摄影、平面设计、网页制作等领域。此处主要介绍Photoshop软件。

<div align="center"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">表8-1 常见的图像处理软件</p></div>

|标志|工具名称|说明|
|:------:|:------:|:------:|
|<img src="/images/meitu.jpg">|美图秀秀|美图秀秀是一款简单易用的图片处理软件，具有人像美容、图片拼贴、添加图片边框和饰品等功能。|
|<img src="/images/ps.png">|Photoshop|Photoshop是Adobe公司开发的专业图像处理软件，具有图像编辑、图像合成、校色调色和特效制作等多种功能，深受平面设计者的喜爱。|
|<img src="/images/tpzhq.png">|图片转换器|图片转换器是一款图片格式转换软件，转换的同时还可以改变图片文件的大小、添加水印、添加边框等，它支持JPG、GIF、BMP、PNG等14种常见的文件格式。| 
|<img src="/images/hqt.png">|红蜻蜓抓图精灵|红蜻蜓抓图精灵是一款专业的屏幕捕捉软件，可以对捕获的图片进行简单的编辑处理，并且可以输出多种格式的图像，例如JPG、GIF、PNG、BMP等。|

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Photoshop|简称PS，支持多国语言，适用于Windows、Mac OS等操作系统，我们以Photoshop2018为例简单介绍一下Photoshop的工作界面和常用操作。

###1.Photoshop的工作界面

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Photoshop2018的界面可以分为六个区域，最上面的一栏为菜单栏，包括文件、编辑、图像、图层、文字、选择、滤镜等；菜单栏的下面一栏为选项栏，选项栏的内容会根据选择不同的工具而发生变化；最左边为工具箱，常用的工具几乎都在这里，例如移动工具、钢笔工具等；中间的区域为工作区域；工作区域右边为活动面板，里面比较常用的是图层面板、通道面板和路径面板；最右边为库面板，可以存储矢量图像、BMP位图文件、图层样式等；最下面一栏为状态栏，显示当前文档的大小、显示比例等。图8-6为Photoshop2018的整体视图。

<div align="center"><img src="/images/8-6.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-6 Photoshop2018的界面</p></div> 

###2.Photoshop的常用操作

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Photoshop的功能很多，此处不一一介绍，只介绍几种常用操作，例如图像色彩的调整校正、图像缺陷修补、图像合成、特效制作等。

####（1）图像色彩的调整校正

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;色彩调色是Photoshop中深具威力的功能之一，利用它可以方便快捷地对图像进行明暗、色彩的调整和校正，也可以调整颜色以满足图像在不同多媒体作品中的需求。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;①调整曝光，在PS中打开曝光过度的图像，此处为图8-7（a）为例，之后进行如下处理，在菜单栏中打开【图像】→【调整】→【色阶】，然后适当调整色阶中的黑场即可。图8-7（b）为图片调整前后的对比效果。

<div align="center"><img src="/images/8-7.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-7 曝光调整前后的对比图</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;②调整色调，在PS中打开图8-8（a），在菜单栏中打开【图像】→【调整】→【曲线】，适当调整曲线即可，图8-8（b）为色调调整前后的对比图。

 <div align="center"><img src="/images/8-8.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-8 色调调整前后的对比图</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;③校正偏色，在拍摄过程中，由于光线或角度问题，可能会出现偏色，图8-9（a）就是一张出现偏色问题的图片。处理偏色时，可以在菜单栏中打开【图像】→【调整】→【色相/饱和度】，进行适当的调整即可，图8-9（b）为偏色校正前后的对比图。 

<div align="center"><img src="/images/8-9.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-9 偏色校正前后的对比图</p></div>

####（2）图像缺陷修补

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;现实生活中，很多拍摄好的原图会存在一些令人不满意的地方，利用PS，我们可以修补原图的缺陷或残损，使得图片更加完美。观察图8-10（a）可以发现，图片右下角有一片光秃秃的土地，但它的周围都是绿油油的小草，我们可以利用修补工具或修复画笔工具等对土地进行修复，便可得到图8-10（b）的效果。

<div align="center"><img src="/images/8-10.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-10 缺陷修补前后的对比图</p></div>

####（3）图像合成

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;图像合成可以将几幅图片上的内容融为一体，产生“以假乱真”的效果。此处介绍两种图像合成的方法。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;①利用抠图合成图像，这种方法就是将我们需要的物体“抠下”，然后放到另一个背景当中，如图8-11所示。抠图时我们可以选择【快速选择工具】和【魔棒工具】，这两个工具适合选择大面积且颜色单一的区域，图8-11（a）的背景颜色就较为单一，我们可以先选中背景，然后按下“Ctrl+Shift+I”就可以反选出图中的玉石，最后移到另一个背景当中即可，如图8-11（b）所示。当背景颜色较为复杂时，我们可以选用【钢笔工具】沿着主体的边缘进行勾勒，勾勒完成后，在活动面板中找到我们刚刚勾勒的工作路径，如图8-12所示，按下“Ctrl”键同时点击路径缩略图，就将我们勾勒出的路径区域转换为了选区，最后将选区移到另一个背景当中即可。

<div align="center"><img src="/images/8-11.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-11 图像合成前后的对比图</p></div> 

<div align="center"><img src="/images/8-12.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-12 工作路径</p></div> 


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;②利用图层蒙版合成图像，除了上述的给主体换背景，还可以将两张风景图融为一体，制作出一种全新的风景。此处以图8-13的素材图为例，首先我们将图8-13（a）与图8-13（b）分别放在图层1和图层0当中；在图层1上，我们选中【图层】→【图层蒙版】→【隐藏全部】，这时，图层1图片的右边会出现一个黑色矩形，如图8-14所示；接下来我们选择【橡皮擦工具】，在合适的位置涂抹即可。最终效果如图8-15所示。

<div align="center"><img src="/images/8-13(a).jpg"><p>（a）</p><img src="/images/8-13(b).jpg"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">（b）</p><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-13 素材图</p></div>
            
<div align="center"><img src="/images/8-14.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-14 图层蒙版</p></div> 

<div align="center"><img src="/images/8-15.jpg"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-15 图片合成</p></div> 

####（4）特效制作

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;特效制作可以使静态的图片呈现出动感，我们以图8-16（a）为例，首先选中需要添加滤镜的区域，即运动员以外的区域，然后选择【滤镜】→【模糊】→【动感模糊】，调整合适的距离即可，最终效果如图8-16（b）所示。

<div align="center"><img src="/images/8-16.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-16 添加滤镜的前后对比图</p></div>