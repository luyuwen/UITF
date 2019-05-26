#8.2 数字音频

##8.2.1 数字音频基础知识

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;声音是由物体振动产生的，发生震动的物体称为声源，通过介质的传播可以被人耳所感知，但人耳只能识别20Hz~20kHz频率之间的声音。音调、响度和音色是声音的三个主要特征，音调是指声音的高低，由频率决定，频率越高音调就越高；响度是指声音的大小，也就是我们常说的音量，由振幅和人离声源的距离决定，振幅即物体震动时偏离原来位置的最大距离，振幅越大响度越大，人离声源越近响度也越大；音色又称为音品，与发声物体的材料、结构等有关，小提琴、吉他等乐器发出的声音，即使音调、响度都一样，但我们仍能分辨出来，这就是因为它们的音色不同。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;音频信号是一种连续的模拟信号，随着科技的发展，将模拟信号转化为数字信号成为可能，这一转化过程称为模数转换，如图8-17所示，主要包括采样、量化和编码等三个过程。

<div align="center"><img src="/images/8-17.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-17模数转化过程</p></div>
 
###1.采样

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;采样就是将音频信号在时间轴上离散化，每隔一个时间间隔都在连续的模拟信号上取一个幅度样本，这样就可以用离散的点表示出连续的模拟量，如图8-18所示。

<div align="center"><img src="/images/8-18.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-18 采样示意图</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;采样的时间间隔称为采样周期，一般用T来表示；每秒钟采样的次数称为采样频率，一般用f来表示，单位为赫兹（Hz），两者之间的关系为T=1/f。采样频率过低时，会出现低频失真现象，为避免这一现象，采样频率应等于或大于音频信号中最高频率的两倍。表8-2展示了一些常用的采样频率。

<div align="center"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">表8-2 常用的采样频率</p></div>

|采样频率|音质|
| :------: |:------: |
|8kHz|电话语音|
|11.025kHz|低品质音乐|
|22.05kHz|调频广播|
|44.1kHz|CD品质的音乐|
|48kHz|	数字电视、电影、专业音频等所用的数字声音|

###2.量化

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;连续的音频信号经过采样后成为离散信号，离散信号经过量化后成为数字信号。量化就是将采样后大量的信号幅度值用确定的有限位二进制数表示出来的过程。信号在量化过程中可能会出现误差，我们称其为量化噪声，量化等级越多，量化噪声就越小，如图8-19所示，16位量化明显比8位量化的精度要高，但同时16位量化生成的数字音频所占用的存储空间也相对较大。

<div align="center"><img src="/images/8-19.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-19 量化示意图</p></div>
 
###3.编码

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;编码就是将采样和量化后的数字音频数据按照一定的格式记录下来的过程。比特率是一个间接衡量音频文件质量的标准。在相同的编码格式下，比特率越大音质就越好，比特率的计算方式为:比特率=采样频率×量化位数×声道数。常见的编码方式有脉冲编码调制（Pulse Code Modulation，简称PCM）、MP3编码、OGG编码等。

###4.音频压縮

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;按照数据压缩前后是否有损失，可以将音频压缩分为无损压缩和有损压缩。无损压缩的压缩比较低，经过压缩重构后的数据与压缩前的数据完全相同；有损压缩的压缩比较高，经过压缩重构后的数据与压缩前的数据不同，但并不会因此影响原始数据的表达。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;音频信号可以被压缩是因为音频信号中存在信息冗余，主要有两种形式的信息冗余：时域冗余和频域冗余。时域冗余的表现形式有信号周期的相关性、声音信息中出现间隔、停顿等；频域冗余的表现形式有长时功率谱密度的非均匀性等。

###5.数字音频的文件格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;数字音频文件格式多种多样，通过互联网，我们可以下载自己需要的音频，目前，播放器大多都支持多种格式，此处简要介绍几种音频文件格式。

####（1）CD-DA格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CD-DA（Compact Disc-Digital Audio）又称激光数字唱盘，是CD中的音乐音频格式，对数据不进行压缩处理，因此占用存储空间相对较大。

####（2）WAVE格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;WAVE（Waveform Audio File Format）是经典的Windows多媒体音频格式，不经过压缩处理，编码、解码相对简单，声音质量很好，常用于多媒体开发音乐、原始音效素材等，但同时WAVE格式的文件需要的存储空间很大，对于有存储限制的应用而言，这是个重要的问题。

