#7.2 Internet及开放教育资源

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;随着计算机网络的不断发展，Internet已经渗透到了各行各业，成为了人们生活、学习、工作中不可或缺的一部分。Internet的普及为教育注入了新的活力，使得学习者脱离了时间、空间的束缚，越来越多的学习者倾向于在线教育。学习者的需求推动了开放教育资源的发展，同时开放教育资源为所有学习者提供了公平的学习机会。

##7.2.1 Internet及其服务

###1.什么是Internet

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Internet即互联网，是全球最大的、资源非常丰富的计算机网络。随着时代的发展，Internet几乎成了人们生活中不可或缺的一部分，Internet之所以发展如此迅速，与它自身的特点密切相关，即它是一个全球计算机互联网络且拥有极其丰富的信息资源。Internet起源于美国国防部的高级研究计划局建设的军用网ARPAnet，之后万维网的成功开发为Internet实现广域超媒体信息截取/检索奠定了基础。20世纪90年代后，部分商家开始关注Internet，这使得Internet开始走向商业化。目前，Internet已经渗透到了人类社会的各个领域，人们的学习方式、工作方式、娱乐方式、购物方式也开始慢慢依赖Internet。

###2.TCP/IP协议

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;网络中的计算机要进行通信，就必须遵守相关的规则、标准等，这些规则、标准的集合称为网络协议。在网络的发展完善过程中，出现了很多协议，其中TCP/IP（Transmission Control Protocol/ Internet Protocol）协议的应用较为广泛。TCP/IP协议起初是为军用网ARPAnet设计的，现在发展为互联网的基础协议。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TCP/IP协议包括两个核心协议：传输控制协议（TCP）和网际协议（IP）。TCP协议是Internet中的传输层协议，提供点对点的链接机制，负责把数据流分割成长度适当的数据包，然后将数据包传给IP层，IP层通过网络将数据包发送到接收端的TCP层。为保证传输的可靠性，TCP将每个包都编上序号，这样接收端也可按序接收。若接收端成功收到数据包就会返回一个确认，如果在合理的往返时延内发送端没有收到确认，就会重新发送该数据包。IP协议规定了在网络上进行数据传输时应遵循的规则等，它的任务是把数据包从发送端传送到接收端，但不保证传输的可靠性，对数据没有差错控制，主要功能是寻址、数据分段等。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TCP/IP参考模型分为四层，即网络访问层、互联网层、传输层和应用层，如图7-12所示。应用层对应于OSI七层参考模型中的应用层、表示层和会话层，包含所有的高层协议，如FTP、SMTP等；传输层对应于OSI七层参考模型中的传输层，提供可靠的传输服务；互联网层对应于OSI七层参考模型中的网络层，完成最佳传输路径的选择；网络访问层是TCP/IP参考模型中的底层，对应于OSI七层参考模型中的数据链路层和物理层。TCP/IP协议的层次结构如图7-13所示。

<div align="center"><img src="/images/7-12.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图7-12 TCP/IP参考模型</p></div> 

<div align="center"><img src="/images/7-13.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图7-13 TCP/IP协议层次结构</p></div> 

###3.IP地址

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;互联网上的设备数量极其庞大，为实现信息的正确传送，需要为互联网上的每个设备都分配一个“编号”。基于TCP/IP协议分配的地址称为IP地址或网络协议地址，互联网上的每台主机都拥有一个唯一的可识别的IP地址，我们可以把一台计算机比作一部手机，那么IP地址就相当于手机号码。为了便于寻址以及层次化构造网络，每个IP地址都包括网络地址和主机地址两部分，同一个物理网络上的主机使用的网络地址相同，不同的主机拥有不同的主机地址，即主机地址是区分各个主机的依据。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;IP地址的长度为32位，将组成IP地址的32位二进制数分成四段，每段8位，例如11001010 11001001 00000111 00001100,但这样表示不便于记忆，将二进制数转化为十进制数后就方便许多。用十进制数表示时，每段数字范围为0～255，通常采用“点分十进制”的方法表示，上述IP地址就可以表示为202.201.7.12。
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;按照不同的标准，IP地址可以分为不同的类型。

