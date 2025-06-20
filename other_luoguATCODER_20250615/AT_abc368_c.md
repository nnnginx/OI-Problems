# AT_abc368_c [ABC368C] Triple Attack

## 题目描述

你正在玩一款游戏。

游戏中有 $N$ 个敌人排成一排，第 $i$ 个敌人有 $h_i$ 的血量,当敌人血量降至 0 或以下时该敌人被消灭。  

从第 1 只敌人开始打，时间 $T$ 从 0 开始，重复执行如下操作:

- $T$ 增加 1，若此时 $T$ 为 3 的倍数，当前敌人掉 3 滴血，否则掉 1 滴血。

 求消灭全部敌人所需时间 $T$。

---

## 输入格式

- 第一行输入一个正整数 $N$。
- 第二行输入 $N$个 正整数 $H_1,H_2,\dots,H_n$。

---

## 输出格式

- 输出一行答案 $T$

--- 

## 样例 #1

### 样例输入 #1

```
3
6 2 2
```

### 样例输出 #1

```
8
```

## 输入输出样例 #1

### 输入 #1

```
3
6 2 2
```

### 输出 #1

```
8
```

## 输入输出样例 #2

### 输入 #2

```
9
1 12 123 1234 12345 123456 1234567 12345678 123456789
```

### 输出 #2

```
82304529
```

## 输入输出样例 #3

### 输入 #3

```
5
1000000000 1000000000 1000000000 1000000000 1000000000
```

### 输出 #3

```
3000000000
```

## 说明/提示

采取的行动如下:

- $T=1$，攻击第 $1$ 个敌人，第一个敌人的血量为 $6-1=5$；
- $T=2$，攻击第 $1$ 个敌人，第一个敌人的血量为 $5-1=4$；
- $T=3$，攻击第 $1$ 个敌人，第一个敌人的血量为 $4-3=1$；
- $T=4$，攻击第 $1$ 个敌人，第一个敌人的血量为 $1-1=0$；
- $T=5$，攻击第 $2$ 个敌人，第二个敌人的血量为 $2-1=1$；
- $T=6$，攻击第 $2$ 个敌人，第二个敌人的血量为 $1-3=-2$；
- $T=7$，攻击第 $3$ 个敌人，第三个敌人的血量为 $2-1=1$；
- $T=8$，攻击第 $3$ 个敌人，第三个敌人的血量为 $1-1=0$；


## 样例 #2

### 样例输入 #2

```
9
1 12 123 1234 12345 123456 1234567 12345678 123456789
```

### 样例输出 #2

```
82304529
```

## 样例 #3

### 样例输入 #3

```
5
1000000000 1000000000 1000000000 1000000000 1000000000
```

### 样例输出 #3

```
3000000000
```


注意数据溢出。


---

- $ 1 \leq\ N \leq\ 2\times 10^5 $
- $ 1 \leq\ H_i \leq 10^9 $
- 所有输入均为整数