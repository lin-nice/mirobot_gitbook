# <center>9. WLKATA Studio-Python编程指南</center>
##&diams; Python编程界面讲解
打开Mirobot Studio进入Python编程界面，下图中上方黄色矩形框内为代码文件操作区，左侧红色矩形框内为Python API选项区，右侧绿色框内为Python代码编辑区。
<font color="red">注：代码编辑区中默认的8行代码不可随意更改！</font>
<center><img src="http://lin88zhang.gitee.io/image/8/8-1.png" width="600"  > </center>
1.文件操作区
<center><img src="http://lin88zhang.gitee.io/image/8/8-2.png" width="600"  > </center>
&rArr; 新建：新建Pyhton文件<br/>
&rArr; 打开：打开本地文件<br/>
&rArr; 保存：保存文件，默认保存到data目录<br/>
&rArr; 另存为：将修改后的文件另存<br/>
&rArr; 运行：运行工作区中的代码<br/>
2.Python API选项区
整个控制区选项分为3大类（动作、角度控制、坐标控制），共计16个功能模块，双击可直接添加使用
<center><img src="http://lin88zhang.gitee.io/image/8/8-3.png" width="600"  > </center>
（1）动作选项<br/>
&rArr; 复位（api.home_simultaneous()）：执行Mirobot机械臂复位动作<br/>
&rArr; 解锁（api.unlock_shaft()）：解锁机械臂各关节<br/>
&rArr; 回归零位（api.go_to_zero()）：Mirobot机械臂由当前位置移动至角度控制模式下的零位<br/>
&rArr; 吸盘开（api.suction_cup_on()）：打开气泵<br/>
&rArr; 吸盘关（api.suction_cup_off()）：关闭气泵<br/>
&rArr; 滑轨移动到（api.slider_move_to(0, 1500)）：移动滑轨到指定位置<br/>
&rArr; 传送带移动到（api.conveyor_move_to(ConveyorMode.relative, 0, 1500))：移动滑轨到指定位置<br/>
&rArr; 延时执行（api.set_delay_time(1)）：延迟指定时间后执行下一项动作<br/>
（2）角度控制选项<br/>
&rArr; 将每个轴移动到特定位置（api.go_to_axis(0,0,0,0,0,0,1500)）：Mirobot机械臂由当前位置移动至角度控制模式下的指定位置<br/>
&rArr; 每个轴增量移动（api.increment_axis(0,0,0,0,0,0,1500)）：Mirobot机械臂由当前位置移动到指定位置<br/>
&rArr; 移动轴（api.move_to_axis(MirobotJoint.Joint1, RevolveDirection.cw, 0, 1500)）：单独指定某个轴向指定方向旋转指定数值<br/>
（3）坐标控制选项<br/>
&rArr; 移动到笛卡尔位置（api.go_to_cartesian_lin(202,0,181,0,0,0,1500)）：Mirobot机械臂由当前位置移动至坐标控制模式下的指定位置<br/>
&rArr; 笛卡尔空间中移动增量（api.increment_cartesian_lin(0,0,0,0,0,0,1500)）：Mirobot机械臂由当前位置向指定方向移动指定坐标数<br/>
&rArr; 定向移动（api.direction_mobility(MoveDirection.forward, 0, 1500)）：Mirobot机械臂由当前位置向指定方向单独移动指定坐标数<br/>
&rArr; 门型轨迹移动（api.jump_move(ConveyorMode.relative, 0, 0, 0, 1500)）：以门型轨迹移动至指定坐标点<br/>
&rArr; 圆弧轨迹移动（api.set_arc_move(MoveMode.relative, RevolveDirection.cw, 0, 0, 0, 60, 1500)）：以圆弧轨迹移动<br/>

##&diams; 示例
如以下代码功能
```
#version python 3.8
#coding=utf-8
from mirobot import *
from time import sleep
api=Mirobot()
#Please do not delete the above code
api.home_simultaneous()                 #机械臂复位
sleep(15)                               #延时15s
for i in range(10):                     #以下动作重复执行10次
    api.go_to_axis(30,0,0,0,0,0,1500)   #第一轴由零位以1500°/min旋转到绝对位置30
    api.go_to_axis(-30,0,0,0,0,0,1500)  #第一轴由零位以1500°/min旋转到绝对位置-30
api.go_to_zero()                        #回到零位
```

