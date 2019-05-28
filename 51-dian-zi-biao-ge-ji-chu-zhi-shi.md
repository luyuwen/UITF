#5.1 电子表格基础知识

<div align="center"><iframe frameborder="0" width="640" height="498" src="https://v.qq.com/txp/iframe/player.html?vid=k087558nbd2" allowFullScreen="true"></iframe></div>
<div align="center"><p style="font-size:20px; font-weight:bold">教学微视频</p></div>

##5.1.1 电子表格基本概念与操作

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Microsoft Excel是一款电子表格软件，可以在Windows和Apple Macintosh操作系统内运行，常用于数据统计与分析。

###1.工作界面

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;图5-1是Excel的工作界面，由快速访问工具栏、标题栏、窗口操作按钮、功能区、状态栏和工作表等构成。其中快速访问工具栏、标题栏、窗口操作按钮、视图栏的功能与Word类似，此处主要介绍功能区、工作区。

<div align="center"><img src="/images/5-1.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-1 Excel工作界面</p></div> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;功能区包括文件、开始、插入、页面布局、公式、数据、审阅、视图等多个选项卡，每个选项卡均包含了与电子表格相关的处理操作命令，点击不同的选项卡，功能区也会随之发生变化。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;工作区由单元格、当前单元格地址、函数、编辑区、列标、行号、滚动条和工作表标签组成。单元格和编辑区内可以输入数据、公式；函数按钮可以选择插入的公式；列标和行号用来标注单元格的地址；工作表标签展示工作表信息。

###2.基本概念

####（1）工作簿

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Excel创建的文件称作工作簿，扩展名为“.xlsx”。工作簿由一个或多个工作表组成，例如一个销售情况工作簿可以由第一季度、第二季度、第三季度和第四季度的销售数据共四个工作表构成。用户可以在工作簿内操作工作表和单元格进行数据处理。

####（2）工作表

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;工作簿窗口中显示的表格称为工作表，工作表标签中高亮显示的是当前操作的工作表。工作表的名称在下方工作表标签中显示，选中工作表单击鼠标右键可以重命名工作表。单击工作表标签右侧的<img src="/images/5-0-1.png">按钮可以增加新的工作表。Excel默认有1张工作表，工作表的默认数量可以在【文件】选项卡中的【选项】命令中修改，图5-2为“Excel选项”对话框。

<div align="center"><img src="/images/5-2.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-2 “Excel选项”对话框</p></div>

####（3）行号和列标

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Excel工作表是由行和列构成的一张二维表。行号由数字1、2、3、……表示。列标由字母A、B、C、……AB、AC、……表示。

####（4）单元格和单元格区域

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;单元格是工作表中行与列的交叉部分形成的矩形区域，它是组成表格的最小单位。每个单元格都有其默认的名字，命名规则为列标加行号，如图5-3中“A”所在单元格的名字为“C4”，代表第C列，第4行的单元格。

<div align="center"><img src="/images/5-3.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-3 单元格</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;单元格可以输入和修改数据，包括字符、文本、数字和公式等，输入完成后，敲击“Enter”键确认输入。单元格中显示的值与编辑区显示的值相同，如果是公式，单元格显示的是公式计算出的值，编辑区仍显示公式。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;单元格区域即多个相邻单元格组成的区域，常用于对多个单元格执行相同的操作，或者对多个单元格中的数据进行运算。单元格区域用“:”表示，例如“A1:C3”代表的是以A1为起点，C3为终点共9个单元格组成的区域。

###3.常用数据类型

####（1）字符型数据

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;字符型数据包括任何中西文文字或字母、数字、空格等。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;如果要输入的字符型数据全部由数字组成且长度较长，如身份证号、电话号码、存折帐号等，为了避免Excel将输入的值按数值型数据处理，在输入时可以先输一个英文状态下的单引号，再输入具体的数字。例如，要在单元格中输入号码“123456789123456789”，先输入英文状态下的单引号，再输入号码，如图5-4所示。

