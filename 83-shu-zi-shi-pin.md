#8.3 数字视频

<div align="center"><iframe frameborder="0" width="640" height="498" src="https://v.qq.com/txp/iframe/player.html?vid=m0875caq7ya" allowFullScreen="true"></iframe></div>
<div align="center"><p style="font-size:20px; font-weight:bold">教学微视频</p></div>

##8.3.1 数字视频的基础知识

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;数字视频是指在视频信号的产生、存储、处理、重放、传送等过程中均采用数字信号。与它相对的是模拟视频，即在视频信号的产生、存储、处理、重放、传送等过程中均采用模拟信号。相比于模拟视频，数字视频的抗干扰性更好，更适合长时间存放，大量复制时不会产生图像失真、信号损失等问题。

###1.数字视频的压缩

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;视频压缩的目标是在尽可能保证视觉效果的前提下减少视频的大小。视频信号可以被压缩是因为存在信息冗余，视频信号的信息冗余主要有空间冗余、结构冗余、时间冗余、视觉冗余、知识冗余、信息熵冗余等。压缩技术就是将数据中的冗余信息去掉，即去除数据之间的相关性。本章第二节介绍了有损压缩和无损压缩，数字视频压缩按照其他的标准还有不同的分类。

####（1）帧内压缩和帧间压缩

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;视频信号是由一帧一帧的图像组成的，按照压缩帧内数据还是压缩帧间数据可以分为帧内压缩和帧间压缩。帧内压缩实际上类似于静态图像压缩，压缩时不考虑帧间信息冗余，仅考虑帧内的信息冗余，一般达不到较高的压缩比；一般情况下，视频中连续两帧的图像信息变化很小，例如主体发生轻微变化但背景没有变化，这样的两帧相关性就很强，存在大量的冗余信息，帧间压缩就是根据这一特性来压缩帧间的信息冗余，这样可以大大减少数据量。

####（2）对称和不对称压缩

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;按照压缩和解压缩占用的计算处理能力和时间是否相同可以分为对称压缩和不对称压缩。对称压缩是指压缩和解压缩占用相同的计算处理能力和时间，适合实时压缩和视频传送；不对称压缩是指压缩和解压缩时占用的计算处理能力和时间不同，一般情况下压缩时需要花费大量的处理能力和时间，解压缩时需要的时间较少，可以较好地实时回放。

###2.数字视频的文件格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;常用的数字视频文件格式非常多，了解每个视频文件格式的特点是非常有必要的，此处简单介绍几种数字视频文件格式。

####（1）MPEG格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MPEG（Moving Picture Experts Group）是运动图像压缩算法的国际标准，采用有损压缩的方式减少信息冗余，主要包括MPEG-1、MPEG-2、MPEG-4、MPEG-7及MPEG-21等五种类型。其中，MPEG-1格式就是VCD制作格式，主要解决多媒体的存储问题；MPEG-2格式主要应用在DVD的压缩；MPEG-4格式强调多媒体系统的灵活性、交互性，主要用于播放高质量的视频流媒体；MPEG-7格式的目的是生成一种用来描述多媒体内容的标准；MPEG-21格式的目的是理解如何将不同的技术和标准结合在一起。

####（2）AVI格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;AVI（Audio Video Interleaved）是由微软公司推出的，将视音频信号交错记录的数字视频文件格式，允许视频、音频同步回放，图像质量较好，常用于多媒体光盘保存电影、电视等各种影像信息。

####（3）WMV格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;WMV（Windows Media Video）是由微软推出的，可以在网上实时观看视频的文件压缩格式。一般情况下，WMV文件包含视频和音频，编码时，部分视频使用Windows Media Video，部分音频使用Windows Media Audio。

####（4）MOV格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MOV（QuickTime Movie）由Apple公司开发，是QuickTime的影片格式，具有跨平台、压缩比高等特点，无论是本地播放还是作为视频流格式在网上传播，MOV都是一种较好的选择。

####（5）ASF格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ASF（Advanced Streaming Format）是微软公司Window Media的核心，属于高压缩率的文件格式，体积非常小，适用于本地或网络回放，图像、音频、视频等多媒体信息都可以以ASF格式进行网络传输。

