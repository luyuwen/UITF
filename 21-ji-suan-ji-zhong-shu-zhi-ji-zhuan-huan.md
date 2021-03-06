#2.1 计算机中数制及转换

<div align="center"><iframe frameborder="0" width="640" height="498" src="https://v.qq.com/txp/iframe/player.html?vid=u0870ds00vh" allowFullScreen="true"></iframe></div>
<div align="center"><p style="font-size:20px; font-weight:bold">教学微视频</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在日常生活中，人们通常使用十进制数，但在计算机内部采用二进制表示数据，为书写及使用方便，还引入了八进制数和十六进制数。

##2.1.1 不同的进制

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;进位计数制是目前广泛使用的一种计数方法，我们日常生活中最常用的是十进制，计算机世界里各种类型的信息均采用二进制编码进行表示和存储，如图像、音频、视频等。除此之外，为了表示方便，有时也会使用八进制、十六进制等表示数据。关于进位计数制，我们首先应该了解基本符号、基数以及位权的概念。基本符号是指用来表示某种数制的基本符号，如二进制的基本符号为0和1；基数表示某数制可以使用的基本符号的个数，如二进制的基数为2，因为二进制只能用0和1两个基本符号表示；位权表示一个数值中每位数字符号的权值大小，如十进制234可以写成2×10<sup style="font-size:10px">2</sup>+3×10<sup style="font-size:10px">1</sup>+4×10<sup style="font-size:10px">0</sup>，那么2的位权为10<sup style="font-size:10px">2</sup>，3的位权为10<sup style="font-size:10px">1</sup>，4的位权就为10<sup style="font-size:10px">0</sup>。不同的进制有不同的运算规则和表示方法，此处介绍几种常用的进制。

###1.二进制

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在具有冯.诺依曼结构的计算机中，都采用二进制代码表示字母、数字以及各种各样的符号、汉字等。二进制的基数为2，基本符号是0和1，运算规则为“逢二进一，借一当二”，即当某一位计数达到2时就向高位进1，反过来向高位借1，那么在低位就相当于2。二进制中第i位的位权为2<sup style="font-size:10px">i-1</sup>。

###2.八进制

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在一些计算机编程语言中，常常以数字“0”作为开头来表明该数字是八进制，如果是负数，则以负号开头，例如，-087。八进制的基数为8，基本符号是0-7，运算规则为“逢八进一，借一当八”，八进制中第i位的位权为8<sup style="font-size:10px">i-1</sup>。

###3.十进制

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;十进制形式是我们最熟悉的表达形式，十进制的基数为10，基本符号是0-9，运算规则为“逢十进一，借一当十”，十进制中第i位的位权为10<sup style="font-size:10px">i-1</sup>。

###4.十六进制

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;十六进制的表示方式有很多，其中最常用的表示方式是将“0x”加在数字前，或在数字后加上小字 16。例如 0x3E6 和 3E6<sub style="font-size:10px">16</sub>。十六进制的基数为16，基本符号是0-9、A-F，运算规则为“逢十六进一，借一当十六”，十六进制中第i位的位权为16<sup style="font-size:10px">i-1</sup>。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;可以将上述内容归纳为表2-1，方便读者查阅，其中位权的表示方法仅适用于整数部分。

<div align="center"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">表2-1 键盘</p></div>

|进位制|运算规则|基数|基本符号|位权|
| :------: | :------: | :------: |:------: | :------: |
|二进制|逢二进一，借一当二|2|0,1|2<sup style="font-size:10px">i-1</sup>|
|八进制|逢八进一，借一当八|8|0,1,2,3,4,5,6,7|8<sup style="font-size:10px">i-1</sup>|
|十进制|逢十进一，借一当十|10|0,1,2,3,4,5,6,7,8,9|10<sup style="font-size:10px">i-1</sup>|
|十六进制|逢十六进一，借一当十六|16|0,1,2,3,4,5,6,7,8,9，A,B,C,D,E,F|16<sup style="font-size:10px">i-1</sup>|

##2.2.2不同进位计数制间的转换

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;不同进位制数之间可以相互转换，但转换方法有所不同，初学进位制转换可以参考以下二进制、八进制、十进制与十六进制之间的对应关系，如表2-2所示。

<div align="center"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">表2-2 进制转换对应关系</p></div>

|二进制|八进制|十进制|十六进制|
| :------: | :------: | :------: |:------: |
|0000|0|0|0|
|0001|1|1|1|
|0010|2|2|2|
|0011|3|3|3|
|0100|4|4|4|
|0101|5|5|5|
|0110|6|6|6|
|0111|7|7|7|
|1000|10|8|8|
|1001|11|9|9|
|1010|12|10|A|
|1011|13|11|B|
|1100|14|12|C|
|1101|15|13|D|
|1110|16|14|E|
|1111|17|15|F|

###1.二进制数与十进制数的相互转换