####（1）按照网络地址和主机地址的不同分类

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;为适合不同容量的网络，Internet委员会定义了5种IP地址类型，它们拥有不同的地址，不同的适用范围，分别为A类、B类、C类、D类和E类，其中D、E类为特殊地址。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;①A类IP地址的四段数字中，第一段数字为网络地址并且规定网络地址的最高位必须为“0”，网络地址范围是1.0.0.0~127.0.0.0，其余三段为主机地址，如图7-14所示。A类网络数量有限，但可以包含的主机数量庞大，适用于大型计算机网络。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;②B类IP地址的四段数字中，前两段数字为网络地址并且规定网络地址的最高位必须为“10”，网络地址范围是128.0.0.0~191.254.0.0，后两段为主机地址，如图7-14所示。B类IP网络地址适用于中等规模的网络。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;③C类IP地址的四段数字中，前三段数字为网络地址并且规定网络地址的最高位必须为“110”，网络地址范围是192.0.0.0~223.254.254.0，最后一段为主机地址，如图7-14所示。C类地址包含的网络数量较大，但每个网络内的主机数量有限，适用于小规模的局域网络。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;④D类IP地址为特殊地址，不标识网络，第一个字节的前四位固定为“1110”，是一个专门保留的地址，目前这一类地址被用在多点广播中。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;⑤E类IP地址为特殊地址，第一个字节的前四位固定为“1111”。

<div align="center"><img src="/images/7-14.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图7-14 IP地址分类</p></div> 

####（2）按照用途和安全级别的不同分类


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;按照用途和安全级别的不同，IP地址可以分为公共地址和私有地址。前述规则都是针对公共IP地址，公共IP地址由Internet Network Information Center负责，一个组织或机构想要接入互联网，就必须申请公共IP地址。考虑到网络安全等问题，在IP地址中保留了私有地址，只能在内部网络中使用，因为本网络中保留的地址可能在其他网络中也被使用，所以当网络互联时，就会因为地址不唯一而出现错误。保留的私有IP地址范围如下：

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;A类 10.0.0.0~10.255.255.255

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;B类 172.16.0.0~172.31.255.255

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;C类 192.168.0.0~192.168.255.255

###4.主机域名

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;IP地址是用数字进行表示的，为了便于人们的记忆和使用，出现了一套为主机命名的机制，用来标识网络上的主机，即域名。IP地址与域名的表示方式不同，但都具有唯一性，每个域名对应着主机的IP地址。当用户利用域名在互联网上进行查询等相关操作时，域名解析服务器会将用户输入的域名转换为其对应的IP地址，这样计算机才可以完成网络内的工作。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;域名是由一串用“.”分隔的字符组成的，代表了互联网上某一台计算机或计算机组的名称。域名一般包含3到4个子域，子域级别由左向右逐渐升高，最右边的子域称为顶级域，最左边的子域是互联网上主机的名字。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;顶级域名一般可以分为机构域和地理域两类，如下表所示：

<div align="center"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">表7-1 部分常见的顶级域名</p></div>

|机构域|	说明|地理域|说明|
|:------:|:------:|:------:|:------:|
|.com|商业机构|.cn|中国|
|.edu|教育及研究机构|.hk|中国香港|
|.info|信息服务机构|.tw|中国台湾|
|.net|网络服务机构|.au|澳大利亚|
|.gov|政府机构|.fr|法国|
|.org|民间组织或非赢利性组织|.uk|英国|
|.mil|军事机构|.ca|加拿大|

###5.Internet接入方式

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Internet的接入方式指的是最终用户连入Internet的方法，接入Internet的方式多种多样，例如拨号上网、ISDN接入、ADSL接入、光纤入户接入、无线网络等。

