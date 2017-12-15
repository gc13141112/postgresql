# postgresql
PostgreSQL 列出所有表名和数据库名,删除数据库

链接数据库：connection=psycopg2.connect(database='airquality',user='airquality',password='123456',host='127.0.0.1',port='5432')

|列出当前数据库所有表| 列出数据库名| 切换数据库 | 
|-------|-----|----|
|\dt |\l   或者 select datname from pg_database;|\c 数据库名|
|查看表的字段|删除表|保存为csv|
|\d 表名|delete from testair;|\copy testair to 'd:/test.csv with csv header;|

时间戳:https://www.cnblogs.com/alianbog/p/5654846.html

refer on :http://initd.org/pyscopg/docs

在本人机器上测试数据入库：

测试环境：

CPU: Intel(R) Core(TM) i5-7300HQ @2.50GHz, Memory: 8GB

测试速度：

1205.4s,一共224个csv文件,一共236M,入库记录4867793条,每条记录16个字段,平均每秒入库4056条记录(每条记录16列).

python是8个进程运行,参考地址https://www.cnblogs.com/yy3b2007com/p/5716907.html

| 测试案例 | 
| :---------------: | 
| ![](https://github.com/gc13141112/postgresql/raw/master/img/%E6%B5%8B%E8%AF%95%E8%BF%9B%E7%A8%8B.png) | 