####（1）二进制数转换为十进制数

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;二进制数转换为十进制数相对比较简单，只要将二进制数的各位数字与其相对应的位权相乘，然后累加所有乘积，那么得到的结果就是该数的十进制形式。确定各位数字的位权时，应把小数点作为分界点，小数点往左应从2<sup style="font-size:10px">0</sup>开始，依次为2<sup style="font-size:10px">1</sup>，2<sup style="font-size:10px">2</sup>，2<sup style="font-size:10px">3</sup>……,小数点往右应从2<sup style="font-size:10px">-1</sup>开始，依次为2<sup style="font-size:10px">-2</sup>,2<sup style="font-size:10px">-3</sup>,2<sup style="font-size:10px">-4</sup>……。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;例如将二进制数1101.01转换为十进制数：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1101.01=1×2<sup style="font-size:10px">3</sup>+1×2<sup style="font-size:10px">2</sup>+0×2<sup style="font-size:10px">1</sup>+1×2<sup style="font-size:10px">0</sup>+0×2<sup style="font-size:10px">-1</sup>+1×2<sup style="font-size:10px">-2</sup>=8+4+0+1+0.5+0.25=13.75

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;结果为（1101.01）<sub style="font-size:10px">2</sub>=（13.75）<sub style="font-size:10px">10</sub>

####（2）十进制数转换为二进制数

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;十进制数转换成二进制数，由于整数和小数的转换方法不同，一般会将整数部分和小数部分分别进行转换，然后拼接在一起。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;①整数部分，整数部分的转换可采用“除2取余法”，基本思想是将需要转换的十进制数除以2，得到商和余数，商作为被除数除以2，再次得到商和余数，重复此步骤，直到商为0。将所得余数按照逆序排列就得到了该数的二进制形式。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;例如将十进制数37转换为二进制数：

<div align="center"><img src="/images/2-0-1.PNG"></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;得到的余数按逆序排列为100101，因此（37）<sub style="font-size:10px">10</sub>=（100101）<sub style="font-size:10px">2</sub>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;②小数部分，小数部分可采用“乘2取整法”，基本思想是将小数部分乘以2，并取出所得乘积的整数部分，将剩余的小数部分再次乘以2，并取出整数部分，重复此步骤，直到小数部分为0或者达到要求的精确度为止，最后将所取整数按顺序排列就是该数小数部分的二进制形式。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;例如将十进制数19.75转换为二进制数：

<div align="center"><img src="/images/2-0-2.PNG"></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;结果为（19.75）<sub style="font-size:10px">10</sub>=（10011.11）<sub style="font-size:10px">2</sub>

###2.二进制数与八进制数的相互转换

####（1）二进制数转换为八进制数

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;由于八进制数的基数8是2的三次方，因此，二进制数转换为八进制数时，可以从小数点开始向左或向右，每3位二进制数为一组，若小数部分最后一组不足3位则在末尾补0。将每组二进制数转为其对应的八进制数，然后拼接在一起即可。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;例如将二进制数10101.11转换为八进制数：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;二进制数  10  101  .  110

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;八进制数  2    5  .  6

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;即（10101.11）<sub style="font-size:10px">2</sub>=（25.6）<sub style="font-size:10px">8</sub>

####（2）八进制数转换为二进制数

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;八进制数转换为二进制数，从小数点开始向左或向右,将每1位八进制数用3位二进制数表示出来，然后拼接在一起，就将该数转换成了它的二进制形式。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;例如将八进制数74.6转换为二进制数：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;八进制数    7     4   .    6

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;二进制数   111	 100  .   110

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;即（74.6）<sub style="font-size:10px">8</sub>=（111100.110）<sub style="font-size:10px">2</sub>

###3．二进制数与十六进制数之间的转换

####（1）二进制数转换为十六进制数

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;由于十六进制数16为2的四次方，因此，二进制数转换为十六进制数时，可以参照二进制向八进制转换的方法，从小数点开始向左或向右，每4位二进制数为一组，若小数部分最后一组不足4位则在末尾补0，将每组二进制数转为其对应的十六进制数，然后拼接在一起即可。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;例如将二进制数11011010.101转换为十六进制数：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;二进制数    1101   1010  .    1010

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;十六进制数   D		 A	.	  A

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;结果为（11011010.101）<sub style="font-size:10px">2</sub>=（DA.A）<sub style="font-size:10px">16</sub>

####（2）十六进制数转换为二进制数

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;十六进制转换为二进制数，可以参照八进制向二进制转换的方法，从小数点开始向左或向右,将每1位十六进制数用4位二进制数表示出来，然后拼接在一起，就将该数转换成了它的二进制形式。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;例如将十六进制数6F.B4转换为二进制数：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;十六进制数      8        D    .   A        3	

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;二进制数	   1000    1101   .  1010     0011	

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;结果为（8D.A3）<sub style="font-size:10px">16</sub>=10001101.10100011)<sub style="font-size:10px">2</sub>

###4.十进制数与十六进制数的相互转换

####（1）十进制数转换为十六进制数

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;十进制数转换为十六进制数，可以参考十进制数转换为二进制数的方法，整数部分可采用“除16倒取余法”，小数部分可采用“乘16取整法”。还有一些相对比较简便的方法，比如，先将十进制数转换为二进制数，然后再将二进制数转换为十六进制数。

####（2）十六进制数转换为十进制数

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;参考二进制数转换为十进制数，将其按权展开求和即可。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;例如将十六进制数12C.A转换为十进制数：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;（12C.A）<sub style="font-size:10px">16</sub>=1×16<sup style="font-size:10px">2</sup>+2×16<sup style="font-size:10px">1</sup>+12×16<sup style="font-size:10px">0</sup>+10×16<sup style="font-size:10px">-1</sup>=（300.625）<sub style="font-size:10px">10</sub>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;结果为（12C.A）<sub style="font-size:10px">2</sub>=（300.625）<sub style="font-size:10px">10</sub>