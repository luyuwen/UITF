#5.2 数据分析和处理

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;本节以图5-28中的工作表为例，讲解Excel的排序、筛选、分类汇总、数据透视表等操作。

<div align="center"><img src="/images/5-28.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-28 示例工作表</p></div> 

##5.2.1 数据排序

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;排序是指对指定数据的先后顺序进行调整，数据可以是文本、数字、日期与时间等。选中需要进行排序的列，单击【开始】选项卡，在【编辑】选项组中选择【排序和筛选】命令按钮，在弹出的列表中选择【升序】、【降序】或【自定义排序】，如图5-29所示。

<div align="center"><img src="/images/5-29.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-29 排序</p></div> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;选定排序方式后，Excel会弹出“排序提醒”对话框，提示是否扩展排序区域，通常情况下选择“扩展选定区域”，避免工作表的数据混乱，如图5-30所示。如果排序结果和预期结果有偏差，应仔细检查各数据格式是否一致。

<div align="center"><img src="/images/5-30.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-30 “排序提醒”对话框</p></div> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;升序和降序是按照阿拉伯数字、汉语拼音、或日期与时间的先后顺序进行排序。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;自定义排序可以设置多个排序条件，以图5-28中的工作表为例，假如用户想要对“职称”进行升序排列的同时又要对“工资”进行降序排列，如图5-31所示。那么需要选中“职称”列，单击【开始】选项卡，在【编辑】选项组中选择【排序和筛选】命令按钮，在弹出的列表中选择【自定义排序】。此时，会弹出“排序”对话框中，设置主要关键字为“职称”，排序依据为“数值”，次序为“升序”；设置次要关键字为“工资”，排序依据为“数值”，次序为“降序”，如图5-32所示，最后单击【确定】即可。

<div align="center"><img src="/images/5-31.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-31 自定义排序</p></div> 

<div align="center"><img src="/images/5-32.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-32 “排序”对话框</p></div> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;自定义排序可以实现区分字母的大小写，或者依据笔画数和字母对文本进行排序。单击【开始】选项卡，在【编辑】选项组中选择【排序和筛选】命令按钮，在弹出的列表中选择【自定义排序】，在“排序”对话框中选择【选项】命令按钮，在弹出的“排序选项”对话框中进行相关设置即可，如图5-33所示。

<div align="center"><img src="/images/5-33.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-33 “排序选项”对话框</p></div> 

##5.2.2 数据筛选

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;筛选可以根据指定条件显示和隐藏数据，Excel提供的筛选功能包括“自动筛选”和“高级筛选”。

###1.自动筛选

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;自动筛选一般用于条件简单的筛选，筛选时将不满足筛选条件的数据暂时隐藏起来，只显示符合筛选条件的数据。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;以图5-28中的工作表为例，假如用户想要查看所有男性员工的信息，如图5-34所示。需要选中“性别”列，单击【数据】选项卡，在【排序和筛选】选项组中选择【筛选】命令按钮，此时“性别”单元格的右下角会出现一个向下的三角符号。单击“性别”单元格右下角的三角符号，取消勾选性别“女”，单击【确定】即可，如图5-35所示。

<div align="center"><img src="/images/5-34.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-34 男性员工信息</p></div> 


<div align="center"><img src="/images/5-35.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-35 设置筛选条件</p></div> 

###2.高级筛选

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;进行高级筛选时，需要预先在被筛选的工作表的空白位置输入筛选的条件。输入的筛选条件需要满足两个要求：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;要求一：筛选条件需要设置表头标题且和数据表中的表头标题一致。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;要求二：筛选条件输入在同一行表示“与”的关系，如图5-36所示；不同的行表示“或”的关系，如图5-37所示。

<div align="center"><img src="/images/5-36-1.png"><img src="/images/5-36-2.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-36 “与”关系</p></div>  
 
<div align="center"><img src="/images/5-37-1.png"><img src="/images/5-37-2.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-37 “或”关系</p></div> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;筛选条件输入完成后，单击【数据】选项卡，在【排序和筛选】选项组中选择【高级】命令按钮，在弹出的“高级筛选”对话框中进行筛选操作，可以设置显示位置、列表区域和条件区域，设置完成后单击【确定】即可，如图5-38所示。

