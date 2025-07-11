# AT_abc278_b [ABC278B] Misjudge the Time

## 题目描述

高桥买了个台钟。这个钟采用 24 小时计时法，显示的时间为 $\overline{AB}:\overline{CD}$。当且仅当 $0\leq \overline {AB}<24$ 且 $0\leq \overline {CD}<60$ 时我们称这个时间是合法的。

高桥决定将满足以下条件的时间叫做 “**迷惑时间**”：

+ 如果把 $B$ 和 $C$ 交换，这个时间仍然是合法的。

比如说 20:13 是“**迷惑时间**”，因为 21：03 是合法的。

现在高桥的钟显示的时间是 $H:M$。请你求出从现在之后离现在最近的“**迷惑时间**”（包括现在）。

## 输入格式

>$H\quad M$

## 输出格式

设答案是 $h:m$，那么请你输出：

>$h\quad m$

输出允许 $h$ 存在前导 $0$。

## 输入输出样例 #1

### 输入 #1

```
1 23
```

### 输出 #1

```
1 23
```

## 输入输出样例 #2

### 输入 #2

```
19 57
```

### 输出 #2

```
20 0
```

## 输入输出样例 #3

### 输入 #3

```
20 40
```

### 输出 #3

```
21 0
```

## 说明/提示

+ $0\leq H\leq 23$
+ $0\leq M\leq 59$
+ $H$ 和 $M$ 是整数
#### 样例解释
+ **样例 1**

1:23 是一个“**迷惑时间**”，因为 2:13 是合法的。因此答案就是 1:23。

当然，即使你输出 ```01 23``` 也是可以的。
+ **样例 2**

19:57 后的下一个“**迷惑时间**”是 20:00。
+ **样例 3**

请注意 24:00 是不合法的时间。