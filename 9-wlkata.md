# <center>10. Mirobot蓝牙示教器快速上手教程</center>
##&diams; 蓝牙示教器功能详解
蓝牙遥控器是专为Mirobot机械臂设计的一款离线控制器，包含角度控制、坐标控制、点位示教、夹具控制等功能。
<center><img src="http://lin88zhang.gitee.io/image/9/9-1.png" width="600"  > </center>
Mirobot蓝牙手柄主要由Angle Mode、Coord Mode、Record、Setting功能页面构成。<br/>
（1）Angle Mode页面：机械臂各个轴的运动控制。
<center><img src="http://lin88zhang.gitee.io/image/9/9-2.png" width="500"  > </center>
（2）Coord Mode页面：机械臂笛卡尔模式的运动控制。
<center><img src="http://lin88zhang.gitee.io/image/9/9-3.png" width="500"  > </center>
（3）Record页面：机械臂的示教与复现运动
<center><img src="http://lin88zhang.gitee.io/image/9/9-4.png" width="500"  > </center>
（4）Setting页面：机械臂运动速度控制与蓝牙连接。
<center><img src="http://lin88zhang.gitee.io/image/9/9-5.png" width="500"  > </center>

##&diams; 蓝牙示教器开关机与连接
第1步：长按蓝牙手柄上的电源按钮三秒，即可打开蓝牙手柄。关机按同一按钮三秒即可。
<center><img src="http://lin88zhang.gitee.io/image/9/9-6.png" width="500"  > </center>
第2步：用IDC排线连接蓝牙扩展模块与机械臂通信扩展接口。
<center><img src="http://lin88zhang.gitee.io/image/9/9-7.png" width="600"  > </center>
第3步：打开机械臂电源。此时蓝牙扩展模块上的红色LED灯开始闪烁，等待蓝牙手柄连接。
<center><img src="http://lin88zhang.gitee.io/image/9/9-8.png" width="300"  > </center>
第4步：切换蓝牙遥控器上的控制页面选项卡到Setting页面。
<center><img src="http://lin88zhang.gitee.io/image/9/9-9.png" width="400"  > </center>
第5步：点击Search按钮，按钮变为Searching，等待几秒后变为Link。然后点击Link按钮即可连接成功。连接成功后，红色LED灯常亮，绿色LED灯点亮。
<center><img src="http://lin88zhang.gitee.io/image/9/9-10.png" width="400"  > </center>

##&diams; 蓝牙示教器控制机械臂
以角度蓝牙手柄控制的角度模式为例，说明蓝牙手柄控制机械臂的基本操作。<br/>
第1步：切换蓝牙手柄界面到Angle Mode界面。
<center><img src="http://lin88zhang.gitee.io/image/9/9-11.png" width="400"  > </center>
第2步：连接成功后，对机械臂进行复位操作，长按蓝牙手柄右上方红色按钮3秒，机械臂开始复位，等待机械臂复位成功。
<center><img src="http://lin88zhang.gitee.io/image/9/9-12.png" width="500"  > </center>
第3步：按蓝牙手柄右侧的6组按钮，可以控制机械臂的6个相应轴向正/负方向运动。
<center><img src="http://lin88zhang.gitee.io/image/9/9-13.png" width="500"  > </center>
第4步：示教演示<br/>
（1）长按左上角“<font color="red">REC键</font>”等到显示器左上角记录点点亮后。在Angle Mode界面控制Mirobot运动到某个位置时单击<font color="red">REC键</font>键记录当前位置，记录多个位置坐标即可形成连贯动作。
<center><img src="http://lin88zhang.gitee.io/image/9/9-14.png" width="600"  > </center>
（2）录制完成后长按<font color="red">REC键</font>键等到显示器左上角记录点熄灭完成示教记录。<br/>
（3）点击回放默认播放Record页面内第一个示教文件，如需播放其他文件需进入Record页面选中相应文件点击OK键或触屏Play图标3秒。
<center><img src="http://lin88zhang.gitee.io/image/9/9-15.png" width="600"  > </center>