<div align="center"><img src="/images/5-38.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-38 “高级筛选”对话框</p></div> 


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;以图5-28中的工作表为例，假如用户想要查看职称为“初级工程师”且工资“大于3000”的员工信息，如图5-39所示。首先需要在空白区域设置筛选条件，此处选择了H17:I18单元格区域。然后单击【数据】选项卡，在【排序和筛选】选项组中选择【高级】命令按钮，在弹出的“高级筛选”对话框中设置【方式】为【在原有区域显示筛选结果】，在【列表区域】输入需要进行筛选的列表区域，在【条件区域】输入条件所在的单元格区域，此处设置为“Sheet1!$H$17:$I$18”，设置完成后单击【确定】即可。

<div align="center"><img src="/images/5-39.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-39 筛选结果</p></div> 
 


##5.2.3 数据分类汇总

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Excel提供了对数据进行分类汇总的功能。选中要进行分类汇总的单元格，单击【数据】选项卡，在【分级显示】选项组中选择【分类汇总】命令按钮，此时会出现如图5-40所示的“分类汇总”对话框。

<div align="center"><img src="/images/5-40.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-40 分类汇总</p></div> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;【分类字段】表示用户想按照哪一字段对工作表进行分类汇总；【汇总方式】包含对汇总项的操作函数，例如求和、平均值、最大值等；【选定汇总项】表示参与计算的列。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;以图5-28中的工作表为例，假如用户想要按照职称对员工的工资进行分类汇总，汇总方式为求和与最大值，如图5-41所示。首先按照职称对工资表进行升序或降序排序，然后选中工作表，单击【数据】选项卡，在【分级显示】选项组中选择【分类汇总】命令按钮。在“分类汇总”对话框中，将分类字段设置为“职称”，汇总方式设置为“求和”，选定汇总项设置为“工资”，确定之后再次单击【数据】选项卡，在【分级显示】选项组中选择【分类汇总】命令按钮，在“分类汇总”对话框中，将分类字段设置为“职称”，汇总方式设置为“最大值”，选定汇总项设置为“工资”，最后点击【确定】即可。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;如果不需要分类汇总的话，在“分类汇总”对话框中选择【全部删除】即可删除工作表中的分类汇总。

<div align="center"><img src="/images/5-41.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-41 分类汇总案例</p></div> 

##5.2.4 数据透视表

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;数据透视表是一种交互式的表，同样是对工作表中的数据进行分类汇总操作，但相对于分类汇总功能，数据透视表更加简洁方便。

###1.建立数据透视表

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;单击【插入】选项卡，在【表格】选项组中选择【数据透视表】命令按钮，此时会弹出“创建数据透视表”对话框，如图5-42所示。在对话框中选择要分析的数据和数据透视表的位置，设置完成后单击【确定】进入数据透视表，如图5-43所示。

<div align="center"><img src="/images/5-42.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-42 “创建数据透视表”对话框</p></div> 

<div align="center"><img src="/images/5-43.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-43 数据透视表</p></div> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在视图右侧的“数据透视表字段”中选择要添加至数据透视表的字段，勾选后字段会出现在下方的区域块内，包括筛选器、列、行、值。行和列即数据透视表的行内容与列内容；值即对字段进行函数操作；筛选器可以在数据透视表中进行自动筛选操作。

###2.修改数据透视表

####（1）修改字段

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在数据透视表右侧的“数据透视表字段”窗格中可以修改数据透视表的字段，在字段节内可以添加或删除相应的字段，如图5-44所示。

<div align="center"><img src="/images/5-44.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-44 字段节</p></div> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在区域节内可以调整数据透视表的行列，对数据的处理方式。如需修改数据透视表的行列，鼠标单击需要改变的字段，拖动至行或列即可，如图5-45所示。在下方的【推迟布局更新】处可以选择实时更新还是手动更新，若不勾选【推迟布局更新】，那么进行相关操作的同时，工作区会发生相应的变化，勾选【推迟布局更新】后，在数据透视表中进行的更改则不出现在工作区，此时可以手动点击【更新】按钮进行更新。

<div align="center"><img src="/images/5-45.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图5-45 修改数据透视表的行列</p></div> 

####（2）修改样式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;选择要修改样式的数据透视表，此时工具栏会显示【分析】和【设计】两个数据透视表工具选项卡，单击【设计】选项卡，在【数据透视表】选项组中挑选合适的样式即可。

###3.删除数据透视表

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;选择要删除的数据透视表，单击【分析】选项卡，在【操作】选项组中选择【清除】命令按钮，在弹出的列表中选择【全部清除】即可删除数据透视表。
