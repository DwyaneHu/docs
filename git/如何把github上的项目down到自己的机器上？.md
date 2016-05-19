### 如何把github上的项目down到自己的机器上？

----

#### 一、准备工作
1. 首先要有一个github的账号，并且最好完成了邮箱验证。
2. 在Personal Settings 的SSH keys中上传自己的公钥。
3. 创建一个本地的代码库文件夹，用来存放自己的代码。如果已有则忽略. 
4. 接下来就能愉快的从github上下载别人的项目啦。


#### 二、核心动作
	
	## 改变当前路径到自己的代码库路径
	cd ~/Documents/repo

	## 拿来主义
	git clone #{项目的ssh}

	## 如果该项目是maven管理的,则可以生成eclipse
	cd ./#{项目路径}
	mvn eclipse:eclipse
	
	
#### 三、在IDE中导入该项目

##### 点击`File` --> `import`--> `Existing Projects into Workspace `--> `select root directory `--> `finish` 