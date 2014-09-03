###业务规则
####免答权
免答权更新个人profile表积分(integrate)字段。

####闯关机制
闯关接口返回关数(数组形式)、组数(数组形式)，每组再加上难度。

接口提供的逻辑:每关的组数相同。(否则不好处理)
####排行榜
在第一行显示自己的排名。

####同步机制
新建个人信息表profile，同步个人信息数据。


####接口调试
根据调试接口的需要，增加表结构重构的工作量。加入到工作计划excel中。

###安全测试
稳定版安全测试与开发版安全测试如何进行以及界面美化的问题。

###2014-9-3
接口调用规则  	 	  	 	| 二级描述 			       |日期     | 状态
-----------------------| ---------------------|----|-----
1.上载错题、对题、收藏题   |bic001。"锦囊佳藏"、"修行进度"ready(检查是否修改后)      |嘉斌|
2.下载错题、对题、收藏题 	|bic002。同上           	|嘉斌|
3.下载闯关配置信息			|bic011。“单人闯关”ready(检查是否修改后)  |武仝|易。
4.下载成就积分对照表		|bic003。同上   	    	|嘉斌|易。
5.下载闯关排名信息			|bic004。"英雄榜-闯关"ready() |武仝|易。
6.下载总积分排名信息		|bic005。"英雄榜"ready()  |嘉斌|易。
7.上传闯关				|bic006。  				|武仝|
8.下载闯关				|bic007。  				|武仝|
9.登录记录接口			|bic008。首页ready()  	                |武仝|易。
10.下载题库				|bic009。  	        	                |嘉斌|
11.下载模拟考试配置		|bic010。"模拟考试"ready(检查是否修改后)   |嘉斌|易。
12.上传积分、成就、专业、模拟考试结果(个人信息)	|bic012。"设置"ready()、首页“定时”  |嘉斌|
13.下载积分、成就、专业、模拟考试结果(个人信息)	|bic013。"设置"ready()、首页“定时”  |嘉斌|
14.下载专业配置			|bic014。"设置"ready(检查是否修改后后)     |武仝|易。

###2014-8-25 
业务规则 	 	  	 | 二级描述 			       |日期     | 状态
------------------------| ------------------------|-----|-----
1.免答权是用总积分兑换	| 业务确认   				|8-25    |ok
2.星期一发包			|    				   		|8-22    |
3.生产版本shell对苹果的支持|注意点:js加载顺序    	|8-28 嘉斌|
4.苹果IOS1.0.0版本检测	|    					|8-29 嘉斌|
5.表结构调整工作量评估		| 3个工作日   			|8-29 武仝|
6.PK功能直接将两个文件夹考入|    					|8-31 嘉斌|

###2014-8-22 
掌上安规服务器端 	 	  	 | 二级描述 			       |日期     | 状态
------------------------| ------------------------|----|-----
1.闯关答题加入难度、题型配置|  		  				   |8-22|-----
2.星期一发包				|    				   	   |8-22|-----


###2014-8-11 
掌上安规服务器端 	 	  	 | 二级描述 			       |日期     | 状态
------------------------| ------------------------|----|-----
1.根据国网题库excel生成SQL题库|    				   |8-11|-----


###2014-8-22
接口部分  	 	  	 	| 二级描述 			       |日期     | 状态
------------------------| ------------------------|----|-----
1.数据库文件夹不要用test.改为。        |  db/zsag.sqlite      |8-11武仝|-----
2.我的错题、对题、收藏改为myquestions 	|  方法封装             |8-13嘉斌|-----
3.专业设置为professional 			|  树型结构，目前支持2级  |8-13武仝|-----
4.profile里面专业 major改为professional	|    	           |8-13嘉斌|-----
5.积分成就对换							|    	           |8-13嘉斌|-----


###2014-8-11 
掌上安规代码优化  	 	  	 | 二级描述 			       |日期     | 状态
------------------------| ------------------------|----|-----
1.数据库文件夹不要用test.改为。        |  db/zsag.sqlite      |8-11武仝|-----
2.我的错题、对题、收藏改为myquestions 	|  方法封装             |8-13嘉斌|-----
3.专业设置为professional 			|  树型结构，目前支持2级  |8-13武仝|-----
4.profile里面专业 major改为professional	|    	           |8-13嘉斌|-----
5.积分成就对换							|    	           |8-13嘉斌|-----
6.苹果我的收藏有问题，cordova.js放在public.js之前|	           |8-27嘉斌|-----






