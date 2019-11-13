# 江振江的答案.md
---
 * ## 问题1：Unity目录下需要哪些就基本文件夹  
   1. Assets（场景，材质，脚本） 2. Library 3.ProjectSettings
* ## 问题二：两个物体相撞需要哪些先决条件  
   1.刚体组件2.脚本控制（力 +键盘）
+ ## 问题三：触发器函数Trigger与Collider有几种类型  
   1.基本为三种（Enter进入，Exit退出，Stay逗留
+ ## 问题四:Start与Update函数的作用
   1.start定义初始化代码（一次）  
   2.update循环调用命令
+ ## 问题五：如何用脚本控制UI层Text的变化
   1.在视图下创建text在主角的脚本中定义text组件  
   2.另可定义wintext显示胜利语言
+ ## 问题六：如何赋予一个物体速度   
   1.创建脚本，start函数下获得刚体组件  
   2.update下调用指令AddForce,创建向量Vector
+ ## 问题七：如何获取键盘
   1.在Update下调用指令获得水平轴Horizontal和Vertial

   