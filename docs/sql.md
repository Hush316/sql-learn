# 数据库基础

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

## SQL 的数据类型

**MySql 支持的数据类型有:数据类型,日期和时间类型,字符串(字符和字节)类型,空间和 JSON 数据类型**

1. 数字类型

- 整数数字类型:INTEGER,INT,SMALLINT,TINYINT,MEDIUMINT,BIGINT;
- 浮点数字类型:FLOAT,DOUBLE(FLOAT 是 4 个字节,DOUBLE 是 8 个字节)
- 精确数字类型:DECIMAL,NUMERIC(DECIMAL 是 NUMERIC 的实现形式)

2. 日期类型

- YEAR 以 YYYY 格式显示值
  - 范围 1901 到 2155,和 0000
- DATE 类型用于具有日期部分但没有时间部分的值
  - DATE 以格式 YYYY-MMMM-DD 显示值
  - 支持的范围是'1000-01-01'到'9999-12-31'