####（1）拨号上网

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;拨号上网是家庭用户普遍使用的一种接入Internet的方式。用户通过电话线，利用当地运营商提供的接入号码，拨号接入Internet。这种方式的优点是使用方便，缺点是速率较低。

####（2）ISDN接入

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ISDN俗称“一线通”，用户利用一条ISDN线路，就可以在上网的同时拨打电话、收发传真，就像拥有两条电话线一样。这种接入Internet的方式比拨号上网的速度要快，但仍无法实现一些高速率要求的网络服务。

####（3）ADSL接入

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ADSL可以在普通电话线上传输高速数字信号，通过在线路两端安装ADSL设备，用户便可使用宽带服务。ADSL与普通电话线共用一条线，接听、拨打电话与ADSL传输互不影响。相比于拨号上网和ISDN接入Internet的方式，ADSL的费用相对较低，因为它传输数据时不通过电话交换机，用户就无需缴纳额外的电话费。

####（4）光纤入户接入

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;现在很多新建小区都支持光纤到户，用户只需办理相关业务便可接入Internet。光纤入户的优点是速率高，可以实现各类高速率的互联网应用，例如视频服务、远程交互等；其次它的抗干扰能力很强，缺点是一次性布线成本较高。

####（5）无线网络

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;无线网络是有线接入的一种延伸，主要使用无线射频技术收发数据，可以减少线路连接。一般情况下，无线网络会作为已存在的有线网络的补充。

###6.Internet服务

####（1）Web服务

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Web服务是目前应用最为广泛的一种Internet服务，可以帮助运行在不同机器上的不同应用相互交换数据，而无须借助第三方软硬件。它建立在请求/服务模式上，用户只需请求服务，无需知道所请求的服务是怎样实现的。在Web服务的体系结构中包括Web服务提供者、Web服务请求者和Web服务中介者三类角色，Web服务提供者将自己已有的功能、服务提供给其他用户；Web服务请求者就是Web服务功能的使用者；Web服务中介者相当于管理者，主要负责将合适的Web服务请求者与Web服务提供者联系在一起。这三类角色在实际应用中可能存在交叉，例如Web服务提供者在某种情况下也可以是Web服务请求者。 

####（2）FTP服务

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;早期在Internet上传输文件并不容易，Internet环境比较复杂，有各种各样的终端且终端的操作系统可能不同。为解决各种操作系统之间的文件交流问题，出现了FTP即文件传输协议。FTP服务与大多数Internet服务一样，也是一种请求/服务模式的应用。初期用户通过FTP客户端软件才可以访问FTP服务，实现文件的上传和下载，现在使用浏览器就可以完成相应的工作，但用户需要获得相应的权限后，才能上传或下载文件。Internet上存在大量的匿名FTP服务器，为了网络安全，大多数匿名FTP服务器都允许用户从其下载文件，而不允许用户向其上传文件。也有部分匿名FTP服务器允许用户向其上传文件，但之后系统管理员会检查这些文件，这样可以有效保护远程主机的安全，避免病毒文件的传播。

####（3）E-mail服务

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;E-mail服务是Internet上应用最广的服务之一，用户通过电子邮件系统可以快速的与其他网络用户联系。起初，用户发送和接收E-mail需要使用专门的客户端软件，例如Outlook。现在Internet上有许多免费的邮件系统，例如腾讯邮件系统，用户只需要一台联网的计算机便可进行访问。用户使用邮件系统时需要先开通自己的邮箱帐号，邮件内容可以是文字、图片、音频等。在邮件收发过程中涉及到发送方和接收方，发送方编辑好的电子邮件会被送到服务器，服务器识别接受者的地址并将电子邮件存放在接受者的邮箱内，之后接受者便会收到邮件提醒。

####（4）电子公告板

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;电子公告板（Bulletin Board System，简称BBS）是一种发布并交换信息的在线服务系统。早期的BBS只能同时接受一两个人访问，而且内容也没有严格的规定。之后出现了以Internet为基础的BBS，受到了广大网友的欢迎，BBS的功能也逐渐扩展，目前BBS已不仅仅是电子布告栏，它主要包括信件讨论区、文件交流区、信息布告区和交互讨论区等。 
                          
