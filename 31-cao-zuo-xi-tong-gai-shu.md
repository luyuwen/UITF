#3.1 操作系统概述

<div align="center"><iframe frameborder="0" width="640" height="498" src="https://v.qq.com/txp/iframe/player.html?vid=a0874d1b28n" allowFullScreen="true"></iframe></div>
<div align="center"><p style="font-size:20px; font-weight:bold">教学微视频</p></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;操作系统是计算机系统中最重要的软件系统，由于计算机拥有繁多的硬件资源和软件资源且要同时运行不同的程序，若由用户来管理这些资源，可能会阻碍计算机的普及，因此计算机中需要有一个可以帮助用户管理各种资源的特权软件，在计算机系统中扮演管家的角色，这个管家就是操作系统，主要负责管理计算机中的硬件和软件资源。

##3.1.1 操作系统的发展

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;纵观计算机的发展历史，操作系统伴随计算机硬件系统经历了从无到有、从简到繁的发展过程。起初，操作系统只提供简单的工作排序服务，后因硬件设施不断更新，而渐渐发生演化。发展至今，操作系统已种类繁多，可以满足不同硬件环境的需求。

###1.20世纪50年代

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;将作业按照一定的特点进行分批，之后成批的提交给计算机系统，由计算机处理这一批作业并输出结果，这样的操作称为批处理，可以有效减少作业建立和结束过程中的时间浪费。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;按照内存中可以存放、处理的作业数，批处理系统可以分为单道批处理系统和多道批处理系统。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;20世纪50年代第二代晶体管计算机问世，为了提高计算机系统的利用率，使其连接运行以减少机器的空闲时间，出现了单道批处理系统。单道批处理系统的工作方式是计算机操作员把一批作业输入到磁带中，系统中的监督程序会将磁带上的第一个作业装入内存并运行，当该作业处理完成时，监督程序把磁带上的第二个作业调入内存并运行，重复上述步骤直至完成磁带上的全部作业。由于内存每次只加载运行一个作业，所以这种批处理系统被称作单道批处理系统。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;由于单道批处理系统的内存中每次仅有一个作业，这致使系统中的资源不能被充分利用，为解决资源的利用率问题，出现了多道批处理系统。如图3-1所示，多道批处理系统的内存可同时容纳多个作业，如果正在执行的作业由于某些原因被暂停，那么内存中的另一个作业会被执行。多道批处理系统提高了计算机的资源利用率和系统吞吐量，但也存在一定的局限，如无交互能力，用户一旦把作业交给系统，那么作业在被执行完成之前，用户不能对作业进行任何交互。

<div align="center"><img src="/images/3-1.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图3-1 多道批处理作业过程</p></div> 

###2.20世纪60年代

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;随着计算机硬件系统的性能不断提高，20世纪60年代出现了分时系统，即一台主机上连接多个终端，允许多个用户共享主机资源，内存中也可同时装入多个作业。分时系统的工作方式是将CPU的时间划分成若干个时间片，当连接主机的多个用户终端提出请求时，系统采用时间片轮转的方式处理用户请求，并通过交互方式向用户显示运行结果。若作业在划分的时间片内无法执行完成，那么处理器会暂停执行该作业并开始执行下一个作业，未执行完成的作业会在下一轮继续执行。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;实时系统是指系统能及时响应外部事件的请求，在一定时间范围内处理好该事件，并控制协调所有实时任务的运行。实时系统在生活比较常见，主要包括实时信息处理系统和实时过程处理系统，我们常用的订票系统、银行事务处理系统都是实时信息处理系统，这类系统在保密性、安全性等方面的要求较高；航天系统的控制、交通控制、工业生产的自动控制等都是实时过程处理系统，这类系统对安全性、可靠性等方面的要求极高。

