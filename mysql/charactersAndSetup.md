# #是单行注释 /* */ 是多行注释
# 字符串和数值进行比较时 会自动将字符串转换为数值 转换失败则转为0
# 任何带null的运算 比较 查询 结果均为 NULL 除非使用安全等于
# 安全等于 <=> 如果一边是NULL 则结果为0 如果都为NULL 则结果是1
# 转义符\
# 字符串和日期用单引号 别名用双引号 自定义的字段和保留字冲突时用斜引号
# 推荐 SQL关键字 函数名 绑定变量都大写  
<br><br><br>

# 修改字符集, 在 my.ini文件中
[mysql]  
在63行左右 添加  
default-character-set=utf8  

[mysqld]  
在76行左右 添加  
character-set-server=utf8  
collation-server=utf8_general_ci  
