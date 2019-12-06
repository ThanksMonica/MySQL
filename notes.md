# MySQL notes
* 创建表<br>
* 查询数据库<br>
* 选择数据库<br>
  USE 库名；
***********
* ## 查询<br>
SELECT 查询列表 FROM 表名；<br>
1. 单个字段<br>
   SELECT 字段 FROM 表名；<br>
2. 多个字段<br>
   SELECT 字段1，2，3 FROM 表名；<br>
3. 所有字段<br>
   SELECT * FROM 表名；<br>
4. 常量/值/表达式/函数
   ***
5. 取别名<br>
   SELECT 查询列表 AS "别名"<br>
    SELECT 查询列表 别名<br>
6. 去重<br>
   SELECT DISTINCT 查询列表 FROM 表名<br>
7. 拼接
   SELECT CONCAT(a,b,c) AS 别名
   ***
8. 条件查询
   SELECT 查询列表 FROM 表名 WHERE 筛选条件；<br> 
   1. 筛选条件：<br> 
   简单条件运算符 > < = >= <= <> !=<br> 
   逻辑表达式 && || !<br> 
   模糊表达式 like（一般与通配符搭配使用）、between and、in（用于判断某字段的值是否属于in列表中的某一项；in列表类型必须一致；不支持通配符）、is null
   2. 