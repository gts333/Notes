# Commands related to Data Definition Language  
## 对于数据库的操作
改变数据库字符集（及其不常用）alter database [database name] character set 'utf-8'  
## 对于表的操作
基于已存在的表创建新表 create table [tablename] as select a,b,c from .....  
重命名表 alter table [tablename] rename to [newname]  
添加表字段 alter table [tablename] add [column name] [column type] .... [LOCATION]; 其中LOCATION如果不加 默认添加到最后; 可以是first (添加到最开头)， after [column name] (在某个字段后面添加)  
修改表字段类型 alter table [tablename] modify [column name] [column type]
重命名字段 alter table [tablename] change [old column name] [new column name] [new column type]  
删除表字段 alter table [tablename] drop [column name]  
清空表 truncate table [tablename] (不可回滚) delete from [tablename] （可回滚）
## 插入一点点 DML
将查询结果插入进去 insert into empl select employee_id, last_name, hire_date, salary from employees  