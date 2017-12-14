# postgresql
PostgreSQL 列出所有表名和数据库名,删除数据库
链接数据库：connection=psycopg2.connect(database='airquality',user='airquality',password='123456',host='127.0.0.1',port='5432')

|列出当前数据库所有表| 列出数据库名| 切换数据库 | 
|-------|-----|----|
|\dt |\l   或者 select datname from pg_database;|\c 数据库名|
|查看表的字段|删除表|
|\d 表名|delete from testair;|