####（3）MP3格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MP3（Moving Picture Experts Group Audio Layer III）是一种有损压缩格式，利用了人耳对高频声音信号不敏感的特性，对不同频段采用不同的压缩率，使得音频文件体积小的同时音质也相对较好，MP3格式具有较高的压缩比，可以达到10:1甚至12:1，是目前应用较为广泛的音频格式之一。

####（4）RealAudio格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;RealAudio格式是RealNetworks公司开发的一种流式音频文件格式。这种格式在网络上颇为流行，主要用于网络上的流媒体传输、播放，并且可以根据网络带宽的不同改变声音的质量。

####（5）WMA格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;WMA（Windows Media Audio）是微软推荐的一种音频格式，采用有损压缩，具有较高的压缩比，一般可以达到18：1。WMA内置了版权保护技术，即使非法保存到了本地也无法收听，也可对播放时间、次数进行限制。

####（6）MIDI格式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MIDI（Musical Instrument Digital Interface）文件并不是一段录制好的声音，而是一段指令，用来告诉声卡如何再现音乐。目前主要用于流行歌曲的表演、游戏音轨以及电子贺卡等。

###6.数字音频的采集方式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;获取数字音频的途径多种多样，此处简单介绍几种常见的数字音频获取方式。

####（1）数字音频的录制

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;利用录音软件、麦克风等可以完成数字音频的录制，目前手机、计算机等多种数字设备都可以完成数字音频的录制。

####（2）网络资源获取

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;信息时代，很多人会以有偿或无偿的方式将自己的数字音频素材发布到互联网上，我们利用互联网可以得到大量的数字音频文件。

####（3）MIDI音乐生成

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;计算机可以与MIDI电子乐器相连，将MIDI电子乐器发出的指令保存到MIDI文件中。

####（4）其他音频设备输入

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过线路输入的方式可以将电视机、广播等提供的音频连接到计算机的声卡上，采集之后可以以数字化的形式存储在计算机中。

##8.2.2 Audition的常用操作

###1.音频处理软件

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;音频是一种重要资源，应用领域相当广泛，由于各种原因，录制好的声音需要经过后期的加工处理才可以达到客户或制作人的要求。音频处理软件是一类对音频进行混音、录制、淡入淡出等处理的软件，表8-3介绍了一些常见的音频处理软件。

<div align="center"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">表8-3 常见的音频处理软件</p></div>

|标志|工具名称|说明|
|:------:|:------:|:------:|
||Audition|Audition是一款专业的音频处理软件，具有录音、声音编辑、修复录制缺陷、声音混合等功能，并且支持WMA、MP3等多种主流音频格式。|
||GoldWave|GoldWave是一个集声音编辑、播放、录制和转换功能于一体的音频编辑软件，支持MP3、WMA、WAC等多种音频格式。|
||CakeWalk|CakeWalk是一款数字音乐制作软件，可以制作、编辑MIDI格式的音乐文件，同时还具有音频录制和常规的音频处理功能。|
||WaveCN|WaveCN是一款录音编辑软件，具有方便、易用的中文操作界面，支持多种音频格式，同时具有常用的音频编辑功能。|
||iFlyTech InterPhonic|iFlyTech InterPhonic是一款真人语音朗读软件，能够根据文本读出声音，导出声音文件，并且提供了不同风格的音色，如成年男声、成年女声以及童声等。|
||语言合成工具|语言合成工具是一款在线语音转换软件，具有安装版本和绿色版本，均是免费提供给用户使用。|
 
###2.Audition操作界面

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Audition有单轨迹编辑环境、多轨迹编辑环境、CD模式编辑环境等三种工作环境，单轨迹编辑环境比较适合处理单个的音频文件；多轨迹编辑环境可以对多个音频文件进行编辑；CD模式编辑环境可以整合音频文件并转化为CD音频。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;此处以Audition2018为例，介绍它的操作界面，图8-20是Audition2018的工作界面，最上面是菜单栏，包括文件、编辑、多轨混音、素材、效果等；最左边为素材选择区，我们可以在这里找到自己需要的音频素材；素材选择区右边为工作区和显示区，工作区用来对音频进行一系列操作，例如降噪、删除等；显示区可以显示音频的声音大小以及音频的起止、持续时间等。Audition的窗口布局较为自由，可以任意调整大小、位置等。

<div align="center"><img src="/images/8-20.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-20 Audition的主界面</p></div>
 
###3.Audition的常用操作

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Audition2018的功能很多，此处介绍几种常用操作。

