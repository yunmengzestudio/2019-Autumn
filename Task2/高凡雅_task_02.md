# 第二期任务
****
## 问题一：一个正常的 Unity 工程目录下初步需要哪些基本文件夹
+ Assets
+ Library 缓存文件夹
+ ProjectSettings 配置信息
+ Tempty Obj 临时文件夹
## 问题二：两个物体之间若能发生碰撞，需要什么先决条件
1. 两个物体具有碰撞组件
2. 运动的物体有刚体组件
## 问题三：触发器函数（Trigger 与 Collider）有几种类型
+ Trigger函数
   1. OnTriggerEnter()函数:进入触发器区域的时候运行
   2. OnTriggerStay()函数:当其处在触发器区域的时候会运行
   3. OnTriggerExit()函数:当其离开触发器区域的时候会运行
+ Collider函数
   1. OncollisionEnter()函数
   2. OncollisioStay()函数
   3. OncollisionExit()函数
## 问题四:Start() 函数和 Update() 函数的作用
+ Start()函数脚本开始时运行且只运行一次
+ Update()函数每一帧都在作用
## 问题五：如何用脚本来控制 UI 层 Text 的变化
1. 添加UnityEngine.UI命名空间
2. 在脚本中定义text组件
3. 控制text组件
## 问题六:如何赋予一个物体速度（或使其动起来）
1. 在物体中添加刚体组件
2. 在物体上的脚本内声明Rigidbody组件
3. 在start()内得到刚体组件
4. 在Update()内调用Addforce指令（直接声明方向大小）

>·rd.AddForce(new Vector(0,0,1))`
## 问题七:如何获取到键盘按下事件
1. 在物体中添加刚体组件
2. 在物体上的脚本内声明Rigidbody组件
3. 在start()内得到刚体组件
4. 在Update()内调用Addforce指令

>`rb.AddForce(Input.GetAxis("Horizontal),0,0）;//左右移动`

>`rd.AddForce(0,0,Input.GetAxis("Vertival"));//前后移动`

>```
>if(Input.GetkeyDown(KeyCode.Space))
>  rb.AddForce(0,100,0);//上下移动
>```
(rd为刚体组件）
