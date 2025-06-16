# AT_code_festival_2018_qualb_c Special Cake for CODE FESTIVAL

## 题目描述

AtCoder 的社长 chokudai 准备了一个长方形蛋糕，准备分发给 CODE FESTIVAL 2018 比赛的参赛者。

蛋糕竖向分 $N$ 块，横向分 $N$ 块，总共要分 $N^2$ 块。

chokudai 养的狗理查德参加了 CODE FESTIVAL 2018 预选赛，但只是勉强通过。

理查德决定在比赛中喷洒一些蛋糕，让所有蛋糕都无法食用。当一块蛋糕被喷涂时，这块蛋糕和所有相邻的蛋糕都会变成不可食用。

请你找出一种喷洒方法，使理查德能够实现他的目标。 另外，喷洒的数量必须在 $201800$ 以内，因为如果他喷洒的时间太长，chokudai就会找到他。

## 输入格式

输入一个 $N$。

## 输出格式

请从第 $1$ 行到第 $N$ 行分别输出长度为 $N$ 的字符串。输出的字符串就是蛋糕的俯视图(每个字符对应 $1$ 块)，在该蛋糕块上喷涂时X，否则则输出.。X的个数不应小于 $201800$ 个。

如果存在多种这样的喷漆方式，可以输出其中的任意一种。

翻译来自于 [banglee](https://www.luogu.com.cn/user/681292)。

## 输入输出样例 #1

### 输入 #1

```
3
```

### 输出 #1

```
X..
..X
X..
```

## 输入输出样例 #2

### 输入 #2

```
6
```

### 输出 #2

```
X.X..X
..X.X.
X..X..
.X...X
X..X..
.X..X.
```

## 输入输出样例 #3

### 输入 #3

```
21
```

### 输出 #3

```
XXXXXXXXXXXXXXXXXXXXX
XXXXXXXXXXXXXXXXXXXXX
X....X....X....X....X
X.XXXX.XX.XX.X.X.XXXX
X.XXXX.XX.XX.X.X....X
X.XXXX.XX.XX.X.X.XXXX
X....X....X....X....X
XXXXXXXXXXXXXXXXXXXXX
X....X....XX...X....X
X.XXXX.XXXX.XXXXXX.XX
X....X....XX..XXXX.XX
X.XXXX.XXXXXXX.XXX.XX
X.XXXX....X...XXXX.XX
XXXXXXXXXXXXXXXXXXXXX
XXX.XX.XX.X....X.XXXX
XXX.XX.XX.X.XX.X.XXXX
XXX.XX.XX.X....X.XXXX
XXX.XXX..XX.XX.X.XXXX
XXX.XXXX.XX.XX.X....X
XXXXXXXXXXXXXXXXXXXXX
XXXXXXXXXXXXXXXXXXXXX
```