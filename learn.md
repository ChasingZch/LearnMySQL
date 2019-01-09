# 学习MySQL
1. MySQL的安装：
- mac端直接用 homebrew 安装就可以了
- 命令为: 
``` brew install mysql ```
2. 在启动阶段常用的命令:
- 启动: 
``` mysql.server start ``` 
- 停止: 
``` mysql.server stop ```
- 操作 mysql :
``` mysql -uroot```
3. 如何使用作者提供的数据库:
- Step.1: 新建一个数据库: ``` create database crashcourse;``` 这里的 crashcourse 就是新建的 database 名称
- Step.2: 使用作者提供的 create.sql 建立一些表 ``` source /Users/mac/desktop/create.sql; ``` 在 source 后面给出作者所提供的 create.sql 的绝对路径
- Step.3: 使用作者提供的 populate.sql 填充数据库  ``` source /Users/mac/desktop/populate.sql; ``` 在 source 后面给出作者所提供的 populate.sql 的绝对路径
4. 实际操作常用的一些语法(mysql 要用 ; 或者 \g 来结束这一行的命令):
- 展示数据源，这样可以看到所有的数据库 ```show databases;```
- 使用数据源中的某个数据库 ```use crashcourse;``` crashcourse 就是你要使用的数据库的名称
- 显示当前所在的数据有很多种方法 ```status;``` ```show tables;``` ```select database();```
- 选中某一列 ```SELECT prod_id;``` SELECT + 列名
- 