<div align="center"><img src="/images/5-4.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-4 输入长数字</p></div>

####（2）数值型数据

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;数值型数据包括阿拉伯数字以及含有正号、负号、货币符号、百分号等任一种符号的数据。在输入过程中，有以下两种比较特殊的情况需要注意：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;①负数，在数值前加一个减号“-”或把数值放在括号里，都可以输入负数，例如要在单元格中输入“-1”，可以输入“(1)”或“-1”，然后敲击回车键即可。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;②分数，对于一些分子和分母数值比较小的分数而言，Excel会将其处理为日期格式的形式，例如“5/15”，单元格显示的内容为5月15日。如需在单元格中输入分数形式的数据，应先在编辑框中输入“0”和一个空格再输入分数，或者在分数前输入英文状态下的单引号，以此确保每一个输入数据都可以正确显示。

####（3）日期型数据和时间型数据

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在人事管理等工作中，经常需要录入一些日期型的数据，在录入过程中要注意以下几点：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;①输入日期时，年、月、日之间要用“/”号或“-”号隔开，例如“2002-8-16”、“2002/8/16”。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;②输入时间时，时、分、秒之间要用冒号隔开，例如“10:29:36”。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;③若要在单元格中同时输入日期和时间，日期和时间之间应该用空格隔开。 

###4.基本操作

####（1）插入单元格

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;选中需要插入单元格的位置，单击鼠标右键，在弹出的菜单中选择【插入】，根据需求在弹出的对话框中选择当前单元格需要移动的位置，如图5-5所示。

<div align="center"><img src="/images/5-5-1.png"><img src="/images/5-5-2.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-5 插入单元格</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;①活动单元格右移：活动单元格向右移一个单元格。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;②活动单元格下移：活动单元格向下移一个单元格。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;③整行：活动单元格所在行向下移一个单元格。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;④整列：活动单元格所在列向右移一个单元格。

####（2）删除单元格

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;①删除单元格：选中单元格，单击鼠标右键，在弹出的菜单中选择【删除】，并根据需求选择周围的单元格如何移动，如图5-6所示。

<div align="center"><img src="/images/5-6-1.png"><img src="/images/5-6-2.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-6 删除单元格</p></div>     

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;②删除单元格内容：选中单元格，在【开始】选项卡中选择中的【清除】命令按钮，在弹出的菜单中选择【清除内容】，如图5-7所示。

<div align="center"><img src="/images/5-7.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-7 删除单元格内容</p></div> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;值得注意的是①和②的区别在于①将整个单元格删除，②仅将单元格中的内容删除，而单元格依然存在。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;③删除行：鼠标右键单击要删除的行号，在弹出的菜单中选择【删除】即可。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;④删除列：鼠标右键单击要删除的列标号，在弹出的菜单中选择【删除】即可。

####（3）选择单元格

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;选择只包含少量单元格的小型单元格区域时，单击第一个单元格，然后拖动到想要包含在该区域中的最后一个单元格即可。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;若要选择较大的单元格区域，单击第一个单元格并按住“Shift”键，同时单击区域中的最后一个单元格即可。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;若要选择整列或整行，单击该列或该行的列标或行号即可。

##5.1.2 数据运算与数据填充

###1.数据运算

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Excel公式是Excel工作表中进行数值计算的等式。公式输入是以“=”开始的。简单的公式有加、减、乘、除四则运算。

####（1）公式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;公式是方便用户输入的运算表达式。如需输入公式，首先定位到要输入公式的单元格，在单元格中或编辑栏中先输入“=”再输入公式，输入完成后敲击“Enter”键进行计算即可。

####（2）运算符

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;①类型，运算符的类型有多种，表5-1列举了常见的运算符类型，并解释了其含义。

<div align="center"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">表5-1 Excel运算符</p></div>

