可选：根据 mybatis-generator/src/main/resources/testdb.sql 创建库表

1. 修改 mybatis-generator/src/main/resources/db-config.properties 配置信息
	
	主要包括：  数据库配置
			  mysql-connector-java.java 绝对路径
			  生成的 java model路径
			  生成的 java mapper 路径
			  生成的 xml  mapper 路径
			  
2. 根目录执行 mvn mybatis-generator:generate -f mybatis-generator/gen-pom.xml

3. 观察生成的文件信息

4. 根目录 mvn clean package  打包发布

注意：数据库命名规范为下划线（"_"）连接