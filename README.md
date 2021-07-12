# Configuration-file
公司练习题第一题

# 解析文件技术文档

### 一，变量规划

```
   Id string        // id
   Rarity string     //稀有度
   UnlockArena string //解锁阶段
   CombatPoints string //战力
   Name string //姓名
   Cvc string //稀有度
   vmap map[string]struct 

```

### 二，开发流程：



1，在main里面读取ini配置文件

2，监听配置端口号

3，打开json文件

4，对json文件进行反序列化

5，编写service层显示数据的方法

6，在Router层写路由接收方法

7，在controller层写数据调用方法

8，下载压力测试工具并进行压力测试

### 三，操作步骤：



步骤1：读取ini配置文件，获取端口号

步骤2：使用open方法打开文件，使用ioutil.ReadFile读取文件，然后反序列化

步骤3:编写service层GetSolider()等方法

步骤4:在controller层编写输出数据Getsolider()等方法

### 四，验证结果

通过localhost:8000/getrarity等url可以成功访问到数据。

