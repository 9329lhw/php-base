<h1 align="center">《redis》</h1>

<p align="center">
<a href="https://github.com/TIGERB/easy-tips/tree/master/redis">
  <img src="https://img.shields.io/badge/redis-doing-blue.svg" alt="redis">
</a>
</p>

<p align="center"><a href="README-EN.md" >English Version</a></p>

<br>

> redis技术整理

## 备注

状态        | 含义
--------- | -------
not-start | 当前未开始总结
doing     | 总结中
α         | 目前仅供参考未修正和发布
done      | 总结完毕
fixing    | 查漏补缺修改中
r*    | 重点识记

## 目录

- redis常见数据类型(done)

  - 符合PSR的PHP编程规范(含个人建议)

    - [实例](https://github.com/TIGERB/easy-tips/blob/master/php/standard.php)
    - [文档](https://github.com/TIGERB/easy-tips/blob/master/php/standard.md)
    - [经验](https://github.com/TIGERB/easy-tips/blob/master/php/artisan.md)

  - 基础知识[读(R)好(T)文(F)档(M)]
    - [数据类型](http://php.net/manual/zh/language.types.php)

    - [运算符优先级](http://php.net/manual/zh/language.operators.precedence.php)
    - [string函数](http://php.net/ref.strings.php)
    - [array函数](http://php.net/manual/zh/ref.array.php)
    - [math函数](http://php.net/manual/zh/ref.math.php)
    - [面向对象](http://php.net/manual/zh/language.oop5.php)
    - 版本新特性

      - [7.1](http://php.net/manual/zh/migration71.new-features.php)
      - [7.0](http://php.net/manual/zh/migration70.new-features.php)
      - [5.6](http://php.net/manual/zh/migration56.new-features.php)
      - [5.5](http://php.net/manual/zh/migration55.new-features.php)
      - [5.4](http://php.net/manual/zh/migration54.new-features.php)
      - [5.3](http://php.net/manual/zh/migration53.new-features.php)

  - [记一些坑](https://github.com/TIGERB/easy-tips/blob/master/pit.md#记一些坑)

- PHP深入学习(doing)
  - 理解yield
  - php的协程
  - 生命周期
  - 垃圾回收
  - 扩展开发

- 网络编程(doing)
    - php实现web服务器
    - go实现web服务器
    - c实现web服务器
    - php扩展实现web服务器

- 问题排查(doing)
  - nginx/php/业务日志
  - 问题排查实例分析
  
- Mysql(doing)

  - [常用sql语句](https://github.com/TIGERB/easy-tips/blob/master/mysql/sql.md)
  - [引擎](https://github.com/TIGERB/easy-tips/blob/master/mysql/base.md#引擎)
    - InnoDB
    - MyISAM
    - Memory
    - Archive
    - Blackhole\CSV\Federated\merge\NDB
  - [事务](https://github.com/TIGERB/easy-tips/blob/master/mysql/base.md#事务)
    + 原子性（Atomicity）
    + 一致性（Consistency）
    + [隔离性（Isolation）](https://github.com/TIGERB/easy-tips/blob/master/mysql/base.md#mysql数据库为我们提供的四种隔离级别)
      * READ UNCOMMITTED:未提交读
      * READ COMMITTED：提交读/不可重复读
      * REPEATABLE READ：可重复读(MYSQL默认事务隔离级别)
      * SERIALIZEABLE：可串行化
    + 持久性（Durability）
  - [索引](https://github.com/TIGERB/easy-tips/blob/master/mysql/base.md#索引)
    + 建立表结构时添加的索引
      * 主键唯一索引
      * 唯一索引
      * 普通索引
      * 联合索引
        - 最左匹配原则
    + 依据是否聚簇区分
      * 聚簇索引
      * 非聚簇索引
    + 索引底层数据结构
      * hash索引
      * b-tree索引
      * b+tree索引
    
  - [锁](https://github.com/TIGERB/easy-tips/blob/master/mysql/base.md#锁)
    - 悲观锁
    - 乐观锁
  - 分表
    - 垂直分表
    - 水平分表
  - sql优化
  - 主从配置

- Redis(doing)

  - 常用命令
  - 实现原理&与memcache区别
  - 常见使用场景实现
    - [缓存](https://github.com/TIGERB/easy-tips/blob/master/redis/cache.php)
    - [队列](https://github.com/TIGERB/easy-tips/blob/master/redis/queue.php)
    - [悲观锁](https://github.com/TIGERB/easy-tips/blob/master/redis/pessmistic-lock.php)
    - [乐观锁](https://github.com/TIGERB/easy-tips/blob/master/redis/optimistic-lock.php)
    - [订阅/推送](https://github.com/TIGERB/easy-tips/blob/master/redis/subscribe-publish)
  - 常见业务实际使用
  - redis的基础数据结构

- 设计模式(done/fixing)

- [数据结构(doing)](https://github.com/TIGERB/easy-tips/blob/master/data-structure.md)

  - 数组
  - 堆/栈
  - 树
  - 队列
  - 链表
  - 图
  - 散列表

- 算法(doing)

  - 算法分析

    - 时间复杂度/空间复杂度/正确性/可读性/健壮性

  - 算法实战

    - 排序算法(α)

      - [冒泡排序](https://github.com/TIGERB/easy-tips/blob/master/algorithm/sort/bubble.php)
      - [快速排序](https://github.com/TIGERB/easy-tips/blob/master/algorithm/sort/quick.php)
      - [选择排序](https://github.com/TIGERB/easy-tips/blob/master/algorithm/sort/select.php)
      - [插入排序](https://github.com/TIGERB/easy-tips/blob/master/algorithm/sort/insert.php)
      - [归并排序](https://github.com/TIGERB/easy-tips/blob/master/algorithm/sort/merge.php)
      - [希尔排序](https://github.com/TIGERB/easy-tips/blob/master/algorithm/sort/shell.php)
      - [基数排序](https://github.com/TIGERB/easy-tips/blob/master/algorithm/sort/radix.php)

- 网络基础(doing)
  - [网络状态码](https://github.com/TIGERB/easy-tips/blob/master/network/internet-protocol.md#互联网协议)
  - [iso七层协议](https://github.com/TIGERB/easy-tips/blob/master/network/internet-protocol.md#互联网协议)
  - [tcp/ip四层协议](https://github.com/TIGERB/easy-tips/blob/master/network/internet-protocol.md#互联网协议)
  - [三次握手/四次挥手](https://github.com/TIGERB/easy-tips/blob/master/network/internet-protocol.md#互联网协议)
  - [互联网协议概述](https://github.com/TIGERB/easy-tips/blob/master/network/internet-protocol.md#互联网协议)
  - [http](https://github.com/TIGERB/easy-tips/blob/master/network/http.md)
    - https
    - http2
  - websocket
    
- 计算机基础(doing)

  - [linux常用命令](https://github.com/TIGERB/easy-tips/blob/master/linux/command.md)
  - shell

- 高并发相关(not-start)
- 面试相关