# maven_config

搭建公司内部maven环境使用的配置

   1.	settings.xml:Maven配置
   	
   		替换开发者本地maven/conf下的settings.xml（推荐原settings.xml备份），使用前请把IP修改为本地私服IP地址。
   
   2. pom.xml:方便共同属性在所有项目共用以及构件发布的配置：
   
   		*. 以下需修改(推荐放在单个文件中) 
		 	groupId
		  	artifactId
		  	name
		  	涉及到的IP
		  	JDK版本视公司环境不同自行修改
		  	
      	*. 修改后，执行以下命令上传到本地私服
        	mvn deploy -N
