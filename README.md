# Xorm-demo
Assignment for service computing : Xorm-demo

## 使用 xorm 实现老师博客中的程序
老师博客地址：<code>http://blog.csdn.net/pmlpml/article/details/78602290</code>

直接在老师的代码上进行修改，使用要求的xorm将老师代码中的一部分作替换。

在原有的代码上进行了一些细节修改。

## orm 是否就是实现了dao的自动化？
对于数据库操作，orm不再需要自己写SQL代码，而是自动生成SQL代码，是实现了dao的自动化。

## 使用 ab 测试性能
```shell
This is ApacheBench, Version 2.3 <$Revision: 1757674 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking localhost (be patient).....done


Server Software:        
Server Hostname:        localhost
Server Port:            8080

Document Path:          /hello/pineapple-chicken
Document Length:        169 bytes

Concurrency Level:      10
Time taken for tests:   1.897 seconds
Complete requests:      100
Failed requests:        0
Total transferred:      18400 bytes
HTML transferred:       3100 bytes
Requests per second:    1623.54 [#/sec] (mean)
Time per request:       7.132 [ms] (mean)
Time per request:       0.702 [ms] (mean, across all concurrent requests)
Transfer rate:          230.21 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    2   3.7      1      21
Processing:     0    4   3.8      2      20
Waiting:        0    3   4.6      2      18
Total:          0    6   6.7      4      19

Percentage of the requests served within a certain time (ms)
  50%      4
  66%      8
  75%      8
  80%      9
  90%     20
  95%     20
  98%     20
  99%     20
 100%     20 (longest request)
```
