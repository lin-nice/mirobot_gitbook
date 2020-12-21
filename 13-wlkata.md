# <center>14. 视觉套件组装说明</center>

<center><img src="http://lin88zhang.gitee.io/image/13/1.jpg" width="600"  > </center>

##&diams; 视觉套件构成
| 名称 | 数量 | 名称 | 数量 |
| :------: | :------: | :------: | :------: |
| 底板 | 1件 | M5×10圆柱头内六角 | 1颗 |
| 立柱连接件 | 1件 | M4×10圆柱头内六角 | 8颗 |
| 立柱 | 1件 | openMV | 1个 |
| 从支架横梁 | 1件 | LCD显示屏 | 1块 |
| M6×10（柄径25）手拧螺丝 | 1颗 | openMV屏幕连接线 |  |
| M4×8圆柱头内六角 | 5颗 | USB | 1根 |
| M5×12圆柱头内六角 | 1颗 | openMV串口线 | 1根 |
| 3×80mm 黑色扎带 | 4根 | 8×250黑色扎带 | 2根 |

<div align="center"><img src="http://lin88zhang.gitee.io/image/13/2.jpg" width="300"><img src="http://lin88zhang.gitee.io/image/13/3.jpg" width="300"></div>

<center><img src="http://lin88zhang.gitee.io/image/13/4.jpg" width="500"  > </center>

##&diams; 视觉套件的组装
**第一步：安装立柱连接件**<br/>
将底板取出，有凹槽面朝上；<br/>
使用M4×8圆柱头内六角将立柱连接件固定在底板上（<font color="red">注意：立柱连接件侧面螺钉孔朝向，其在底板安装位置最近的一边 </font>）<br/>

<center><img src="http://lin88zhang.gitee.io/image/13/5.jpg" width="500"  > </center>

**第二步：安装立柱**<br/>
将立柱插入立柱连接件并用M4×8圆柱头内六角将其固定（<font color="red">注意：有侧面圆孔的一段朝下，方向与立柱连接件方向一致</font>）<br/>

<center><img src="http://lin88zhang.gitee.io/image/13/6.jpg" width="500"  > </center>
<center><img src="http://lin88zhang.gitee.io/image/13/7.jpg" width="500"  > </center>

**第三步：安装从支架横梁**<br/>
将从支架横梁穿过立柱调整合适高度及角度（与底板中心线平行）（<font color="red">注意：从支架横梁有凹槽面朝向底板</font>）<br/>
用M6×10（柄径25）手拧螺丝将从支架横梁固定在立柱上<br/>

<center><img src="http://lin88zhang.gitee.io/image/13/8.jpg" width="500"  > </center>

**第四步：安装Lcd显示屏及openMV**<br/>
用M5×12圆柱头内六角将openMV固定在从支架横梁上<br/>
用M5×10圆柱头内六角将LCD显示屏固定在从支架横梁上<br/>
用openMV屏幕连接线连接openMV和LCD显示屏<br/>

<div align="center"><img src="http://lin88zhang.gitee.io/image/13/9.jpg" width="300"><img src="http://lin88zhang.gitee.io/image/13/10.jpg" width="300"></div>

<center><img src="http://lin88zhang.gitee.io/image/13/11.jpg" width="400"  > </center>
<center><img src="http://lin88zhang.gitee.io/image/13/12.jpg" width="400"  > </center>

**第五步：安装机械臂**<br/>
使用M4×10圆柱头内六角螺钉将机械臂（<font color="red">注意：机械臂方向</font>）<br/>

<center><img src="http://lin88zhang.gitee.io/image/13/13.jpg" width="500"  > </center>

##&diams; 线路的连接
**第一步：连接openMV灯板电源**<br/>

<center><img src="http://lin88zhang.gitee.io/image/13/14.jpg" width="400"  > </center>

**第二步：连接串口接口线**<br/>

<center><img src="http://lin88zhang.gitee.io/image/13/15.jpg" width="400"  > </center>

**第三步：连接USB线**<br/>

<center><img src="http://lin88zhang.gitee.io/image/13/16.jpg" width="400"  > </center>

**第四步：固定线路**<br/>
用3×80mm黑色扎带将openMV串口线固定到从支架横梁上<br/>
用8×250黑色扎带将openMV串口线固定到立柱上<br/>

<div align="center"><img src="http://lin88zhang.gitee.io/image/13/17.jpg" width="300"><img src="http://lin88zhang.gitee.io/image/13/18.jpg" width="300"></div>

**第五步：与机械臂的连接**<br/>
用IDC排线将机械与标有“EXTENDER BOX”字样的扩展模块连接<br/>

<center><img src="http://lin88zhang.gitee.io/image/13/19.jpg" width="400"  > </center>

将openMV串口线连接到标有“EXTENDER BOX”字样的扩展模块上的标有“5V RT TX GND”字样的接口<br/>

<center><img src="http://lin88zhang.gitee.io/image/13/20.png" width="400"  > </center>
<center><img src="http://lin88zhang.gitee.io/image/13/21.jpg" width="400"  > </center>

将openMV串口线另一端的电源接口连接到机械臂上<br/>
<center><img src="http://lin88zhang.gitee.io/image/13/22.png" width="400"  > </center>

将电源连接到openMV串口线<br/>
<center><img src="http://lin88zhang.gitee.io/image/13/23.png" width="400"  > </center>
