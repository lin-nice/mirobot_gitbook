# <center>15. 多功能扩展模块用户手册</center>
##一、功能介绍
&emsp;&emsp;多功能扩展模块主要用于扩展机械臂对外接口，主要功能有：<br/>
&emsp;&emsp;&rArr;外接气泵、舵机夹子、滑轨、传送带等外部设备<br/>
&emsp;&emsp;&rArr;离线脱机运行机械臂的动作组<br/>
&emsp;&emsp;&rArr;扩展通信接口，支持WIFI、BT蓝牙、RS485通信<br/>
&emsp;&emsp;&rArr;显示机械臂状态<br/>

##二、接口及外观

<center><img src="http://lin88zhang.gitee.io/image/14/1.jpg" width="600"  > </center>

**Communication Interface / 通信接口：**<br/>
&emsp;&emsp;多功能扩展模块通过IDC排线连接机械臂，因此该接口用于多功能扩展模块和机械臂之间的通信。<br/>
**PWM Port / PWM信号输出接口：**<br/>
&emsp;&emsp;机械臂可输出PWM信号，该接口用于外接气泵、舵机夹子配件。接口电压5V，最大输出电流2A。<br/>
**Stepper Motor Port / 步进电机接口：**<br/>
&emsp;&emsp;该接口为第七轴步进电机接口，主要用于外接滑轨或传送带。<br/>
**Limit Switch Port / 复位开关结接口：**<br/>
&emsp;&emsp;该接口为第七轴复位开关接口，用于第七轴和机械臂的六个轴的同时复位。<br/>
**Power Output / 电源输出口：**<br/>
&emsp;&emsp;该接口为电源输出接口，用于外接设备的供电。输出电压12V，最大电流1A。<br/>
**RS485 Port / RS485接口：**<br/>
&emsp;该接口为RS485通信接口，用于多个机械臂的联动控制。<br/>
**OLED Screen / OLED屏幕：**<br/>
&emsp;&emsp;1.3寸 OLED屏幕，用于显示机械臂状态信息。<br/>
**State of the LED / LED指示灯：**<br/>
&emsp;&emsp;该指示灯会指示机械臂状态：<br/>
&emsp;&emsp;红灯闪烁：Offline，机械臂初始化中<br/>
&emsp;&emsp;红灯常亮：Alarm，机械臂锁定中<br/>
&emsp;&emsp;绿灯常亮：Idle，机械臂待命中<br/>
&emsp;&emsp;蓝灯常亮：Run，机械臂运动中<br/>
**Navigation / 导航键：**<br/>
&emsp;&emsp;长按中间的导航键2秒，机械臂<font color="red">复位 (Homing)</font>。<br/>

##三、快速入门
###1.连接线缆

<center><img src="http://lin88zhang.gitee.io/image/14/2.jpg" width="400"  > </center>

&emsp;&emsp;按图连接好机械臂和多功能扩展模块后，打开机械臂电源。
###2.使用末端工具
&emsp;&emsp;详见“WLKATA气动套件安装与使用指南”。
###3.使用手机app （目前只支持安卓版本）
&emsp;&emsp;步骤1：下载app并安装<br/>
&emsp;&emsp;&emsp;&emsp;下载地址：https://www.wlkata.com/support/download-center

<center><img src="http://lin88zhang.gitee.io/image/14/3.jpg" width="600"  > </center>

&emsp;&emsp;步骤2：打开手机蓝牙，配对蓝牙“Mirobot”，配对密码“7676”。

<center><img src="http://lin88zhang.gitee.io/image/14/4.jpg" width="300"  > </center>

&emsp;&emsp;步骤3：打开APP，点击Scan,然后点击Select Device，选择点击以下项目。

<center><img src="http://lin88zhang.gitee.io/image/14/5.jpg" width="300"  > </center>

&emsp;&emsp;然后点击Connect，如果显示以下状态，表示连接成功。

<center><img src="http://lin88zhang.gitee.io/image/14/6.jpg" width="400"  > </center>

&emsp;&emsp;步骤4：开始操作，首先需要长按Homing对机械臂进行复位，然后进行其他操作。
###4.示教器使用
&emsp;&emsp;步骤1：打开示教器电源，等待屏幕右上角出现蓝色的蓝牙标志，表示蓝牙连接成功。<br/>
&emsp;&emsp;步骤2：开始操作，首先需要长按Homing对机械臂进行复位，然后进行其他操作。
###5.离线运行功能
&emsp;&emsp;通过上位机的Blockly下载功能，可以将Blockly中写好的代码下载至多功能扩展模块中，从而实现机械臂脱机离线运行。
文件下载（**目前只支持Blockly**）<br/>
&emsp;&emsp;步骤1：在Blockly中编写动作后，点击“下载”按钮

<center><img src="http://lin88zhang.gitee.io/image/14/7.jpg" width="600"  > </center>

&emsp;&emsp;步骤2：选择文件保存位置，输入文件名（文件名不支持中文），例如“test”。点击确定后，文件开始下载。提示“GCode保存完成！”，表示下载成功。

<center><img src="http://lin88zhang.gitee.io/image/14/8.jpg" width="600"  > </center>

###6.文件运行
&emsp;&emsp;步骤1：查询已下载的文件列表，切换命令控制，发送指令“o110”

<center><img src="http://lin88zhang.gitee.io/image/14/9.jpg" width="600"  > </center>

&emsp;&emsp;步骤2：在上位机运行下载文件。发送指令“o111”+文件名，例如 o111test。<br/>
&emsp;&emsp;&emsp;&emsp;如果机械臂返回noIdle，表示机械臂没有解锁。用户需先执行机械臂<font color="red">复位(Homing)</font>，再发送该指令。<br/>
&emsp;&emsp;&emsp;&emsp;如果机械臂返回ok，表示文件运行成功。<br/>

<center><img src="http://lin88zhang.gitee.io/image/14/10.jpg" width="600"  > </center>

###7.脱机运行
&emsp;&emsp;（1）连接机械臂线缆以及机械臂与多功能控制板之间的线缆，如有夹具，连接好夹具线缆。<br/>
&emsp;&emsp;（2）按下机械臂电源按钮。<br/>
&emsp;&emsp;（3）刚开始红灯闪烁：Offline，机械臂初始化中等到红灯常亮：Alarm，机械臂锁定中，长按导航键2秒，完成机械臂复位之后，机械臂将会自动脱机运行文件。<br/>
