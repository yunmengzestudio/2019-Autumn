# 第一题:一个正常的 Unity 工程目录下初步需要哪些基本文件夹
- 需要的基本文件夹如图所示:

![Asset](https://img-blog.csdn.net/20170721202144549?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvQmVVbmlxdWVUb1lvdQ==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

# 第二题：两个物体之间若能发生碰撞，需要什么先决条件
- 两个物体都必须 ***带有碰撞器*** 或者 ***开启了碰撞效果***。
- 其中一个物体需 ***带有刚体性质***
- 必须 ***相对运动*** 才能导致碰撞

# 第三题：触发器函数（Trigger 与 Collider）有几种类型
## Trigger


  - 当绑定着碰撞器的游戏对象 ***进入触发器区域*** 的时候，会运行触发器对象上的 ***OnTriggerEnter()*** 函数
  - 当其 ***处在触发器区域*** 的时候会运行 ***OnTriggerStay()*** 函数，且每帧调用一次 ***OnTriggerStay()*** 函数
  - 当其 ***离开触发器区域*** 的时候会运行 ***OnTriggerExit()函数***

## Collider


  - 同理有 ***OnCollisionEnter()*** 、 ***OnCollisionExit()*** 、 ***OnCollisionStay()***

# 第四题： Start() 函数和 Update() 函数的作用
## start() 函数作用


  - 顾名思义是 ***初始化*** 的意思，是脚本刚开始的时候运行的，所以一般情况下只运行一次。

       <font color=red> ***PS:当Update函数第一次被调用前会先调用Start函数。*** </font>

## update() 函数作用C


  - 顾名思义是 ***更新*** 的意思,可以理解成像视频一样，任意一个打开的unity应用也是一帧一帧播放的，即使画面没有任何变化。
  - Update() 函数相当于是在说，每刷新一帧的时候，该做什么。

# 第五题：如何用脚本来控制 UI 层 Text 的变化
- 首先、需要将using UnityEngine.UI写入脚本头端
- 其次、定义一个public Text text
- 其次、将定义的public Text 带进函数中，并且写入你想要的表达式
- 然后、在unity中将你想要改变的text文本  拖入 定义的public执行框内

# 第六题：如何赋予一个物体速度（或使其动起来）
- 首先、需要一个物体（最好是球体）和 一个地板
- 其次、给物体添加刚体组件
- 其次、在物体的组件下 创建一个脚本
- 最后、在脚本内通过代码控制（在  建立的向量上的  某个方向上  施加力），使其能够运动

# 第七题：如何获取到键盘按下事件
- 用input.GetKeyDown( )方法将按键值作为参数，判断此按键是否被按下。
```
            if (Input.GetKeyDown (KeyCode.W))  
            {  
                Debug.Log("您按下了W键");  
            }  
              
            if (Input.GetKeyDown (KeyCode.S))  
            {  
                Debug.Log("您按下了S键");  
            }  
              
            if (Input.GetKeyDown (KeyCode.A))  
            {  
                Debug.Log("您按下了A键");  
            }  
              
            if (Input.GetKeyDown (KeyCode.D))  
            {  
                Debug.Log("您按下了D键");  
            }  
              
            if (Input.GetKeyDown (KeyCode.Space))  
            {  
                Debug.Log("您按下了空格键");  
```
# GIT教程等
[Git教程1](https://www.liaoxuefeng.com/wiki/896043488029600)

[Git教程2](https://www.runoob.com/git/git-tutorial.html)

[一个小时学会Git](https://www.cnblogs.com/best/p/7474442.html)

[Github的学习和使用](https://www.e-learn.cn/content/qita/974817)

[开源软件是什么？有哪些？](http://c.biancheng.net/view/2943.html)

[开源协议是什么？有哪些？如何选择?](http://c.biancheng.net/view/2947.html)

# Markdown 语法
[GitHub Flavored Markdown](https://www.jianshu.com/p/40ba812dd973)

[Mastering Markdown - Github Guides](https://guides.github.com/features/mastering-markdown)
# 坦克大战
- 血条的跟随与增减
- 简单的：AI状态机，行为树
- AI发射时间的调整（如：每过多少秒发车一次炮弹）
- 游戏声音的加入
# 坦克大战仓库地址
[源码](https://github.com/Deviltxx/xmhTanksWar)