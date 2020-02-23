第二次考核
=========
1.一个正常的Unity工程目录下初步需要的文件夹为：
+ Assets
+ Library
+ ProjectSettings
+ Temp Obj

2.两个物体能碰撞的先决条件是：
+ 两个物体都添加了collider
+ 有一方添加了刚体组件

3.触发器有几种函数：六种
+ OnCollisionEnter
+ OnCollisionExit
+ OnCollisionStay
+ OnTriggerEnter 
+ OnTriggerExit
+ OnTriggerStay

4.Start() 函数和 Update() 函数的作用：
+ Start()用于放置初始化的代码，只调用一次
+ Update()用于放置命令，且持续调用

5.如何用脚本来控制 UI 层 Text 的变化：
+ 引入命名空间using UnityEngine.UI
+ 使用ToString()函数

6.如何赋予一个物体速度（或使其动起来）
+ 给该物体添加刚体组件，使其有物理效果
+ 创建脚本
+ 编写初速度代码
+ 将C#脚本赋予该物体
+ 改变force大小以改变速度大小

7.如何获取到键盘按下事件
+ 在update()中得到左右按键 float h=Input.GetAxis("Horizontal")
+ 将x轴改为变量h
+ 得到前后键float v=Input.GetAxis("Vertical")
+ 将z轴改为变量v
