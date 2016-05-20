## Maven 常用命令

```
mvn help:describe -Dplugin=pluginName -Dgoal=goalName
mvn archetype:generate 
	
# 不用eclipse理的tomcat来运行项目
mvn tomcat:run -Dmaven.tomcat.port=9090
#其它关联项目有过更新的话,一定要在项目根目录下运行mvn clean install来执行更新
mvn clean install
```






