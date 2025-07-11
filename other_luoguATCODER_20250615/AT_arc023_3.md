# AT_arc023_3 [ARC023C] タコヤ木

## 题目描述

高桥君从神秘人X那里得到了章鱼烧，种在院子里，长出了章鱼烧的树。高桥君为它取名“章鱼烧树”，小心翼翼地养护着它。有一天，高桥君发现章鱼烧树上结出了章鱼烧的果实，于是他每天数章鱼烧果实的数量，决定每天将“至今为止章鱼烧果实的总数”记录下来。

记录开始$N$天后，高桥君不小心将章鱼烧掉到了记录表上，共$N$天的记录的一部分被弄脏而无法阅读了。高桥君试图恢复这个记录，决定先计算一下记录数据的总数。

## 输入格式

按照以下格式标准输入：


------------


$N$ 

 $A_1$   $A_2$ ... $A_N$
 

------------
第1行输入一个整数$N$(1 ≦ $N$ ≦ 2,000)，表示记录天数；

第2行输入$ N $ 个表示记录的整数：$A_1$   $A_2$ ... $A_N$，之间以空格隔开(其中任何一个数$A_i$均满足$1$ ≦ $A_i$ ≦ $10^5$或$A_i$ = $0$)：

表示当$A_i$ = $-1$时，第$i$天的记录被弄脏了，无法阅读；当$A_i$ $\not=$ $-1$时，当天数据可读，“第$i$天时章鱼烧果实的总数”为$A_i$。

然而，$A_1$与$A_N$均不为$-1$。

保证输入数据中可阅读数据的个数不小于$1$.

## 输出格式

在下一行输出所有可能数据的个数除以$1,000,000,007$（质数）的余数。

## 输入输出样例 #1

### 输入 #1

```
3
1 -1 3
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
6
2 -1 -1 9 -1 9
```

### 输出 #2

```
36
```

## 输入输出样例 #3

### 输入 #3

```
5
1 -1 -1 -1 1000000000
```

### 输出 #3

```
999999972
```

## 说明/提示

对于所有$N$ ≦ $100$且$A_i≦100$的测试点，答案完全正确的给予50分；

对于所有$A_i$ ≦ $2,000$的测试点，答案完全正确的给予80分。