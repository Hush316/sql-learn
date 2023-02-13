## 数据库基础

1. 创建数据库  create database music_db;
2. 使用数据库 use music_db;
3. 创建表  create table  t_singer(name varchar(10) age int);
4. 展示表 show tables;
5. 插入数据  insert into t_singer (name,age) values ('kabuto',30);
6. 查找数据  select * from t_singer;


##  SQL语句
- 我们希望操作数据库(特别是在程序中),就需要有和数据库沟通的语言,这个语言就是SQL
  - SQL是Structured query Language,称之为结构化查询语言,简称SQL
  - 使用SQL编写出来的语句,就称之为SQL语句
  - SQL语句可以用于对数据库进行操作
- 事实上,常见的关系型数据库SQL语句都是比较相似的
- SQL语句的常用规范
  - 通常关键字使用大写,比如CREATE,TABLE,SHOW的等
  - 一条语句结束后,需要以;结尾
  - 如果遇到关键词作为表名或者字段名称,可以使用`包裹`


