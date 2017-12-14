# postgresql
PostgreSQL 列出所有表名和数据库名,删除数据库

列出当前数据库所有表

\dt

列出数据库名

\l   或者 select datname from pg_database;

切换数据库

\c 数据库名

查看表的字段

\d 表名

delete from testair;
