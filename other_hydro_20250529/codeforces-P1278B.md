## Description

<div><p>You are given two integers $a$ and $b$. You can perform a sequence of operations: during the first operation you choose one of these numbers and increase it by $1$; during the second operation you choose one of these numbers and increase it by $2$, and so on. You choose the number of these operations yourself.</p><p>For example, if $a = 1$ and $b = 3$, you can perform the following sequence of three operations: </p><ol> <li> add $1$ to $a$, then $a = 2$ and $b = 3$; </li><li> add $2$ to $b$, then $a = 2$ and $b = 5$; </li><li> add $3$ to $a$, then $a = 5$ and $b = 5$. </li></ol><p>Calculate the minimum number of operations required to make $a$ and $b$ equal. </p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$) �� the number of test cases.</p><p>The only line of each test case contains two integers $a$ and $b$ ($1 \le a, b \le 10^9$).</p></div><div class="output-specification"><p>For each test case print one integer �� the minimum numbers of operations required to make $a$ and $b$ equal. </p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$) �� the number of test cases.</p><p>The only line of each test case contains two integers $a$ and $b$ ($1 \le a, b \le 10^9$).</p>

## Output

<p>For each test case print one integer �� the minimum numbers of operations required to make $a$ and $b$ equal. </p>

## Samples

```input1
3
1 3
11 11
30 20
```

```output1
3
0
4
```




## Note

<p>First test case considered in the statement.</p><p>In the second test case integers $a$ and $b$ are already equal, so you don't need to perform any operations.</p><p>In the third test case you have to apply the first, the second, the third and the fourth operation to $b$ ($b$ turns into $20 + 1 + 2 + 3 + 4 = 30$).</p>
