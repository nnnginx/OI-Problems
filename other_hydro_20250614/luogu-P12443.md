## 题目描述
There are $n$ food items lying in a row on a long table. Each of these items is either a loaf of bread (denoted as a capital Latin letter $\texttt{L}$ with ASCII code 76) or an onion (denoted as a capital Latin letter $\texttt{O}$ with ASCII code 79). There is at least one loaf of bread and at least one onion on the table.

You and your friend want to divide the food on the table: you will take a prefix of this row (several leftmost items), and the friend will take the rest. However, there are several restrictions:

- Each person should have at least one item.
- The number of your loaves should differ from the number of your friend's loaves.
- The number of your onions should differ from the number of your friend's onions.

Find any correct division and print the number of items you take or report that there is no answer.

## 输入格式
The first line contains one integer $n$ ($2 \le n \le 200$) --- the number of food items on the table. The second line contains a string of length $n$ consisting of letters $\texttt{L}$ and $\texttt{O}$. $i$-th symbol represents the type of the $i$-th food item on the table: $\texttt{L}$ stands for a loaf of bread, and $\texttt{O}$ stands for an onion. It is guaranteed that this string contains at least one letter $\texttt{L}$ and at least one letter $\texttt{O}$.

## 输出格式
Print one integer --- a number $k$ such that, if you take $k$ leftmost items and your friend takes the remaining $n - k$ items, each of you and your friend get at least one item, your number of loaves is different from your friend's, and your number of onions is different from your friend's. If there are several possible answers, print any of them. If there are no possible answers, print the number $-1$.

```input1
3
LOL
```

```output1
-1
```

```input2
2
LO
```

```output2
1
```

```input3
4
LLLO
```

```output3
1
```

```input4
4
OLOL
```

```output4
-1
```

```input5
10
LLOOOOLLLO
```

```output5
5
```

## 提示
In the first example, in any division the left and the right part contain one loaf of bread.

In the second example, the division is $\texttt{L}$ and $\texttt{O}$, and in these two strings the number of loaves is different (1 and 0) and the number of onions is different (0 and 1).

In the third example, any number 1, 2 or 3 is a correct answer.


