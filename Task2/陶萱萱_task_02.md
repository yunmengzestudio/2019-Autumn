##问题1
####Assets,Library,ProjectSetting。
##问题2
####两物体都必须带有碰撞器，其中一个物体还必须带有Rigidbody刚体
##问题3
####Trigger:当进入触发器；当退出触发器；当逗留触发器。
####Collider：当进入碰撞器；当退出碰撞器；当逗留碰撞器。
##问题4
####start：仅调用一次。
####update：持续调用。
##问题5
####在小球脚本中定义一个text，将层级视图中text指定到检视视图，在小球代码中控制text
##问题6
####通过代码：
(```)
Start(){
rd=GetComponent<Rigidbody>();}
Update(){
rd.AddForce(new Vector3(1,0,1));}
(```)
##问题7
####通过代码：
(```)
Start(){
rd=GetComponent<Rigidbody>();}
Update(){
float h=Input.GetAxis("Horizontal");
float v=Input.GetAxis("Vertical");
(```)