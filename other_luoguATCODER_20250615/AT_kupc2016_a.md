# AT_kupc2016_a バリケード

## 题目描述

暑假结束了，新学期如约而至。你是京都大学的一个学生，但在开学前你听说了一则爆炸性新闻：**教室会被某人封锁（摆上路障）**。 

该路障将在A时期开始之时建立，并将在B时期之前那千钧一发的时候被童鞋们销毁。（**这个地方太危险了吧**）

在封锁时段内，教室将无法正常使用，因为童鞋们将无法进入或离开教室。

如果你在大学中读书，今天要上N堂课，每堂课的开始时间都是t[i],问你能安安静静地上几节课？

## 输入格式

一共N+1行,

第一行输入N,A,B；

下面N行，每行输入一个t[i];
```
N N N   A A A   B B B 
t1 t1 t1 
:
tN tN tN 
```

## 输出格式

你能上的课的总节数（**记得换行**）

**输入输出样例**

见题面

## 输入输出样例 #1

### 输入 #1

```
5 5 9
4
3
6
9
1
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
5 4 9
5
6
7
8
9
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
4 3 6
9
6
8
1
```

### 输出 #3

```
4
```

## 输入输出样例 #4

### 输入 #4

```
2 1 2
1
2
```

### 输出 #4

```
1
```