####（6）FLV格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;FLV（Flash Video）格式是随着Flash的发展而出现的视频格式，它形成的文件极小、加载速度极快，适合流式传输和播放，目前广泛应用于各在线视频网站。

####（7）RM格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;RM格式由RealNetworks公司开发的，是一种可以根据网络数据传输速率来制定压缩比的流媒体视频文件格式，主要包含RealAudio、RealVideo和RealFlash三部分。

####（8）RMVB格式

RMVB（RealMedia Variable Bitrate）是RealMedia格式的扩展版本，RMVB降低了静态画面下的比特率，拥有出色的画质和众多优秀软件的支持，例如Easy RealMedia Producer。

###3.数字视频的获取方式：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;目前，我们接触到的大量视频都是数字视频，获取数字视频的途径多种多样，此处简单介绍几种常见的数字视频获取方式。

####（1）利用相关设备拍摄

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;随着数字产品的普及，我们对手机、数字摄像机等设备已不再陌生，通过手机、数字摄像机等我们可以拍摄视频，最终得到满意的数字视频。

####（2）通过制作软件获取

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;目前，制作动画的软件已非常繁多且发展成熟，例如Flash、3D Studio Max 等，利用这些软件，我们可以制作出数字视频素材。
####（3）通过互联网获取

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过互联网，我们不仅可以下载图片、音频，还可以下载视频，目前大多网站都提供了视频下载服务，这种途径也可以帮助我们获得数字视频，但部分视频需要付费后才可下载。
####（4）将模拟视频转为数字视频

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;利用视频采集卡我们可以将模拟视频转换成数字视频。视频采集卡对模拟信号进行处理后交由计算机记录编码，但这种方法会损失一定的信号。
####（5）利用抓取软件录制

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;利用视频抓取软件从播放器的视频中抓取需要的视频信息也可以得到数字视频，不过抓取的视频清晰度较原视频可能会比较低。
##8.3.2 使用CS录制微视频
###1.视频处理软件

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;数字视频的处理主要有视频剪辑、配音、添加字幕、添加滤镜等。表8-4介绍了一些常用的视频处理软件，每种软件的功能侧重有所不同，用户可以根据自己的需要进行选择。

<div align="center"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">表8-4 常用的视频处理软</p></div>

|标志|工具名称|说明|
| :------: | :------: | :------: |
|<img src="/images/cs.png">|Camtasia|Camtasia是一款小巧灵活的录屏软件。界面精致、操作简单，可以轻松地记录屏幕动作，例如影像、鼠标移动轨迹、音效等，除此之外还具备视频编辑的基本功能。|
|<img src="/images/gsgc.jpg">|格式工厂|格式工厂是一款多媒体文件格式转换软件，支持多种主流多媒体文件格式的转换，如MP4、AVI、FLV、WMV等。同时还具有视频旋转、改变播放速率等视频编辑功能。|
|<img src="/images/mm.jpg">|Movie Maker|Movie Maker是入门级的视频剪辑软件，功能比较简单，适合家用摄像后的一些小规模的处理。|
|<img src="/images/pr.png">|Premiere|Premiere是一款专业的视频编辑软件，功能强大，易学易用，广泛应用于广告制作、电影剪辑等领域。|
|<img src="/images/hshy.png">|会声会影|会声会影是常用的视频制作和剪辑软件，与Premiere等专业的视频剪辑软件相比，操作更为简单。|
|<img src="/images/ai.png">|爱剪辑|爱剪辑是一款国产视频剪辑软件，操作方便简单，功能强大，画质好，稳定性高。|
|<img src="/images/ave.png">|AVS Video Editor|AVS Video Editor是一款类似于会声会影的视频编辑软件，可以将影片、图片、声音等素材合成输出为视频文件，并为其添加丰富的特效、过渡、场景效果等。 |

