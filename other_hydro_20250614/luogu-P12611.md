## 题目背景
Score: 15.

## 题目描述
A store has hired the Code Cleaning Crew to help it update all of its product codes.

The original product codes are sequences of letters, positive integers, and negative integers. For example, $\tt{cG23mH-9s}$ is a product code that contains two uppercase letters, three lowercase letters, one positive integer, and one negative integer.

The new product codes are made by removing all lowercase letters, keeping all uppercase letters in order, and adding all the integers to form one new integer which is placed at the end of the code. For example, the new product code for $\tt{cG23mH-9s}$ is $\tt{GH14}$.

Your job is to take a list of original product codes and determine the new product codes.

## 输入格式
The first line of input contains a positive integer, $N$, representing the number of original product codes that need to be updated. The following $N$ lines each contain one original product code.

Each original product code contains at least one uppercase letter, at least one lowercase letter, and at least one integer. Also, a positive integer never immediately follows another integer. This means, for example, that $23$ is the integer $23$ instead of the integer $2$ followed by the integer $3$.



## 输出格式
Output the $N$ new product codes, one per line.

```input1
1
AbC3c2Cd9
```

```output1
ACC14
```

```input2
3
Ahkiy-6ebvXCV1
393hhhUHkbs5gh6QpS-9-8
PL12N-2G1234Duytrty8-86tyaYySsDdEe
```

```output2
AXCV-5
UHQS387
PLNGDYSDE1166
```

## 提示
**Explanation of Output for Sample Input 1**

For the single original product code, the uppercase letters $\tt A$, $\tt C$, and $\tt C$ are kept in order and the sum of the integers is $3 + 2 + 9 = 14$.

**Explanation of Output for Sample Input 2**

For the first original product code, the uppercase letters $\tt A$, $\tt X$, $\tt C$, and $\tt V$ are kept in order and the sum of the integers is $-6 + 1 = -5$.

For the second and third original product codes, their uppercase letters are also kept in order and the sums of the integers are $393 + 5 + 6 - 9 - 8 = 387$ and $12 - 2 + 1234 + 8 - 86 = 1166$ respectively.

The following table shows how the available $15$ marks are distributed:

|Marks|Description|
|:-:|:-:|
|2|All the integers are positive and single-digit|
|2|All the integers are single-digit.|
|7|Any positive integer may be multi-digit.|
|4|Any integer may be multi-digit.|

