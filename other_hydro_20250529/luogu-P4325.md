## 题目描述
Given two integers A and B, A modulo B is the remainder when dividing A by B. For example, the numbers 7, 14, 27 and 38 become 1, 2, 0 and 2, modulo 3. Write a program that accepts 10 numbers as input and outputs the number of distinct numbers in the input, if the numbers are considered modulo 42.

## 输入格式
The input will contain 10 non-negative integers, each smaller than 1000, one per line.

## 输出格式
Output the number of distinct values when considered modulo 42 on a single line.

## 题目大意
给出 $10$ 个整数，问这些整数除以 $42$ 后得到的余数有多少种。

- 第一个样例的十个结果是 $1,2,3,4,5,6,7,8,9,10$，有 $10$ 个不同的结果；
- 第二个样例结果都是 $0$，只有一个不同的结果；
- 第三个样例余数是 $39,40,41,0,1,2,40,41,0,1$，有 $0,1,2,39,40,41$ 这六个不同的结果。

```input1
1
2
3
4
5
6
7
8
9
10
```

```output1
10
```

```input2
42
84
252
420
840
126
42
84
420
126
```

```output2
1
```

```input3
39
40
41
42
43
44
82
83
84
85
```

```output3
6
```

## 提示
In the first example, the numbers modulo 42 are 1, 2, 3, 4, 5, 6, 7, 8, 9 and 10.
In the second example all numbers modulo 42 are 0.
In the third example, the numbers modulo 42 are 39, 40, 41, 0, 1, 2, 40, 41, 0 and 1. There are 6 distinct numbers.

