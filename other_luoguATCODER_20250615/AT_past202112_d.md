# AT_past202112_d 試験

## 题目描述

有 $N$ 名 学生在 AtCoder 高中上学，他们有学生 ID ，叫学生 $1$ ，学生 $2$ ， $...$ ，学生 $N$ 。 一天，他们都参加了数学和英语的考试，学生 $i$ $(1\leq i\leq n)$ 的数学成绩是 $A_i$ ，英语成绩是 $B_i$ 。在这所学校，学生的排名规则如下：

- 学生数学和英语的总分更高排名更高。

- 两个学生总分相同时，数学成绩成绩更高排名更高。

- 当两个学生总分和数学成绩都相同时，学生 ID 较小的学生排名更高。

按排名降序输出 $N$ 名学生的 ID。

## 输入格式

输入共 $3$ 行。

第一行一个整数 $N$ ，代表有 $N$ 名学生。

第二行共 $N$ 个整数，第 $i$ 个数为 $A_i$，代表第 $i$ 名学生的数学成绩，用空格隔开。

第三行共 $N$ 个整数，第 $i$ 个数为 $B_i$，代表第 $i$ 名学生的英语成绩，用空格隔开。

## 输出格式

按排名降序输出 $N$ 名学生的 ID，用空格隔开

## 输入输出样例 #1

### 输入 #1

```
5
5 10 10 12 5
10 10 5 0 10
```

### 输出 #1

```
2 3 1 5 4
```

## 输入输出样例 #2

### 输入 #2

```
2
0 1000000000
0 1000000000
```

### 输出 #2

```
2 1
```

## 说明/提示

$2\leq N\leq 2\times 10^5$

$0\leq A_i\leq 10^9$

$0\leq B_i\leq 10^9$

translated by @[wangyinghao](https://www.luogu.com.cn/user/453759)