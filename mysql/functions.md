# 数值型
GREATEST( ) 最大值   
LEAST( ) 最小值   
IN(1,2,3) 是否为 1 2 3  
# 字符型 
LENGTH( ) 字节长度   
CHAR_LENGTH() 字符长度  
CONCAT( [STR] , [STR] ) 字符串连接  
UPPER( ), LOWER() 大写/小写  
LEFT('hello', 2), RIGHT('hello', 3) 左/右的前几个字符  
LPAD(salary, 10, '0') 左位补0 补到10位 RPAD同理  
TRIM( [STR] ) 去空格   
LTRIM( [STR] ) 去左侧空格 RTRIM同理  
NULLIF(val1, val2) 比较两个字符串 如果val1和val2相等， 则返回NULL， 否则返回val1
# 日期与时间型
CURDATE( ) 当前日期  
CURTIME( ) 当前时间  
NOW( ) 当前日期时间  
UTC_TIME( ) UTC时间   
UTC_DATE( ) UTC日期  
UNIX_TIMESTAMP('2021-10-01 12:12:32') 时间转时间戳  
FROM_UNIXTIME(1633061552) 时间戳转时间  
# 流程控制型
IF(A,B,C) 三元运算符 如果A为真 那么结果为B 否则结果为C  
IFNULL(A,B) 如果A不为NULL 则结果为A 不然结果为B  
CASE WHEN THEN ELSE END 举例子：  
select salary, case when salary > 10000 then 'rich'  
                    when salary > 5000 then 'ok'  
                    else 'poor' end  
from employees;
# 其他
ISNULL( ) 是否为NULL   
VERSION() 版本号
CONNECTON_ID() 连接id
DATABASE() 当前数据库