###2.CS的工作界面介绍

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;此处以Camtasia Studio9.1为例，介绍它的操作界面，图8-29是Camtasia Studio9.1的工作界面。最上面是菜单栏，包括文件、编辑、视图、分享、帮助等；最左边为功能编辑区，在这里可以添加标注、设置光标效果、设置转场效果等；功能编辑区右边是视频预览区，可以查看实时的编辑效果；最下面为视频编辑时间轴，主要用来执行对视频、声音、字幕的裁剪、拼接等操作。

<div align="center"><img src="/images/8-29.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-29 Camtasia Studio的主界面</p></div> 

###3.Camtasia Studio的常用操作

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Camtasia Studio的功能强大，此处只介绍几个常用的功能。

####（1）屏幕的录制

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;录制视频一般有三种方式，第一种方式是从软件打开后跳出的对话框中选择录制，如图8-30所示；第二种方式是进入主界面，点击【Record】按钮；第三种方式是按下录制的快捷键“Ctrl+R”。准备录制时会出现如图8-31所示的录制面板，点击最右边的【rec】便可开始录制，录制面板中常用的设置有【Select area】和【Recorded inputs】，在【Select area】中，我们可以选择全屏录制或自定义录制窗口的大小，在【Recorded inputs】中可以设置是否记录摄像头的拍摄，是否记录系统音频或麦克风音频等。屏幕录制阶段，我们可以在控制窗口看到录制时间，也可以通过【Delete】、【Pause】、【Stop】按钮对屏幕录制进行删除、暂停和停止操作，如图8-32所示。

<div align="center"><img src="/images/8-30.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-30 选择录制</p></div> 

<div align="center"><img src="/images/8-31.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-31 录制面板</p></div> 
 
<div align="center"><img src="/images/8-32.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-32 控制窗口</p></div>

####（2）视频的编辑

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;屏幕录制完后点击【Stop】，录制的视频便会自动导入Camtasia Studio，我们也可以将需要编辑的视频导入。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;①视频粗剪，如果部分视频是多余的或者不需要的，可以拖动时间轴上的绿色和红色光标进行选择，如图8-33所示，右击选择删除便可清除这一段视频。也可利用时间轴上方的操作按钮执行相应的操作，其中 按钮为返回上一步， 按钮为返回下一步， 按钮为剪切， 按钮为复制， 按钮为粘贴， 按钮为分离，可以将一段视频“切”成多段。

<div align="center"><img src="/images/8-33.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-33 视频粗剪</p></div> 


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;②添加标注，点击【Annotations】可以看到各种样式的标注，如图8-34所示，选择要添加的标注拖动至预览区，并在时间线上拖动以修改标注出现的时间及持续时间。

<div align="center"><img src="/images/8-34.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-34 添加标注</p></div> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;③添加片头，点击【Media】→【Library】可以使用软件自带的素材给视频添加片头，如图8-35所示

<div align="center"><img src="/images/8-35.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-35 添加片头</p></div> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;④添加光标效果，点击【Cursor Effects】，可以选择合适的光标效果、左击效果、右击效果等，如图8-36所示。

<div align="center"><img src="/images/8-36-1.png"><img src="/images/8-36-2.png"><img src="/images/8-36-3.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-36 光标效果</p></div>   

####（3）视频的导出

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;视频编辑好之后，选择【Share】→【Local File】，会出现如图8-37（a）所示的对话框，我们可以根据实际需求设置导出视频的参数。在这里，我们选择【Custom production settings】；点击下一步后出现如图8-37（b）所示的对话框，选择需要的视频格式；点击下一步后出现如图8-37（c）所示的对话框，我们可以对控制条、视频设置、音频设置进行相应的选择，当然设置的视音频品质越高，视频文件也越大；点击下一步后出现如图8-37（d）所示的对话框，这里我们一般不做更改，点击下一步出现如图8-37（e）所示的对话框，在这里我们对视频文件命名并选择保存路径即可完成视频的导出。

<div align="center"><img src="/images/8-37(a).png"><img src="/images/8-37(b).png"><img src="/images/8-37(cd).png"><img src="/images/8-37(d).png"><img src="/images/8-37(e).png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-37视频导出向导</p></div>