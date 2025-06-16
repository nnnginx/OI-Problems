## 题目描述
Farmer John's $N$ cows are standing in a row, as they have a tendency to do from time to time.  Each cow is labeled with a distinct integer ID number so FJ can tell them apart. FJ would like to take a photo of a contiguous group of cows but, due to a traumatic  childhood incident involving the numbers $1 \ldots 6$, he only wants to take a picture of a group of cows if their IDs add up to a multiple of 7.

Please help FJ determine the size of the largest group he can photograph.

## 输入格式
The first line of input contains $N$ ($1 \leq N \leq 50,000$).  The next $N$ lines each contain the $N$ integer IDs of the cows (all are in the range $0 \ldots 1,000,000$).


## 输出格式
Please output the number of cows in the largest consecutive group whose IDs sum to a multiple of 7. If no such group exists, output 0.

## 题目大意
### 题目描述

Farmer John 的 $N$ 头奶牛站成一排，这是它们时不时会做的事情。每头奶牛都有一个独特的整数 ID 编号，以便 Farmer John 能够区分它们。Farmer John 希望为一组连续的奶牛拍照，但由于童年时与数字 $1 \ldots 6$ 相关的创伤事件，他只希望拍摄一组奶牛，如果它们的 ID 加起来是 7 的倍数。

请帮助 Farmer John 确定他可以拍摄的最大奶牛组的大小。

### 输入格式

输入的第一行包含 $N$（$1 \leq N \leq 50,000$）。接下来的 $N$ 行每行包含一头奶牛的整数 ID（所有 ID 都在 $0 \ldots 1,000,000$ 范围内）。

### 输出格式

请输出 ID 之和为 7 的倍数的最大连续奶牛组中的奶牛数量。如果不存在这样的组，则输出 0。

### 说明/提示

在这个例子中，$5+1+6+2+14 = 28$。

```input1
7
3
5
1
6
2
14
10
```

```output1
5
```

## 提示
In this example, $5+1+6+2+14 = 28$.