###2014-8-1 
掌上安规  	 	  	 | 二级描述 			       |日期     | 状态
------------------------| ------------------------|----|-----
1.错题回顾的逻辑 	 |只记录自由练习中三种题型的错题    |8-1|-----
2.进度统计 	     |只记录自由练习中三种题型的错题    |8-1|-----
3.2万条数据测试数据 |    							|8-1|-----
4.答案显示时候底部提升 |    						|武仝8-6|8-8.OK.
5.专业设置的可扩展性及接口的支持 |闯关排行根据服务器按专业返回的结果进行展现(闯关排行的tab是动态根据专业显示的)并同步到数据库    					|武仝8-6|-----
6.答案显示时候底部提升 |    						|武仝8-6|8-8.OK.



###2014-7-29
掌上安规  	 	  	 | 二级描述 			       |日期     | 状态
------------------------| ------------------------|----|-----
1.自由练习中左右可以滑动移位 | ssssssssssssssssss      |7-28|因为设置了固定宽度。去掉OK。
2.自由练习中js代码优化 	 | 需要加入 alert()才能成功   |7-26     | 
3.进度统计 				 | 需要上一步解决才行	        |7-28 嘉斌|
4.专业分类，要体现在切换专业后题目不一样| Content Cell   |7-28 嘉斌|8月12日。OK
5.目录结构清理，非项目文件放到doc目录下 | Content Cell   |        |7-29。OK
6.userId用户id的取法      | Content Cell  		    |7-29 嘉斌|
7.接口方法的重写  			 |   	|7-29|
8.发布包测试 			 	| 7月30日发布包|7-30|7-30.OK
9.调用"进度统计"函数应该统一  	| 业务调整--仅在 自由练习里面进行"进度统计"|7-30嘉斌|
10.操作数据库未完时，页面跳转会导致数据库阻塞 | 重点不要过多的进行页面跳转(操作数据库时)  		    |    |
Content Cell  			 | Content Cell  		    |    |

###2014-7-29 界面问题
掌上安规  	 	  	 | 二级描述 			       |日期     | 状态
------------------------| ------------------------|----|-----
1.米3,PK进度条有黑色痕迹 	 |暂不处理	  |7-29|-----
2.案例分析超长题显示问题 	 |暂不处理 嘉斌|7-31|-----

2.案例分析


###2014-7-31 总结
掌上安规  	 	  	 | 二级描述 			       |日期     | 状态
------------------------| ------------------------|----|-----
1.取用户ID的时候cordova.js放在public.js前面 	 |比较重要|7-31|-----



http://cp.londit.com

号164909的 

ftp :lq0PJ8Xd 

wbi8awMR请登录成功后

## 2014-1-19
1.  ldap 控制台 编辑可操作
2.  osx 虚拟机

## 2014-1-16
1.  /etc/openldap/slapd.conf

1月16日 执行结果
[root@hadoopside certs]# ls -s /etc/pki/tls/certs/slapd.pem /etc/openldap/certs/slapd.pem
0 /etc/openldap/certs/slapd.pem  4 /etc/pki/tls/certs/slapd.pem



## 2014-1-10
1.  安装gitblit.
2.  sdf
3.  ll
4.  l
3.  

## 2014-1-9
1.  kft-activiti 1.7.0 版本 用的是activiti哪个版本。
2.  改包名。
3.  丁德详 dingeai
4.  工作电脑装gitserver


## 2013-12-27
1.  sonatype nexus develop group
2.  o-my-shell git上 "x"是什么意思


## 2013-12-24
1.  sonatype nexus desvelop group
2.  o-my-shell git上 "x"是什么意思
3.  咖啡兔版本跑通activiti-5.1.4
4.  


## 2013-12-23
1.  ss4 mysql版本跑起来
2.  编译生成的项目
3.  


## 2013-12-22
1. git 先 checkout 一个tag为branch
2. quickstart mysql
3. git 离线手册


## 2013-12-20
1. mac 虚拟机安装
2. 虚拟机安装
3. mac 查看磁盘使用量 进程 