####（5）网格计算

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;网格计算是分布式计算的一种，它可以将一个需要巨大计算能力才能解决的问题分割成许多小的部分，例如分析来自外太空的电讯号、寻找隐蔽黑洞等，然后把这些小部分分配给许多计算机进行处理，最后把这些计算结果综合起来得到最终结果。参与分布式计算可以充分发挥个人计算机的利用价值且不会对个人计算机的使用造成影响。参与分布式计算的绝不是一台计算机，而是一个计算机网络，这样的计算方式拥有很强的数据处理能力，具有共享稀有资源和平衡计算负载等优点，很多超级计算机都难以完成的项目，却可以通过网格计算得以实现。

####（6）P2P

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;P2P（Peer to Peer）即对等网络，是一种分布式网络，具有非中心化、可扩展性、健壮性和负载均衡等特点。在P2P网络结构中不存在中心服务器，所有节点都是平等的，每个节点既可以是信息消费者，同时也可以是信息提供者，即每个节点既充当服务器为其他节点提供服务，同时也享用其他节点提供的服务。P2P网络打破了传统的客户端/服务器模式，没有服务器的介入，避免了可能的瓶颈，并且网络中的节点越多，下载速度就越快。常见的P2P应用包括协同处理服务、文件资源服务、及时通信等。

##7.2.2 Web技术

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Web是一种基于超文本和HTTP的分布式图形信息系统。1994年，人们进入了Web1.0时代，这个时候的信息主要通过静态的HTML网页进行发布，传递过程主要是单向的，用户只是信息的消费者。Web1.0将众多信息聚集在一起，满足了用户搜索信息的需求。与Web1.0时代不同，Web2.0强调用户的参与，用户不仅仅是信息的消费者，还是信息的创造者、共建者，维基百科就是Web2.0时代的一个典型产物，同时还出现了大量的博客、百科全书等。Web3．0是Web2．0的发展与延伸，拥有智能化及个性化的搜索引擎，提供了更多人工智能服务，用户可以实现实时参与。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Web技术是Web应用开发的技术总称，大体可以分为Web服务端技术和Web客户端技术两大类。由于Web技术涉及的内容很多，此处仅介绍几个基础的概念。

###1.HTML

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HTML为超文本标记语言，是网页内容的描述语言，“超文本”是指页面内不仅可以包含文字，还可以包含图片、链接，音乐等非文字元素。HTML可以利用标记符号来描述网页内容，浏览器解释标记符后将页面呈现给用户，不同的浏览器对同一标记符可能会有不同的解释，呈现给用户的界面也就不同。HTML的结构包括头部和主体，头部主要提供网页的相关信息，例如页面的标题等；主体部分主要提供网页的具体内容。在HTML文件中，大多标记符都是成对出现的，例如文件的开始与结尾分别用`<html>`和`</html>`来标记，头部信息的开始与结尾分别用`<head>`和`</head>`来标记，主体信息的开始与结尾分别用`<body>`和`</body>`来标记。

###2.网页与网站

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;网页是一个包含HTML标签的纯文本文件，包括文字、图片、动画、音乐、程序等元素。网页可以分为静态网页和动态网页，静态网页是存储在Web服务器或本地服务器上的内容确定的页面，静态网页具有制作周期短、成本低，确定后不易修改，对服务器的性能要求较低等特点；动态网页由服务器端的程序动态创建，页面内容取决于用户提供的参数和存储在数据库中的数据，动态网页对服务器的性能要求较高。我们可以将静态网页看作照片，不会轻易改变，而动态网页则是镜子，不同的人会出现不同的镜像，即不同的参数会出现不同的页面内容。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;网站是指按照一定规则，展示特定内容的网页集合。初期，网站只能呈现单纯的文本，随着网络技术的发展，图像、声音、动画、视频等都可以呈现给用户，现在部分网站还为用户提供了业务处理服务、在线交流服务等。

