## 题目描述
Mirko has found a matrix with N rows and M columns at the back seat of his car. The first
row of the matrix consists of numbers 1, 2, … M, the second row of numbers M+1, M+2, …
2⋅M and so on until the $N^{th}$  
row which consists of numbers (N-1)⋅M + 1, (N-1)⋅M + 2, …
N⋅M, respectively.

For example, for N = 3 and M = 4:

| - | - | - | - |
| :----------: | :----------: | :----------: | :----------: |
| **1** | **2** | **3** | **4** |
| **5** | **6** | **7** | **8** |
| **9** | **10** | **11** | **12** |

Such matrix wasn’t interesting enough to him, so he chose a row or a column K times and
multiplied its values with a non-negative integer.

Naturally, now he wants to know the sum of all the values from the matrix. Since this sum
can be very large, Mirko will be satisfied with the value modulo $10^9$ + 7. Help Mirko answer
this question.

## 输入格式
The first line of input contains the numbers N (1 ≤ N ≤ 1 000 000), M (1 ≤ M ≤ 1 000
000) and K (1 ≤ K ≤ 1000) from the task.

 - Either the multiplication of the $X^{th}$
row with Y, in the form of "R X Y", where “R”
represents row multiplication, X is a positive integer (1 ≤ X ≤ N), and Y is a
non-negative integer (0 ≤ Y ≤ $10^{9}$
).

 - Or the multiplication of the $X^{th}$ column with Y, in the form of “S X Y”, where “S”
represents column multiplication, X is a positive integer (1 ≤ X ≤ M), and Y is a
non-negative integer (0 ≤ Y ≤ $10^{9}$
).

## 输出格式
You must output the sum of the final values from the matrix modulo $10^{9}$ + 7

```input1
3 4 4
R 2 4
S 4 1
R 3 2
R 2 0
```

```output1
94
```

```input2
3 1 1
S 1 4

```

```output2
24
```

```input3
2 4 4
S 2 0
S 2 3
R 1 5
S 1 3
```

```output3
80
```

## 提示
In test cases worth a total of 50 points, it will hold 1 ≤ N, M ≤ 1000.

**Clarification of the first test case:**
After multiplying the second row with 4, the fourth column with 1, the third row with 2, and again the
second row with 0, the final matrix looks like this:

| - | - | - | - |
| :----------: | :----------: | :----------: | :----------: |
| **1** | **2** | **3** | **4** |
| **0** | **0** | **0** | **0** |
| **18** | **20** | **22** | **24** |

The sum of the elements from the final matrix is 1 + 2 + 3 + 4 + 0 + 0 + 0 + 0 + 18 + 20 + 22 + 24 =
94.

