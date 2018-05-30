########################################################################################################################
优化可分解为三个层面：

    1.硬件配置
    
    2.配置文件
    
    3.语句及索引

########################################################################################################################

日志分析工具
    mysqldumpslow

慢查询工具
    pt-query-digest 

########################################################################################################################

3.语句及索引

1.查询次数多且每次查询时间长的sql
      pt-query-digest 分析的前面几个查询

2.IO大的sql
      pt-query-digest 分析中 Rows examine项

3.未命中的索引
      pt-query-digest 分析中 Rows examine vs Rows Send

B. explain查询和分析SQL
      运算函数查询
      子查询
      排序查询
      分页查询

C.如何选择建立索引