## 2013-12-19
1. springside4项目生成
2. 生成自定义路径项目
3. mysql版本
4. activiti项目
5. [maven 私服设置](http://www.blogjava.net/xiaomage234/archive/2012/11/22/391770.html)

## 2013-12-18
1. java7 安装 适应 nexus oss
2. [370kan](http://www.370kan.com/)
3. iTerm2 类似 putty的功能
4. firefox为什么 安装了没用 homebrew安装	
5. Sublime Text3


# 2013-12-17
1. test
2. php rpm install
3. mac mnmp 安装参数
4. bugfree xp上安装 PC机器实验
5. nexus oss war 包部署 tomcat或jetty
6. To have launchd start nexus at login:
    ln -sfv /usr/local/opt/nexus/*.plist ~/Library/LaunchAgents
Then to load nexus now:
    launchctl load ~/Library/LaunchAgents/homebrew.mxcl.nexus.plist
Or, if you don't want/need launchctl, you can just run:
    /usr/local/opt/nexus/libexec/bin/nexus start


## 2013-12-16
1. brew intall phpmyadmin
2. nexus oss install
3. joomla 		开发框架
4. springside	
5. jetty demo 	跑通
6. activiti 	跑通
7. joomla 		相册
8. mac scp
9. mac ssh

# 2013-06-18
1. 关键字 ant warning: sun.management.ManagementFactory is Sun proprietary API and may be removed in a future release  
2. 

## 2013-05-09
1. bootstrap bundle

## 2013-05-08
1. git commit -m "中文" --用小乌龟
2. 

## 2013-05-06
1. 单点登录 互联网。
2. 

http://www.stumbleupon.com/su/27XjEs?email=qinkun1234%40163.com&type=touch-recommend-weekly&variant=default
## 2013-02-24
1. yui-compress。

## 2013-02-17
1. 9.42 上安装ftp服务器。(OK--装到 43.82上面)
2. c/wamp/www目录需要经常执行以上命令。

## 2013-01-20
1. 重要的命令 git push orgin master/ git pull origin master。
2. c/wamp/www目录需要经常执行以上命令。

## 2013-01-13
1. jnuc093-springside4导出为 笔记本本地 s4项目 切换到新v4rc_v1项目

## 2013-01-14
1. 笔记本上数据库 设置为wtr
2. pom 暂时注释掉 httpclient
3. 台式机上 加上面的jar 包
4. 台式机上加 http://files.couchbase.com/maven2/spy/spymemcached/ 私服外挂----Testing
5. 

## 2013-01-13
1. jnuc093-springside4导出为 笔记本本地 s4项目 切换到新v4rc_v1项目

## 2013-01-12
1. exit-web-framework 生成eclipse项目

## 2013-01-03
1. git 如何 push request

## 2012-12-23
1. git 删除的文件如何提交

## 2012-12-22
1. michaelfly0621@hotmail.com(168502345)--kettle
2. mvn tomcat:run -Dmaven.tomcat.port=8088
3. 
4. 
5. 



## 2012-12-21
1. [memcached win客户端 会自动启动不要再启!](http://neo.com/)

## 2012-12-19
1. [neo](http://neo.com/)

## 2012-12-17
1. [运行 showcase先要上传 springside-extension-4.0.0.RC4.jar包](blog/activiti.md)

## 2012-12-17
1. [git pull origin v4RC](http://stackoverflow.com/questions/4235964/what-can-i-do-when-git-push-fails-with-local-out-of-date)--OK

## 2012-12-15
1. [git图形客户端](blog/activiti.md)

## 2012-12-14
1. [笔记本上 SpringSide RC4跑通](blog/activiti.md)--将regository清空,用代理重下在--OK
2. [将SpringSide RC4切换到 mysql](https://github.com/springside/springside4/blob/master/examples/quickstart/src/main/resources/sql/mysql/schema.sql)--用master版本下的schema.sql和import-data.sql脚本执行--OK

## 2012-12-13
1. [如何为 maven项目 添加一个公用的maven仓库地址](blog/activiti.md)----待解决
2. [mvn -Dmaven.surefire.debug test](http://maven.apache.org/plugins/maven-surefire-plugin/examples/debugging.html)


## 2012-12-12
1. [SpringSide RC4 项目跑通--OK](blog/activiti.md)
2. [基于上面DEMO 实现个ROP 项目 PDF链接](http://www.iteye.com/topic/1125834)

## 2012-12-11
1. [Sublime Text 2.0.1 注册 UTF-8版本 在微盘](www.hao123.com)                
2. [maven 结构 项目  参考 咖啡兔]             (www.hao123.com)                

demo

## jqgrid
[jqgrid event](http://www.trirand.com/jqgridwiki/doku.php?id=wiki:events)

[jqgrid select](http://www.trirand.com/blog/phpjqgrid/examples/selection/selectedrow_client/default.php)


[jqSuitePHP jquery-ui-bootstrap](http://127.0.0.1/demo/project/jqSuitePHP_4_4_2_0/)



* restlet 问题
[ERROR] Failed to execute goal on project activiti-webapp-rest2: Could not resol
ve dependencies for project org.activiti:activiti-webapp-rest2:war:5.10: The fol
lowing artifacts could not be resolved: org.restlet.jee:org.restlet:jar:2.0.15,
org.restlet.jee:org.restlet.ext.servlet:jar:2.0.15, org.restlet.jee:org.restlet.
ext.jackson:jar:2.0.15, org.restlet.jee:org.restlet.ext.fileupload:jar:2.0.15: C
ould not find artifact org.restlet.jee:org.restlet:jar:2.0.15 in 127 (http://127
.0.0.1:8081/nexus/content/groups/public/) -> [Help 1]



