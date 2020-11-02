# <center>2. Mirobot快速上手指南-Windows</center>
##第1步：点击WLKATA Studio目录下的“WLKATA Studio.exe”打开控制软件
<center><img src="http://lin88zhang.gitee.io/image/1/1-1.png" width="600"  > </center>

##第2步：Mirobot机械臂连线
1）使用USB数据线连接机械臂与计算机。
<center><img src="http://lin88zhang.gitee.io/image/1/1-2.png" width="350"  > </center>
2）接通Mirobot机械臂电源并按下机械臂底座上电源开关
<center><img src="http://lin88zhang.gitee.io/image/1/1-3.png" width="350"  > </center>
3）开机：按下Mirobot机械臂底座侧面的开关按钮，按钮上的电源指示灯将亮起
即打开Mirobot机械臂的电源。
<center><img src="http://lin88zhang.gitee.io/image/1/1-4.png" width="600"  > </center>

##第3步：Mirobot Studio与机械臂连接
1）打开“设备管理器”窗口。在“端口（COM和LPT）”中可以找到 “USB-SERIAL CH340(COMX )”，则说明驱动安装成功，COMX中X表示对应端口号，下图中对应COM5。
<center><img src="http://lin88zhang.gitee.io/image/1/1-5.png" width="600"  > </center>
打开Mirobot Studio软件。正常情况下，WLKATA Studio上位机会自动连接Mirobot机械臂对应串口，如果未能连接，可单击设置选项卡设置“串口号”及“波特率”。点击“确定”后，左上角会显示“已连接”。
<center><img src="http://lin88zhang.gitee.io/image/1/1-6.png" width="600"  > </center>

##第4步：让Mirobot动起来
1）在进行任何对机械臂的控制操作之前，必须对机械臂进行复位操作。点击Mirobot Studio中右上角“复位”按钮，如图所示。然后等待机械臂复位完成。
<center><img src="http://lin88zhang.gitee.io/image/1/1-7.png" width="600"  > </center>
下图所示为复位后的机械臂姿态。
<center><img src="http://lin88zhang.gitee.io/image/1/1-8.png" width="500"  > </center>
2）“角度控制模式”下，可通过界面右侧“J1~J6”控制机械臂各个轴转动。
<center><img src="http://lin88zhang.gitee.io/image/1/1-9.png" width="600"  > </center>
3）“坐标控制模式”下，可通过界面右侧“X、Y、Z、RX、RY、RZ”控制机械臂末端坐标位置及末端姿态。
<center><img src="http://lin88zhang.gitee.io/image/1/1-10.png" width="600"  > </center>