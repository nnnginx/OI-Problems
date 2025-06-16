## 题目描述

原题面请把语言调整为 English 即可查看!

中文简化题面 :

给定 $n$ 个人　包含坐标$x,y$和速度 $v$，如果一个点被一个人占有是指这个人比其他任何人都能先到达这个点。

对于这 $n$ 个人中的第 $i$ 个人，如果他占有的面积为无穷大，就输出 $1$，否则输出 $0$。

translate by [](/user/34)

## 输入格式

There are multiple test cases, terminated by a line "0".
For each test case, the first line contains one integer  $n$ $(1 \le n \le 500)$.
In following n lines, each line contains three integers  $x_i,y_i,v_i$ $(0 \le |xi|,|yi|,vi \le 10^4)$.

## 输出格式

For each case, output "Case #k: s", where $k$ is the case number counting from $1$, and $s$ is a string consisting of n character. If the area in the charge of the $i^{th}$ student isn't infinite, the $i^{th}$ character is "0", else it's "1".

```input13
0 0 3
1 1 2
2 2 1
0
```

```output1
Case #1: 100
```

