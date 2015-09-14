# JSF-Primefaces-Spring-Integration

Java ,JSF, Primefaces, Spring, Spring Security, Mybatis, Login Example + Templates

PreBuild Steps :

	1. Create Database : Run/Import CreateDatabase.sql (sk-app-db\CreateDatabase.sql)

	2. Edit : sk-app-db\src\main\resources\spring-config.xml
			: Line 19 Host_Database:Port/Schema_&_Database_Name
			: Line 20 Username to Database
			: Line 21 Password to Database

![db_Connect](http://s14.postimg.org/7o2yoriwh/db_Connect.jpg)

Build :
	
	1. Build sk.app.db - First we need compile sk-app-db.jar  -  mvn clean install
	
	2. Build sk.app.core - mvn clean install

Deploy

	1. You can deploy war File to any Application Server
	
	2. Run from console : mvn clean install -P jetty
						: localhost:9999
						: You can find Jetty Configuration in pom.xml - line 126
