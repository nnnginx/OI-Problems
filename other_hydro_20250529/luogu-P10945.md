## 题目描述
Robert is a famous engineer. One day he was given a task by his boss. The background of the task was the following:

Given a map consisting of square blocks. There were three kinds of blocks: Wall, Grass, and Empty. His boss wanted to place as many robots as possible in the map. Each robot held a laser weapon which could shoot to four directions (north, east, south, west) simultaneously. A robot had to stay at the block where it was initially placed all the time and to keep firing all the time. The laser beams certainly could pass the grid of Grass, but could not pass the grid of Wall. A robot could only be placed in an Empty block. Surely the boss would not want to see one robot hurting another. In other words, two robots must not be placed in one line (horizontally or vertically) unless there is a Wall between them.

Now that you are such a smart programmer and one of Robert's best friends, He is asking you to help him solving this problem. That is, given the description of a map, compute the maximum number of robots that can be placed in the map.


## 输入格式
The first line contains an integer T (<= 11) which is the number of test cases.

For each test case, the first line contains two integers m and n (1<= m, n <=50) which are the row and column sizes of the map. Then m lines follow, each contains n characters of '#', '*', or 'o' which represent Wall, Grass, and Empty, respectively.


## 输出格式
For each test case, first output the case number in one line, in the format: "Case :id" where id is the test case number, counting from 1. In the second line just output the maximum number of robots that can be placed in that map.


## 题目大意
### 题目描述

罗伯特是一位著名的工程师。一天，他的老板给了他一个任务。任务的背景如下：给定一个方格地图。地图上有三种可以放置的方块：墙方块、草方块和空地。老板希望在地图上可以尽可能多地放置机器人。每个机器人都配备了激光武器，可以同时向四个方向（东南西北，可以理解为上下左右）发射激光。机器人必须待在同一位置（也就是一开始放置的位置）且只能放在空地上不断地发射激光。激光束可以穿过草方块，但不能穿过墙方块。显然，老板不希望看到一个机器人伤害另一个机器人。换句话说，两个机器人不能放置在同一行或同一列上，除非它们之间有一堵墙。作为罗伯特的好朋友和聪明的程序员，他请你帮忙解决这个问题。也就是请你根据给定地图的描述，计算在地图上可以放置的最大机器人数量。

### 输入格式

 第一行包含一个整数 T ,表示测试用例的数量。对于每个测试用例，第一行包含两个整数 m 和 n ，分别表示地图的行数和列数。接下来是 m 行，每行包含 n 个字符，分别是 ‘#’, ‘*’, 或 ‘o’，表示墙方块、草方块和空地。
 
### 输出格式
 
 对于每个测试用例，首先输出一行，格式为：```Case :id```，其中 id 是测试用例编号，从 1 开始计数。1第二行输出在该地图上可以放置的最大机器人数量。
 
### 说明/提示

#### 数据范围
 
$T \leq 11$，$1 \leq m , n \leq 50$

```input1
2
4 4
o*** 
*### 
oo#o 
***o 
4 4 
#ooo 
o#oo 
oo#o 
***#
```

```output1
Case :1 
3
Case :2 
5
```