<table>
 <tr>
  <th>类型</th>
  <th>运算符</th>
  <th>描述</th>
 </tr> 
 <tr>
  <td rowspan="6">算术运算符</td>
  <td>+</td>
  <td>加法：相加运算符两侧的值</td>
 </tr>
 <tr>
  <td>-</td>
  <td>减法：左操作数减去右操作数</td>
 </tr>
 <tr>
  <td>*</td>
  <td>乘法：相乘运算符两侧的值</td>
 </tr>
 <tr>
  <td>/</td>
  <td>除法：左操作数除以右操作数</td>
 </tr>
 <tr>
  <td>%</td>
  <td>百分比：操作数的百分数</td>
 </tr>
 <tr>
  <td>^</td>
  <td>幂运算：底数（底数的个数等于指数）相乘</td>
 </tr>
 <tr>
  <td rowspan="6">比较运算符</td>
  <td>＝</td>
  <td>等于：检查如果两个操作数的值是否相等，如果相等则条件为真</td>
 </tr>
 <tr>
  <td>&lt;&gt;</td>
  <td>不等于：检查如果两个操作数的值是否相等，如果值不相等则条件为真</td>
 </tr>
 <tr>
  <td>&lt;</td>
  <td>小于：检查左操作数的值是否小于右操作数的值，如果是那么条件为真</td>
 </tr>
 <tr>
  <td>&lt;=</td>
  <td>小于等于：检查左操作数的值是否小于或等于右操作数的值，如果是那么条件为真</td>
 </tr>
 <tr>
  <td>&gt;</td>
  <td>大于：检查左操作数的值是否大于右操作数的值，如果是那么条件为真</td>
 </tr>
 <tr>
  <td>&gt;=</td>
  <td>大于等于：检查左操作数的值是否大于或等于右操作数的值，如果是那么条件为真</td>
 </tr>
 <tr>
 <td>文本运算符</td>
 <td>&</td>
 <td>连接：将一个或多个文本连接成为一个新文本</td>
 </tr>
 <tr>
  <td rowspan="3">引用运算符</td>
  <td>：</td>
  <td>区域运算符：对两个引用之间（包括两个引用）的所有单元格进行引用</td>
 </tr>
 <tr>
  <td>，</td>
  <td>联合运算符：将多个引用合并为一个引用</td>
 </tr>
 <tr>
  <td>空格</td>
  <td>交叉运算符：对两个引用共有的单元格的引用</td>
 </tr>
</table>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;②运算优先级

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;如果公式中运用了多个运算符，其优先级从高到低依次为：冒号>逗号>空格>负号>百分比>幂运算>乘、除>加、减>连接符>比较运算符。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;需要注意的是，运算过程中若有括号则先算括号中的内容。

####（3）函数

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;函数是Excel内预设的公式，函数可以计算多个值并返回结果。函数可以避免用户输入复杂公式，提高工作效率。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Excel中一共有13类函数，包括财务函数、日期与时间函数、数学与三角函数、统计函数、查找与引用函数、数据库函数、文本函数、逻辑函数、信息函数、工程函数、多维数据集函数、兼容性函数、Web函数。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;使用函数时，首先选中插入公式的单元格，单击【函数】按钮，此时会弹出“插入函数”对话框，如图5-8所示，从中选择需要的计算函数，单击【确定】。在“函数参数”对话框中选择进行计算的数据，单击【确定】即可得出运算结果，如图5-9所示。

<div align="center"><img src="/images/5-8.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-8 “插入函数”对话框</p></div> 

<div align="center"><img src="/images/5-7.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-9 设置参数</p></div> 

###2.数据填充

####（1）自动填充

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;对于工作表的一列数据而言，如果当前输入数据的前几个字符与该列输入数据的前几个字符重复，Excel就会自动填充后面的文本，如图5-10所示。输入的数据可以是纯文本，也可以是文字与数字的组合（文字在前）。

<div align="center"><img src="/images/5-10.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-10 自动填充文本</p></div> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;如果用户确定输入相同的内容，敲击“Enter”键即可；否则的话敲击“BackSpace”键删除自动填充的内容。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;用户可以根据需要关闭自动填充功能。单击【文件】选项卡，选择【选项】命令按钮，在“Excel选项”对话框中选择【高级】，在编辑选项中取消勾选【自动快速填充】即可，如图5-11所示。