###3.URL

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;统一资源定位符（Uniform Resource Locator，简称URL）是Internet上各种资源地址的表示。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Internet上的每个资源文件都拥有一个唯一的URL，URL可以分为绝对URL和相对URL两类，绝对URL表示文件在硬盘上真正完整的绝对路径，相对URL表示，目标文件相对于当前文件的位置。一个URL包括协议、服务器名称或IP地址、路径和文件名，如兰州大学主页的URL为http://www.lzu.edu.cn:80/。

###4.HTTP

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;超文本传输协议（Hyper Text Transfer Protocol，简称HTTP)是一种应用较为广泛的网络协议，它提供了一种发布和接收HTML页面的方法，各类学校的门户网站、文献检索等大多都是采用HTTP进行服务的。HTTP协议采用了请求/响应模型，客户机向服务器发送服务请求，服务器处理客户机发送的请求并将处理结果返回客户机，呈现给用户。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HTTP的工作过程是：首先客户机与服务器建立连接；连接成功之后客户机向服务器发送请求，请求的参数中包含请求页面的URL地址；服务器接收到请求后进行相关的处理，并把处理结果返回到客户端，处理结果的相关信息通过浏览器呈现给用户；之后客户机与服务器之间的连接会断开，以保证其他客户机与服务器能够建立连接。如果上述过程中出现了错误，那么产生错误的信息会返回到客户端，整个过程中，用户只需点击鼠标，等待信息即可，具体工作会由HTTP完成。图7-15是HTTP请求响应的示意图。

<div align="center"><img src="/images/7-15.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图7-15 HTTP工作原理示意图</p></div> 

###5.Web服务端技术与Web客户端技术

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Web服务端技术是Web服务器实现相关服务时所使用的技术，主要包括PHP、ASP、ASP.NET、Servlet和JSP技术；Web客户端的主要任务是将服务器返回的响应内容展现给用户，主要使用到的技术有HTML语言、Java Applets、脚本程序、CSS、DHTML、插件技术以及VRML等技术。

##7.2.3 开放教育资源

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;联合国教科文组织曾指出:开放教育资源（Open Educational Resources, 简称OER）是缩小教育鸿沟、推动教育公平、增进教育机会、提高教学品质、激发教育创新的重要驱动力。开放教育资源是指使用者可以无限制或较少限制地获取、使用、重组、重用并重新散播置于公共领域的、在开放许可协议下的任何形式资料。互联网时代，世界各国都在积极建设开放教育资源，开放教育资源平台则是开放教育资源的支撑。目前国际上有影响力开放教育资源平台有Wiki Books、Coursera等。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;大规模在线开放课程（Massive Open Online Courses，简称MOOC）是“互联网+教育”的产物。它打破了时间和空间的限制，突破传统课程人数限制，增强了学习者参与课程的自主性，终身学习变得越来越容易。MOOC最初在美国兴起，之后便以其独特的优势席卷全球，目前知名度较高、影响力较大的MOOC平台是美国的edX、Coursera和Udacity三大MOOC平台。我国也大力支持MOOC的发展，《教育信息化“十三五”规划》提出“发展在线教育与远程教育，推动各类优质教育资源开放共享，向全社会提供服务”。清华大学推出了学堂在线，根据美国课程中央网站给出的数据，2016年底，学堂在线的课程数量、注册用户数量位居全球第三，仅次于Coursera和edX；网易公司推出了网易云课堂，为更多的学习者提供在线课程；包括复旦大学、南京大学在内的多所高校签约MOOC平台Coursera，致力于打造优质的在线课程。此处简单介绍几个国内外具有影响力、发展较为成熟的MOOC平台。

###1.美国MOOC平台介绍