###3.20世纪80年代

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;20世纪80年代家用计算机开始普及，之后用户不同的需求使得操作系统更加多样化，同时操作系统的能力也越来越强大，出现了个人计算机操作系统、嵌入式操作系统和分布式操作系统等。个人计算机操作系统伴随个人计算机的出现应运而生，这类操作系统给用户提供了更多支持，更方便的使用接口。嵌入式操作系统是用于嵌入式智能芯片的操作系统，它的用途十分广泛，具有系统内核小、专用性强、系统精简、高实时性等特点。分布式操作系统主要负责管理分布式系统资源处理和控制分布式程序运行，它通过网络将计算机连接在一起以实现对分散资源的管理等，因此分布式操作系统具有极高的运算能力。

##3.1.2 常用的操作系统

###1.DOS

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;磁盘操作系统（Disk Operation System，简称DOS）是由微软公司开发的单用户单任务操作系统,部分Windows系统是以DOS为基础开发的，如Windows 95、Windows 98和Windows Me等。之后DOS的概念也包含了与MS-DOS兼容的系统，如PC-DOS、DR-DOS。目前随着开放源代码的兴起，越来越多的爱好者和程序员参与到了DOS软件的设计和开发当中，这使得DOS软件的功能更加强大。

###2.UNIX

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1969年美国AT&T公司贝尔实验室的工作人员研发了UNIX，起初研发者只是对UNIX比较感兴趣，关于UNIX的第一篇文章发表后，引起了学术界的广泛关注，各个大学、公司开始尝试基于UNIX源码进行各种改进和拓展，UNIX逐渐开始流行。20世纪70年代，AT&T公司注意到了UNIX的商业价值便开始采取一些手段来保护UNIX。UNIX属于支持多用户、多任务的分时操作系统，具有易读、易修改、易移植，且安全性、保密性和可维护性较高的特点。只有符合单一UNIX规范的UNIX系统才可以称为UNIX，否则只能称为类UNIX。
 
###3.Linux

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Linux属于类UNIX操作系统，是由林纳斯·托瓦兹及其团队开发完成的，图3-2是林纳斯·托瓦兹的照片。Linux拥有图形界面和字符界面，支持多用户、多任务，保证各用户之间互不影响且多个程序可同时独立运行。Linux可以在多种硬件平台上运行，如手机、平板电脑、台式计算机、大型机和超级计算机。

<div align="center"><img src="/images/3-2.png"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图3-2 Linux创始人林纳斯·托瓦兹</p></div> 

###4.Windows

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Windows系统问世于1985年，是由微软公司研发的基于图形用户界面操作系统，相比于DOS操作系统，它的操作方式更具人性化，深受大众喜爱，这使其很快成为个人计算机上使用比较广泛的操作系统。目前个人计算机上所使用的操作系统主要包括Windows7、Windows8、Windows8.1、Windows10，服务器上主要安装的是Windows Server 2003、Windows Server 2008、Windows Server 2012。微软公司也开发了用于嵌入式设备的Windows CE和用于智能手机的Windows Phone，图3-3是Windows Phone的界面。

<div align="center"><img src="/images/3-3.jpg"><p style="text-align:center; font-size:10px; margin-top:2px; font-weight:bold">图3-3 Windows Phone界面</p></div> 

###5.Mac OS 与 iOS

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Mac OS是首个在商用领域获得成功的图形用户界面操作系统，突出了形象的图标和人机对话，它运行于苹果计算机上。现行的最新的系统版本是Mac OS 10.14.3，在苹果推送的Mac OS Mojave 10.14中，更新了Safari浏览器，增加了深色模式等。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;iOS是苹果公司开发的移动操作系统，属于UNIX类的操作系统，最初是设计给iPhone使用的，后来陆续应用到了iPod touch、iPad以及Apple TV等产品上。

###6.Android

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Android是基于Linux的操作系统，最初是由Andy Rubin开发的，主要用于手机。随后Google公司收购注资，继续开发此系统，并公布了Android的源代码，随着程序员的不断开发更新，Android逐渐扩展到了其他领域上。2011年Android在全球的市场份额首次跃居全球第一，目前Android是基于Linux移动平台的主流操作系统。 
