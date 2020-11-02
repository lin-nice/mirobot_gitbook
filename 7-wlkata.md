# <center>8. WLKATA Studio-Blockly编程指南</center>
##&diams; Blockly图形化编程界面讲解
打开Mirobot Studio进入Blockly图形化编程界面，下图中中间黄色矩形框内为图形化编程工作区，右侧绿色框内为Python代码显示区。可拖动分界轴调整工作区大小或隐藏代码生成区
<center><img src="http://lin88zhang.gitee.io/image/7/7-1.png" width="600"  > </center>
1.基础功能
<center><img src="http://lin88zhang.gitee.io/image/7/7-2.png" width="600"  > </center>
&rArr; 新建：新建文件夹<br/>
&rArr; 打开：打开本地文件<br/>
&rArr; 保存：保存文件，默认保存到data目录<br/>
&rArr; 另存为：将修改后的文件另存<br/>
&rArr; 导出：将Gcode导出到本地文件夹<br/>
&rArr; 下载：下载Gcode到机械臂分控板<br/>
&rArr; 运行：运行工作区中的代码<br/>
&rArr; 单步：选中工作区一个代码块，单步该条代码<br/>
2.Blockly编程模块
<center><img src="http://lin88zhang.gitee.io/image/7/7-3.png" width="600"  > </center>
动作选项中Mirobot常用编程代码块共有14个，分别为：<br/>
&rArr; 复位：Mirobot机械臂复位动作。<br/>
&rArr; 回归零位：Mirobot机械臂由当前位置移动至角度控制模式下的全零位置。<br/>
&rArr; 延迟下发（）秒：程序延迟指定时间后下发下一条指令。<br/>
&rArr; 延时执行（）秒：延迟指定时间后执行下一条指令。<br/>
&rArr; 移动到坐标：Mirobot机械臂由当前位置移动至坐标控制模式下的指定位置。<br/>
&rArr; 向（前/后/上/下）移动（）速度（）：由当前位置向指定方向移动指定坐标数（前、后、左、右、上、下）。<br/>
&rArr; 吸盘（开/关）：控制吸盘的打开或关闭。<br/>
&rArr; 夹具（开/关）：控制夹具的打开或关闭。<br/>
&rArr; 滑轨移动到（）速度（）：控制滑轨向指定位置移动。<br/>
&rArr; 传送带移动带（相对位置/绝对位置）速度（）：控制传送带向指定位置移动。<br/>
&rArr; 旋转到：Mirobot机械臂由当前位置移动至角度控制模式下的指定位置。<br/>
&rArr; （关节X）延（逆/顺）旋转（）：指定Mirobot机械臂指定关节顺时针或逆时针移动指定坐标。<br/>
&rArr; 门型轨迹移动：以门型轨迹移动到指定的相对或绝对位置。<br/>
&rArr; 圆弧轨迹移动：以弧形轨迹移动的要求绘制弧线<br/>
##&diams; 拖拽拼接代码块让机械臂动起来
<center><img src="http://lin88zhang.gitee.io/image/7/7-4.png" width="600"  > </center>
动作说明：<br/>
&rArr; 对机械臂进行复位<br/>
&rArr; 让以下动作循环执行10次<br/>
&rArr; 让机械臂从复位后的“零位”以1500mm/min速度移动到A点，坐标为“X202Y0Z20”，末端姿态不变<br/>
&rArr; 机械臂从A点以1500mm/min速度移动到B点，坐标为“X202Y0Z200”，末端姿态不变<br/>
&rArr; 机械臂从B点以1500mm/min速度回到零点位置<br/>
&rArr; 将机械臂第一轴以1500°/min速度旋转到绝对位置+20°<br/>
&rArr; 机械臂第一轴以1500°/min速度旋转到绝对位置-20°<br/>
&rArr; 机械臂回归零位<br/>