<div align="center"><img src="/images/5-11.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-11 “Excel选项”对话框</p></div>

####（2）使用填充柄填充

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;填充柄是Excel提供的快速填充单元格的工具，默认开启，用户可以在“Excel选项”对话框中关闭。选中包含数据的单元格，将光标移动至选区右下角的绿色方块上，此时光标会变成填充柄（黑色十字）。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;①填充字符和数字：激活填充柄，单击鼠标左键并拖动，可以实现单元格内容的填充。单击鼠标右键并拖动可以选择单元格的填充方式，如图5-12所示。

<div align="center"><img src="/images/5-12.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-12 选择填充方式</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;②填充日期数据：选中填充数据区域的第一个单元格，输入起始日期，激活填充柄并拖动即可。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;③填充数字序列：选中填充数据区域的第一个单元格，输入起始数据，在下一个单元格内输入第二个数据，激活填充柄并拖动即可。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;④自定义序列：Excel允许用户自定义序列。单击【文件】选项卡，选择【选项】命令按钮，会弹出“Excel选项”对话框，选择其中的【高级】，接下来在【常规】中选择【编辑自定义列表】，如图5-13所示，此时会弹出“自定义序列”对话框，用户可以直接导入Excel预置的自定义序列，也可以手动输入自定义序列，输入完成后单击【确定】即可，如图5-14所示。新的序列定义完成后，用户可以通过填充柄使用自定义序列填充单元格。

<div align="center"><img src="/images/5-13.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-13 “Excel选项”对话框</p></div>

<div align="center"><img src="/images/5-14.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-14 “自定义序列”对话框</p></div>

##5.1.3 工作表格式设置

###1.单元格格式设置

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;单元格格式包括对单元格数据类型、对齐方式、字体、边框、填充颜色和保护的设置。进入【开始】选项卡，单击【数字】选项组右下方的对话框启动器，此时会弹出“设置单元格格式”对话框，如图5-15所示，用户根据实际需要进行相应的设置即可。

<div align="center"><img src="/images/5-15.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-15 “设置单元格格式”对话框</p></div>

###2.单元格样式设置

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;单击【开始】选项卡，可以在【样式】选项组中设置单元格的样式，如图5-16所示。

<div align="center"><img src="/images/5-16.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-16 设置单元格样式</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;①条件格式：可以根据指定条件，标记符合条件的单元格。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;②套用表格格式：将单元格区域快速转换为具有Excel内置样式的表格，如图5-17所示，也可以根据需要新建表格样式。

<div align="center"><img src="/images/5-17.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-17 套用表格格式</p></div>

###3.单元格设置
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
单元格设置包括行、列、单元格和工作表的插入和删除，以及单元格大小、可见性、组织工作表和保护等。单击【开始】选项卡，在【单元格】选项组中进行设置，如图5-18所示。

<div align="center"><img src="/images/5-18.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-18 单元格设置</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;如需修改全部工作表格式，按住“Ctrl”键，选中全部工作表标签，或者点击任一标签，单击鼠标右键选择【选定全部工作表】，选中的工作表标签为白色。修改任一工作表的格式，其他工作表的格式也会随之改变。

##5.1.4 工作表相关操作

###1.插入工作表

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;一个工作簿中默认有1个工作表，插入工作表的方法有以下三种：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;方法一：在任意一个工作表标签上单击鼠标右键，在弹出的菜单中选择【插入】。此时会弹出“插入”对话框，选择需要创建的工作表类型，单击【确定】即可，如图5-19所示。

<div align="center"><img src="/images/5-19.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-19 插入工作表</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;方法二：单击【开始】选项卡，在【单元格】选项组中选择【插入】命令按钮，在弹出的菜单中选择【插入工作表】。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;方法三：单击工作表标签最右侧的 符号，即可添加新工作表。

