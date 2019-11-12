# **一个正常的Unity工程目录初步需要哪些文件夹**
## 1. Assets
## 2. Library
## 3. Logs
## 4. Obj
## 5. Packages
## 6. ProjectSettings
----
#  两个物体之间若能发生碰撞，需要什么先决条件
## 都选中Collider组件
----
#  触发器函数（Trigger 与 Collider）有几种类型
## 三种：
### 1. 双方都有刚体，都有触发器，碰撞时各自执行碰撞脚本
### 2. 一方有刚体，另一方没有，有刚体的执行脚本
### 3. 都没有刚体，碰撞时会直接穿过去
---
#  Start() 函数和 Update() 函数的作用
## 1. Start()函数:提前赋值，创造环境
## 2. Update()函数:不断调用
---
#  如何用脚本来控制 UI 层 Text 的变化
## 当分数改变（或出现相关条件） text.text = score.ToString();
---
#  如何赋予一个物体速度（或使其动起来）
## AddForce(new Vector3(x, y, z) * force)
---
#  如何获取到键盘按下事件
## 1. Input.GetAxis("Horizontal")//水平按键
## 2. Input.GetAxis("Vertical")//垂直按键
---