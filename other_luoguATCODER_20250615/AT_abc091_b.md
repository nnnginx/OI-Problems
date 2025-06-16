# AT_abc091_b [ABC091B] Two Colors Card Game

## 题目描述

有两组字符串，一组蓝色，一组红色，各有n、m个字符串。你可以随便说一个字符串：

如果你在蓝色的字符串组中找到了这个字符串，就加一分；如果在红色的字符串组中找到了，就扣一分。

现在让你输出得分的最大值，且只有得分非负时才输出。

## 输入格式

输入n，接下来n行输入字符串(s[i])。输入m，接下来m行输入字符串(t[i])

## 输出格式

输出得分的最大值。

## 输入输出样例 #1

### 输入 #1

```
3
apple
orange
apple
1
grape
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
3
apple
orange
apple
5
apple
apple
apple
apple
apple
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
1
voldemort
10
voldemort
voldemort
voldemort
voldemort
voldemort
voldemort
voldemort
voldemort
voldemort
voldemort
```

### 输出 #3

```
0
```

## 输入输出样例 #4

### 输入 #4

```
6
red
red
blue
yellow
yellow
red
5
red
red
yellow
green
blue
```

### 输出 #4

```
1
```