###2.删除工作表

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;删除工作表的方式有以下两种：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;方法一：在任意一个工作表标签上单击鼠标右键，在弹出的菜单中选择【删除】即可，如图5-20所示。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;方法二：单击【开始】选项卡，在【单元格】选项组中选择【删除】命令按钮，在弹出的菜单中选择【删除工作表】，如图5-21所示。

<div align="center"><img src="/images/5-20.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-20 删除工作表的第一种方法</p></div>

<div align="center"><img src="/images/5-21.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-21 删除工作表的第二种方法</p></div>

###3.工作表的隐藏和显示

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;当工作表数量过多时，可以选择隐藏其中不常用的工作表，提高工作效率，但工作簿内至少得有一张显示的工作表。

####（1）隐藏工作表

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;隐藏工作表的方式有以下两种：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;方法一：在任意一个工作表标签上单击鼠标右键，在弹出的菜单中选择【隐藏】即可。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;方法二：单击【开始】选项卡，在【单元格】选项组中选择【格式】命令按钮，在弹出的菜单中点击【隐藏和取消隐藏】→【隐藏工作表】即可。

####（2）显示工作表

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;显示工作表的方式有以下两种：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;方法一：在任意一个工作表标签上单击鼠标右键，在弹出的菜单中选择【取消隐藏】，在弹出的对话框中选择需要显示的工作表，单击【确定】即可。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;方法二：单击【开始】选项卡，在【单元格】选项组中选择【格式】命令按钮，在弹出的菜单中点击【隐藏和取消隐藏】→【取消隐藏工作表】，在弹出的“取消隐藏”对话框中选择需要显示的工作表，单击【确定】即可，如图5-22所示。

<div align="center"><img src="/images/5-22.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-22 “取消隐藏”对话框</p></div>

###4.工作表的移动

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;工作表可以在当前工作簿内移动，也可以移动至其他的工作簿内。选中需要移动的工作表标签，单击鼠标右键，在弹出的菜单中选择【移动或复制】，此时会弹出“移动或复制工作表”对话框，如图5-23所示，选择合适的工作簿及位置即可。

<div align="center"><img src="/images/5-23.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-23 “移动或复制工作表”对话框</p></div>

###5.工作表的重命名

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;选中需要重命名的工作表标签，单击鼠标右键，选择【重命名】，工作表标签的名称变为可更改状态，输入新名称即可。

###6.设置工作表标签颜色

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;选中需要更改标签颜色的工作表标签，单击鼠标右键，在弹出的菜单中选择【工作表标签颜色】，从弹出的主题颜色选择框中选择合适的颜色即可。

###7.保护工作表

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;保护工作表可以防止对数据进行不必要的修改，避免误操作。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;选中需要保护的工作表标签，单击鼠标右键，在弹出的菜单中选择【保护工作表】，此时弹出“保护工作表”对话框，如图5-24所示。用户需要设置取消保护时的密码，以及允许用户进行哪些操作。

<div align="center"><img src="/images/5-24.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-24 “保护工作表”对话框</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;工作表保护可以撤销，撤销时需要输入之前设置的取消保护的密码。单击【开始】选项卡，在【单元格】选项组中选择【格式】命令按钮，在弹出的菜单中选择【撤销工作表保护】，输入密码即可，如图5-25所示。

<div align="center"><img src="/images/5-25-1.png"><img src="/images/5-25-2.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-25 撤销工作表保护</p></div>  

##5.1.5 页面设置与打印

###1.选择打印区域

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;选中工作表中需要打印的区域，单击【页面布局】选项卡，在【页面设置】选项组中单击【打印区域】→【设置打印区域】，如图5-26所示。

<div align="center"><img src="/images/5-26.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-26 设置打印区域</p></div>

###2.打印

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;单击【文件】选项卡，选择【打印】命令按钮，在右侧的菜单栏中可以根据需要进行相应的打印设置，如图5-27所示，最后点击【打印】即可。

<div align="center"><img src="/images/5-27.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-27  打印界面</p></div>