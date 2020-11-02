# <center>11. Mirobot激光雕刻教程</center>
##&diams; 激光雕刻头安装与连接
第1步：将激光头固定在笔架上
<center><img src="http://lin88zhang.gitee.io/image/10/10-1.png" width="350"  > </center>
第2步：用扳手将笔架固定在机械臂的末端
<center><img src="http://lin88zhang.gitee.io/image/10/10-2.png" width="600"  > </center>
第3步：将扩展模块（背面标有“EXTENDER BOX”字样）用IDC排线与机械臂扩展通信接口连接。
<center><img src="http://lin88zhang.gitee.io/image/10/10-3.png" width="600"  > </center>
第4步：连接扩展模块、 PWM 电子开关以及激光雕刻头
<center><img src="http://lin88zhang.gitee.io/image/10/10-4.png" width="600"  > </center>

##&diams; 软件安装
第1步：登录网址http://www.cncbox.cn/s_soft/92.html 下载微雕大师软件安装包。
<center><img src="http://lin88zhang.gitee.io/image/10/10-5.png" width="600"  > </center>
第2步：安装微雕大师软件
<center><img src="http://lin88zhang.gitee.io/image/10/10-6.png" width="600"  > </center>

##&diams; 让Mirobot开始激光打印
第1步：打开微雕大师软件，在“连接机器”处找到机械臂对应的串口，然后点连接。
<center><img src="http://lin88zhang.gitee.io/image/10/10-7.png" width="600"  > </center>
第2步：在下部的指令输入行中，首先输入$H 指令，点击发送，让机械臂执行复位操作。
<center><img src="http://lin88zhang.gitee.io/image/10/10-8.png" width="600"  > </center>
第3步：在命令行输入：$41=150，点击发送，设置一个进行激光雕刻的必要参数。
（注意：机械臂完成雕刻后，正常使用时，须设置该参数为$41=0，否则机械臂将无法正常工作！）。
<center><img src="http://lin88zhang.gitee.io/image/10/10-9.png" width="600"  > </center>
第4步：在命令行输入：M20，切换机械臂为笛卡尔坐标模式。
<center><img src="http://lin88zhang.gitee.io/image/10/10-10.png" width="600"  > </center>
第5步：在命令行输入：Z70F2000，调整激光头高度。
<center><img src="http://lin88zhang.gitee.io/image/10/10-11.png" width="600"  > </center>
第6步：在激光头下方铺放一张雕刻专用纸板，佩戴激光护目镜。点击软件中的“强光“按钮，此时激光头被打开。用手拧激光头头部的调焦旋钮，使激光在纸板上形成一个最小最亮的光斑。点击软件中的关闭按钮，关闭激光，准备开始雕刻。
<center><img src="http://lin88zhang.gitee.io/image/10/10-12.png" width="600"  > </center>
第7步：点击软件中的“雕刻图形”，选择一张要雕刻的图片。
<center><img src="http://lin88zhang.gitee.io/image/10/10-13.png" width="600"  > </center>
第8步：在这个界面设置雕刻的速度，一般速度不超过 2000。推荐设置：尺寸 60*60，逐点雕刻， 每毫米内雕刻 6 行，每个点雕刻 160 毫秒。
<center><img src="http://lin88zhang.gitee.io/image/10/10-14.png" width="600"  > </center>
第9步：设置起点为“左下“，然后点击开始按钮。激光雕刻开始进行，等待到结束即可。
<center><img src="http://lin88zhang.gitee.io/image/10/10-15.png" width="600"  > </center>