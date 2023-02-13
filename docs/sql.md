## 数据库基础

1. 创建数据库 create database music_db;
2. 使用数据库 use music_db;
3. 创建表 create table t_singer(name varchar(10) age int);
4. 展示表 show tables;
5. 插入数据 insert into t_singer (name,age) values ('kabuto',30);
6. 查找数据 select \* from t_singer;

## SQL 语句

- 我们希望操作数据库(特别是在程序中),就需要有和数据库沟通的语言,这个语言就是 SQL
  - SQL 是 Structured query Language,称之为结构化查询语言,简称 SQL
  - 使用 SQL 编写出来的语句,就称之为 SQL 语句
  - SQL 语句可以用于对数据库进行操作
- 事实上,常见的关系型数据库 SQL 语句都是比较相似的
- SQL 语句的常用规范
  - 通常关键字使用大写,比如 CREATE,TABLE,SHOW 的等
  - 一条语句结束后,需要以;结尾
  - 如果遇到关键词作为表名或者字段名称,可以使用`包裹`

## SQL 语句的分类

**常见的 SQL 语句我们可以分成四类**

- DDL(Data Definition Language):数据定义语言;
  - 可以通过 DDL 语句对数据库或者表进行:创建,删除,修改等操作
- DML(Data Manipulation Language):数据操作语言
  - 可以通过 DML 语句对表进行:添加,删除,修改等操作
- DQL(Data Query Language):数据查询语言
  - 可以通过 DQL 语句从数据库中查询记录(重点)
- DCL(Data Control Language):数据控制语言
  - 对数据库,表格的权限进行相关访问控制操作

## 常见的语句

-- 1.查看当前所有的数据库
SHOW DATABASES;

-- 2.使用某一个数据库
USE music_db;

-- 3.查看目前哪一个数据库是选中状态(就是正在使用的数据库)
SELECT DATABASE();

-- 4.创建一个新的数据库
CREATE DATABASE IF NOT EXISTS test_demo;

-- 5.删除某一个数据库
DROP DATABASE IF EXISTS test_demo;

-- 6.修改数据库(了解)