####（1）edX

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;edX是麻省理工和哈佛大学联手创建的大规模开放在线课程平台，主要目的是配合校内教学，提高教学质量、推广网络在线教育，为所有学习者提供免费开放的课程。edX实行董事会领导下的伙伴学校支委员会监管、会员学校领导委员会下属的委员会与团队分工负责制，以此保证平台的正常运行。目前edX汇集了100多名校课程，国内高校包括清华大学、北京大学、香港科技大学等。edX为非营利性的平台，但若想拿到签名认证的证书就需要缴纳一定的费用，图7-16为edX官网主页。

<div align="center"><img src="/images/7-16.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图7-16 edX官网主页</p></div> 

####（2）Coursera

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Coursera是由斯坦福大学创建的，汇集了全球100多所名校的MOOC课程，与Coursera合作的国内高校有北京大学、复旦大学、上海交通大学、西安交通大学、南京大学、香港大学、香港科技大学等。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Coursera是一个比较综合的平台，涉及的学科、语言较多，界面显示支持中文，并且部分英文课程还会提供中文字幕。Coursera的课程中只有一部分可以免费观看，其他课程则需缴纳规定的费用才可进行学习，与edX相同的是用户需要交费才可以拿到签名认证的证书。虽然Coursera提供给用户的部分课程需要收费，但同时它也设置了助学金，以帮助没有能力支付规定费用的学生，图7-17为Coursera官网主页。

<div align="center"><img src="/images/7-17.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图7-17 Coursera官网主页</p></div> 

####（3）Udacity

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Udacity于2012年2月推出,截至目前，Udacity上的课程涵盖了计算机科学、数学、物理学、统计学等。Udacity界面支持英文，但目前Udacity中文官网已经上线，试运行期间，所有纳米学位的课程均可免费体验一个月，到期后将会收取一定的费用。纳米学位是 Udacity与Google、Facebook、亚马逊等互联网公司联合推出的学历认证项目，学员以在线学习的方式，完成Udacity的课程学习，考核合格后即可获得学历，同时Udacity会为部分学员提供奖学金，支持学员的学习与深造，图7-18为Udacity官网主页。

<div align="center"><img src="/images/7-18.jpg"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图7-18 Udacity官网主页</p></div> 

###2.国内MOOC平台介绍

####（1）学堂在线

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;学堂在线是清华大学基于edX开放源代码研发的中文在线教育平台，现初步完成平台国际化与中文本地化。在2016年果壳网发布的“全球MOOC排行榜”中，学堂在线被评为“拥有最多精品好课”的三甲平台之一。目前学堂在线的合作伙伴有斯坦福大学、复旦大学、西安交通大学、哈尔滨工业大学、山东大学、同济大学等。学堂在线的课程涵盖面较广，涉及的学科较多，部分课程需要付费才可学习，图7-19为学堂在线官网主页。

<div align="center"><img src="/images/7-19.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图7-19 学堂在线官网主页</p></div> 

####（2）中国大学MOOC

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;中国大学MOOC是由网易与高教社合作推出的大型开放式在线课程学习平台，于2014年5月上线，它联合北京大学、复旦大学、浙江大学、南京大学、同济大学、北京师范大学、新加坡国立大学、微软亚洲研究院等多所知名高校和机构推出上千门精品课程，涉及计算机、心理学、经济学、管理等多领域，还有专门针对英语四六级、考研的课程，图7-20为中国大学MOOC官网主页。

<div align="center"><img src="/images/7-20.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图7-20 中国大学MOOC官网主页</p></div> 


####（3）好大学在线

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;好大学在线是上海交通大学发起的中国高水平大学MOOC联盟官方网站,致力于汇聚优质的教学资源，平台的界面支持中文和英文显示。目前好大学在线的课程涵盖了哲学、经济学、法学、教育学、理学、工学、农学、医学等多个领域，部分课程采用英文作为授课语言。好大学在线有学分互认的运作机制，即在校大学生修读完其学校认定的好大学在线课程，并且考核通过后，学校会给予相应的学分，图7-21为好大学在线官网主页。

<div align="center"><img src="/images/7-21.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图7-21 好大学在线官网主页</p></div> 
