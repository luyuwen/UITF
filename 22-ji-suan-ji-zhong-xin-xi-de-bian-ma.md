#2.2 计算机中信息的编码

<div align="center"><iframe frameborder="0" width="640" height="498" src="https://v.qq.com/txp/iframe/player.html?vid=c087018hhsg" allowFullScreen="true"></iframe></div>
<div align="center"><p style="font-size:20px; font-weight:bold">教学微视频</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在计算机中，各种信息都是以二进制编码的形式存在的。也就是说，不管是文字、数字、图形、音频、动画，还是电影等信息，在计算机中都是以0和1组成的二进制代码表示的，此处介绍计算机怎样利用1和0进行信息的编码。

##2.2.1计算机中数值数据的编码

###1.数值的表示

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;生活中很多应用场合，只需正数的表达，如表示年龄、身高。但在绝大多数应用中，我们既需要考虑数的值，也要考虑数的符号，才能正确处理问题。所以，在计算机中，将只需要表示值的数据称为无符号数；将需要同时表示值和符号的数称为带符号数。表示无符号数时，所有的二进制位都可用来表示数的值。表示带符号数时，我们取二进制位的最高位来表示数的符号，其他位表示数的值。最高位为“0”表示正数，反之表示负数。符号和数一起进行存储和运算，如果用一个字节存储表示带符号的整数，则最高位为符号位，具体表示数值的只有7位，其最小数为（1111111）<sub style="font-size:10px">2</sub>=（-127）<sub style="font-size:10px">10</sub>，最大数为（01111111）<sub style="font-size:10px">2</sub>=（+127）<sub style="font-size:10px">10</sub>。例如，用八位二进制数表示+50和-50，分别为(00110010)<sub style="font-size:10px">2</sub>和(10110010)<sub style="font-size:10px">2</sub>。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;我们把用“0”和“1”表示符号的数称为机器数，将其所表示的带有正负号的实际数值称为真值。例如，机器数10000111的真值为-0000111。

###2.常见的编码方式

####（1）原码

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;原码是一种机器数表示方式，若用一个字节存储,则需要补满8位,若用两个字节存储,则需要补满16位长度……以此类推；例如，78如用一个字节存储，则其原码为(01001110)<sub style="font-size:10px">2</sub>，－78的原码为(11001110)<sub style="font-size:10px">2</sub>。细心的同学可能会想到，一个正数的原码与一个负数的原码相加，结果一定为负数，如3的原码为(00000011)<sub style="font-size:10px">2</sub>，-5的原码为(10000101)<sub style="font-size:10px">2</sub>，两者相加：

<div align="center"><img src="/images/2-0-3.PNG"></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;显而易见，这并不是正确的运算结果，说明仅使用原码无法正确完成含有负数的运算。为解决这一问题，又引入了反码表示形式。

####（2）反码

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;正数的反码与原码相同，负数的反码是将原码中符号位以外的其它各位都取反，即1变为0，0变为1，如3的原码为(00000011)<sub style="font-size:10px">2</sub>，反码为(00000011)<sub style="font-size:10px">2</sub>；-5的原码为(10000101)<sub style="font-size:10px">2</sub>，-5的反码为(11111010)<sub style="font-size:10px">2</sub>。那么利用反码计算3+（-5）的步骤如下：

<div align="center"><img src="/images/2-0-4.PNG"></div>

####（3）补码

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;正数的补码与原码相同，负数的补码是将其反码的最低位加1。例如，－5的原码为(10000101)<sub style="font-size:10px">2</sub>，其反码为(11111010)<sub style="font-size:10px">2</sub>，补码为(11111011)<sub style="font-size:10px">2</sub>。

##2.2.2计算机中非数值数据的编码

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;随着时代的发展，计算机不仅限于处理数值数据，字符、图像、音频、视频等数据也是计算机处理的对象。我们知道无论什么类型的数据在计算机中都是以二进制的形式表示的，计算机之所以能够区分这些数据，是因为它们采用的编码规则不同。

