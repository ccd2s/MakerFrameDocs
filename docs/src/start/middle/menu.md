---
title: 标题画面
author:
  name: 深林孤鹰
  url: https://github.com/leamus
icon: bars
order: 6
---

## 说明

&emsp;&emsp;系统没有专门的标题画面编辑器，但初学者可以用系统自带的简易标题画面（使用game.menu实现的）：

&emsp;&emsp;在游戏开始脚本可视化编辑器中，如果你删除了默认的  *start函数，则系统会自动生成一个默认的标题画面（包含 开始游戏、读取存档、游戏说明、制作人员 菜单），并将你的代码编译在“开始游戏”菜单中；如果有默认的 *start函数，则不会生成默认的标题画面。

&emsp;&emsp;当然你还可以用另外三种方法来制作。

&emsp;&emsp;1、使用地图和地图事件：

&emsp;&emsp;绘制的地图是整个界面，NPC可以是按钮。这个方案比较简单，适合初学者。

&emsp;&emsp;在地图start事件里加入一句：

game.scale(Math.min(game.\$sceneSize.width / game.\$mapSize.width ,game.\$sceneSize.height / game.\$mapSize.height))

&emsp;&emsp;便可以自适应屏幕。

&emsp;&emsp;2、使用game.showimage和game.showsprite：

&emsp;&emsp;这个命令是显示特效，特效也可以被点击，稍微比地图方案麻烦一点。

&emsp;&emsp;3、使用插件：

&emsp;&emsp;这个方案无疑是最强的也是最难的，只要你有想法和技术，任何界面你都可以做出来。