####（1）声音的录制

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在计算机上插入麦克风并打开Audition后，单击菜单栏中的【文件】→【新建】→【新建音频文件】，会出现图8-21所示的对话框，在这里我们需要命名该文件，选择合适的采样率、声道、位深度并单击【确定】；然后单击编辑器上的<img src="/images/8-0-5.png">【录音】按钮便可通过麦克风进行录音，录音完毕，可以单击<img src="/images/8-0-6.png">【停止】按钮结東录音，编辑器如图8-22所示。

<div align="center"><img src="/images/8-21.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-21 新建音频文件</p></div>
 
<div align="center"><img src="/images/8-22.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-22 编辑器</p></div>
 
####（2）录制程序中的声音

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;我们首先打开所要运行的程序(如课件、游戏软件等)，并找到想要录制的内容；单击Audition菜单栏中的【编辑】→【首选项】→【音频硬件】，在“首选项”对话框中的【默认输入】下拉菜单中选择【立体声混音】并单击【确定】，如图8-23所示；最后单击编辑器中的【录音】按钮便可进行录制。

<div align="center"><img src="/images/8-23.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-23 设置音频硬件</p></div>
 
####（3）音频粗剪

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在声音素材的编辑过程中，有时需要删除一些空白或者错误的部分，有时需要把一部分声音文件粘贴到另一个位置。删除声音时，我们选中需要删除的部分，按下“Delete”键即可，复制粘贴文件时，选中需要复制的部分按下“Ctrl+C”，并在合适的位置按下“Ctrl+V”进行粘贴。

####（4）声音效果的处理

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;①降噪，在录制声音素材时，不可避免的会出现一些噪声，我们可以通过降噪来处理声音素材。首先将该声音文件的波形放大，直到能够清楚地看到该声音文件的低频噪声波形；选中该波段，单击【效果】→【降噪/恢复】→【降噪（处理）】，打开“效果-降噪”对话框，如图8-24所示，单击【捕捉噪声样本】，软件便会对噪声样本进行分析，之后单击【选择完整文件】，此时整个声音素材文件都会被选中，最后单击对话框中的<img src="/images/8-0-4.png">按钮，就可以试听降噪的效果了。如果觉得效果比较理想，单击【应用】按钮，即可完成降噪处理，如果觉得声音失真，可以调节【降噪】和【降噪幅度】来完善效果，如图8-25所示。

<div align="center"><img src="/images/8-24.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-24 降噪面板</p></div>

<div align="center"><img src="/images/8-25.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-25 降噪和降噪幅度的设置</p></div>
 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;②淡入淡出，通常我们会在声音开始和结束部分进行淡入淡出处理，使得声音的产生和消失不那么突兀。编辑音频文件时，在工作区的左上角和右上角分别有一个淡入标识和淡出标识，如图8-26所示。向右拖动左上角的淡入标识，可对声音素材进行淡入处理；向左拖动右上角的淡出标识，即可对声音素材进行淡出处理。

<div align="center"><img src="/images/8-26.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-26 淡入淡出标识</p></div>

####（5）音频的修复

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在录制声音素材的过程中，可能会混入一些杂音，例如电话铃声，上课铃声，此时我们就需要对声音进行修复。首先单击【显示频谱频率显示器】<img src="/images/8-0-1.png">，调出该声音素材的频谱图；之后单击【框选工具】<img src="/images/8-0-2.png">，对杂音部分进行框选，如图8-27所示，最后按下“Delete”键便可进行删除。对于框选不干净的部分，我们可以使用【套索选择工具】<img src="/images/8-0-3.png">，将需要删除的部分选出，并按“Delete”键进行清除。

<div align="center"><img src="/images/8-27.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-27 音频的框选</p></div>

####（6）声音的合成

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;背景音乐可以烘托气氛、酝酿情绪，在影视作品、游戏、动漫等领域应用广泛，利用Audition可以为音频添加背景音乐。首先单击【文件】→【新建】→【多轨会话】，为新建的多轨会话文件命名，并单击【确定】按钮，将需要添加背景音乐的音频素材拖到轨道1上，并根据素材的长度调整另一轨道上背景音乐的长度；通过上下拖动音量线条来调节音量，如图8-28所示，通过【淡入】、【淡出】标识对声音进行淡入、淡出处理，直到达到理想的效果；最后单击【文件】→【导出】→【多轨混音】→【整个文件】，打开“导出多轨混音”面板，选择需要的格式、位置，单击【确定】就可以得到所需的音频。

<div align="center"><img src="/images/8-28.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图8-28 通过音量线条调节音量</p></div>