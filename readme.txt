


Host配置：
1.	将pinx.plw放入IDA 的plugins目录（启动该插件的快捷方式是alt+f9或者在插件菜单栏中找到pinx）
2.	配置环境变量名%IDA%，值是:[IDA目录]/idavm.cmd
3.	Vmware根目录加入Path环境变量里
4.	在IDA根目录下新建idavm.cmd,内容为:
Vmrun -gu <username>  -gp <password> copyFileFromHostToGuest <vmx文件路径>	
=============
Guest配置：
1.	将guest下pin文件夹与工具放入 C:\

=======
使用步骤：
加载完样本后:
1.	启动插件，
2.	点击RunFile
3.	如果第二步不出问题，会在目录下生产x.cmd
4.	点击x.cmd，样本会运行起来
5.	获取虚拟机ip然后写入ip栏，点击connect，之后会获取api trace的信息，api  trace窗口。当样本运行结束之后，会获取动态字符串。
=========

使用过程中有什么问题可以微博联系：@f4ck_gfw
