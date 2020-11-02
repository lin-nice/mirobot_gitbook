# <center>3. 初识WLKATA Studio控制软件</center>
WLKATA  Studio是一款专门控制Mirobot桌面六轴教育机械臂的软件，软件包含机械臂指令控制、角度/坐标控制模式、点位示教、图形化编程、Python编程、写字画画、固件升级等多种功能。
##&diams; 中英文切换功能：
打开软件后点击设置语言选择英文或中文后确定并重启即可（也可通过点击界面右上角绿色框内的“CN”设置）。
<center><img src="http://lin88zhang.gitee.io/image/2/2-1.png" width="600"  > </center>

##&diams; 角度/坐标控制模式切换
（1）角度控制模式<br/>
第1步：单击命令控制选项卡
<center><img src="http://lin88zhang.gitee.io/image/2/2-2.png" width="600"  > </center>
第2步：在Mirobot Studio中控制模式选择处选择“角度运动模式”，选中后显示为白底高亮状态
<center><img src="http://lin88zhang.gitee.io/image/2/2-3.png" width="600"  > </center>
点击Mirobot Studio右侧的“J1~J6”单轴运动控制按钮可以控制机械臂的六个关节单独运动。可通过“速度”按钮或输入值调节各轴运动速度，可点击“步长”按钮调节单次运动的步进量，“滑轨”按钮可直接控制滑轨运动。<br/>
（2）角度控制模式<br/>
在Mirobot Studio中控制模式选择处选择“坐标运动模式”，选中后显示为白底高亮状态
Studio中控制模式选择处选择“角度运动模式”，选中后显示为白底高亮状态
<center><img src="http://lin88zhang.gitee.io/image/2/2-4.png" width="600"  > </center>
点击Mirobot Studio右侧的“X、Y、Z、RX、RY、RZ”控制按钮可以控制机械臂末端执行机构的空间位置与末端姿态。可通过“速度”按钮或输入值调节各轴运动速度，可点击“步长”按钮调节单次运动的步进量，“滑轨”按钮可直接控制滑轨运动。

##&diams; 点位示教-复现功能
第1步：单击示教选项卡
<center><img src="http://lin88zhang.gitee.io/image/2/2-5.png" width="600"  > </center>
第2步：点击Mirobot Studio右上角“控制模式”切换按钮可选择示教模式。
<center><img src="http://lin88zhang.gitee.io/image/2/2-6.png" width="600"  > </center>
第3步：以“角度控制模式”为例，控制机械臂各轴转动角度，当调整到一个满意的示教位置点时，点击“增加点位”按钮，增加示教点。继续调整机械臂的位置与姿态，点击“增加点位”按钮，增加第二个示教点、第三个示教点......，直到增加完所有的示教点。
<center><img src="http://lin88zhang.gitee.io/image/2/2-7.png" width="600"  > </center>
第4步：单击Mirobot Studio面板中的“运行”或“单步”按钮，可以实现所记录示教点的连续复现运动或示教点的单步运动。
界面下方的“删除”、“向下/上”、“撤销”、“复制”、“粘贴”按钮可实现记录示教点的删除、向上或向上移动、撤销记录、复制和粘贴示教点等功能。
<center><img src="http://lin88zhang.gitee.io/image/2/2-8.png" width="600" > </center>

##&diams; 设置界面介绍
<center><img src="http://lin88zhang.gitee.io/image/2/2-9.png" width="600"  > </center>
（1）设置串口：设置Mirobot Studio连接机械臂的串口和波特率（115200）<br/>
（2）绘制设置：设置绘画速度（推荐默认值）<br/>
（3）校准：用于校准机械臂<br/>
（4）重置：重置机械臂所有数据（重置后需要重新校准）<br/>
（5）语言：设置语言和字体（语言设置后点击确定自动重启软件生效，字体设置后点击确定手动重启软件生效）或者点击界面右上角“CN”按钮可以切换界面中英文。<br/>
<center><img src="http://lin88zhang.gitee.io/image/2/2-10.png" width="600"  > </center>
（6）末端工具选项：选择机械臂使用的末端工具和导轨/传动带模式
<center><img src="http://lin88zhang.gitee.io/image/2/2-11.png" width="600"  > </center>
（7）固件：更新固件，详细操作参考《Mirobot固件升级及校准》