###1.西文字符编码

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;由于构成西方单词的字母并不繁多，所以西文字符的编码比较简单。目前，通常采用ASCII（American Standard Code for Information Interchange，美国标准信息交换码）来对西文字符进行编码。每个ASCII码用1个字节储存，但ASCII码只用到了后7位，即b6b5b4b3b2b1b0,最高位一般记为0。数值范围为0~127，可表示128个不同的字符，如图2-1所示。

<div align="center"><img src="/images/2-1.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图2-1 ASCII码表</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ASCII码是ANSI (American National Standard Institute ，美国国家标准学会)制定的，最初是美国国家标准，规定了计算机在通信时须遵守的编码标准，后被国际标准化组织定为国际标准。在这128个字符中，有96个可打印字符，32个控制字符。每个字符都有与之对应的ASCII码值，如大写字母“A”对应的二进制码为1000001，十进制码为65，所以“A”的ASCII码值就是65。目前除了ASCII码，还有UCS、Unicode等常用的编码标准。

###2.汉字编码

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;从输入汉字到计算机存储汉字再到屏幕显示、打印输出汉字，会涉及汉字的输入码、机内码、字形码、地址码等一系列编码，计算机对汉字信息的处理过程就是各种汉字编码间的转换过程，如图2-2所示。

<div align="center"><img src="/images/2-2.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图2-2 汉字在计算机中的编码</p></div>

####（1）汉字输入码

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;为将汉字输入计算机，利用计算机标准键盘上按键的不同排列组合来对汉字的输入进行编码。输入编码方案用程序实现即为输入法，可分为音码、形码、音形码等。

####（2）国标码

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;我国1980年发布了编号为GB2312—80的国家汉字编码标准《信息交换用汉字编码字符集——基本集》，确定的编码称为国编码。该标准收入了进行一般汉字信息处理时所用的7445个字符编码。国标码使用两个字节表示一个汉字的编码。

####（3）汉字机内码

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;汉字机内码又称汉字内码或内码，与国际码有简单的对应关系，是计算机内部对汉字进行存储、处理和传输的编码。汉字机内码由两字节表示一个汉字，且最高位均为1。

####（4）汉字地址码

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;汉字地址码是汉字库中存储汉字字形信息的逻辑地址码。

####（5）汉字字形码

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;汉字字形码是用0和1编码无亮点和有亮点像素,形成汉字字形的一种编码。依据字形码通过显示器或打印机输出汉字。

###3.声音编码

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;人能听到的声音包括：语音、音乐、其他声音（环境声、音效声、自然声等）。声音是由振动产生的，并以声波形式在传播介质中传播，属于模拟信号。而计算机无法处理模拟信号，所以需将声音信号转换为计算机可以处理的数字信号，即将声波进行周期性的采样并将样本数据以有限位的二进制数字形式存储，这个过程就是声音的数字化。常见的数字音频文件格式有：CD-DA、WAVE、MP3、RealAudio、WMA、APE、FLAC、MIDI等。其中MIDI格式不是数字化的音频波形数据，而是演奏乐器的各种指令和数据信息，主要用于计算机作曲领域、游戏音轨以及电子贺卡。

###4.图像编码

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;图像具有直观、表现力强、包含信息量大等特点，计算机中的图像可以分为位图图像和矢量图像。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;位图图像又称光栅图，通过描述图像中各个像素点的亮度与颜色信息来表示图像。像素、分辨率和颜色深度是位图图像的3个基本要素。像素是构成位图图像的最小单位，以矩阵的方式排列成图像，像素越多，图像的质量就越好；分辨率是用来度量位图图像内数据量的多少，分辨率越高，占用的硬盘空间越大，图像的质量越好；像素的颜色信息用若干二进制位来表示，这里的二进制位数称为图像的颜色深度（或图像深度）。常见的位图图像格式有JPEG、GIF等。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;矢量图像也称矢量图形或向量式图形，用计算机指令来表示构成图像的基本元素。与位图图像相比，矢量图像文件较小，不易失真，但不易制作色调丰富或色彩变化太多的图像，绘制出来的图像不够逼真。常见的矢量图像格式有WMF、SVG等。