# DevOps-Project-SpringBootApplication-rediscache-MySQLDB
![image](https://github.com/kamalmohan217/DevOps-Project-SpringBootApplication-rediscache-MySQLDB/assets/128888356/3e69b205-a5e1-48e0-a7bb-ddea919ade07)
<br><br/>
1. Clone source code present in repo https://github.com/kamalmohan217/spring-redis-cache-mysql.git as shown in screenshot below
![image](https://github.com/kamalmohan217/DevOps-Project-SpringBootApplication-rediscache-MySQLDB/assets/128888356/b61942f3-21e5-488d-affb-51655cec8583)
2. Now connect to the MySQL database and create database and table as required for the project.
![image](https://github.com/kamalmohan217/DevOps-Project-SpringBootApplication-rediscache-MySQLDB/assets/128888356/fbdff5bc-3b7e-4387-bbf9-fe0f4065064b)
![image](https://github.com/kamalmohan217/DevOps-Project-SpringBootApplication-rediscache-MySQLDB/assets/128888356/340b5dcb-91e8-4f77-b128-ac6646704918)
![image](https://github.com/kamalmohan217/DevOps-Project-SpringBootApplication-rediscache-MySQLDB/assets/128888356/533263d8-e51e-4b98-9a90-181c6d5b4bc2)
![image](https://github.com/kamalmohan217/DevOps-Project-SpringBootApplication-rediscache-MySQLDB/assets/128888356/5ca41da0-2cac-4044-94d8-3392be2c43cc)
3. Do the entry in the file spring-redis-cache-mysql/src/main/resources/application.properties for spring.datasource.url, spring.datasource.username and spring.datasource.password as shown in the screenshot below.
![image](https://github.com/kamalmohan217/DevOps-Project-SpringBootApplication-rediscache-MySQLDB/assets/128888356/d6af64b1-850c-4c7c-8e20-6fbf4129e170)
4. Do the entry in the file spring-redis-cache-mysql/src/main/java/com/springredis/cache/SpringRedisCacheApplication.java for Redis hostname, Redis Port and Redis primary key.
![image](https://github.com/kamalmohan217/DevOps-Project-SpringBootApplication-rediscache-MySQLDB/assets/128888356/a3ff0fc7-b1ad-4209-be43-9f328995d606)
5. Build the Code using Maven as shown in the screenshot below
![image](https://github.com/kamalmohan217/DevOps-Project-SpringBootApplication-rediscache-MySQLDB/assets/128888356/daf8c7b6-c42c-4996-9a6c-6fda029ac179)
6. Start the Spring Boot Application as shown in screenshot below
![image](https://github.com/kamalmohan217/DevOps-Project-SpringBootApplication-rediscache-MySQLDB/assets/128888356/4e28760a-073c-4c48-b6a0-faddc6824632)
7. Now use POST method for entry into the table items from POSTMAN as shown in screenshot below
![image](https://github.com/kamalmohan217/DevOps-Project-SpringBootApplication-rediscache-MySQLDB/assets/128888356/96ae74c7-4819-44c4-ad8b-e4855bc5d58b)
8. Checked from database and found entry is present in the database table as shown in the screenshot below
![image](https://github.com/kamalmohan217/DevOps-Project-SpringBootApplication-rediscache-MySQLDB/assets/128888356/b90da209-955a-46ab-93ac-7735bc5d1b4c)
9. Now Access the entry using GET method from POSTMAN and record the time as shown in the screenshot below
![image](https://github.com/kamalmohan217/DevOps-Project-SpringBootApplication-rediscache-MySQLDB/assets/128888356/25eed2b0-054b-434e-af7e-65570228b0ab)
This is the first time we are accessing the data So Application will connect to database and provide the result and you can see from screenshot below the time taken 669ms.
10. Finally Access the entry second time using GET method from POSTMAN and record the time as shown in the screenshot below 
![image](https://github.com/kamalmohan217/DevOps-Project-SpringBootApplication-rediscache-MySQLDB/assets/128888356/490f1926-6eb0-45d3-a16c-1dd591136eba)
This time when we access the data then SpringBoot Application will connect with Redis cache and provide the data and hence the time taken is less.
<br><br/>
The motive of this project is to show the advantage of implementing Redis Cache with MySQL database in an Application. Whenever we query any data then Application will connect with the Redis Cache and if it doesn't find the data in cache then it will connect with database and get the data. After geting the data from database it will make an entry in the Redis Cache for the same. So that next time if same data will be queried then Application will conect with Redis Cache and get the data rather than connecting with the database and get the data and hence the latency for the request has been reduced.

<br><br/>
<br><br/>
<br><br/>
<br><br/>
<br><br/>
<br><br/>
<br><br/>
```
Source Code:- https://github.com/kamalmohan217/spring-redis-cache-mysql.git
```
<br><br/>
<br><br/>
<br><br/>
<br><br/>
<br><br/>
<br><br/>
<br><br/>
```
Reference:-  https://github.com/souravkantha/spring-redis-cache.git
```
