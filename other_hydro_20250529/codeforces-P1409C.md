## Description

<div><p>We have a secret array. You don't know this array and you have to restore it. However, you know some facts about this array:</p><ul> <li> The array consists of $n$ <span class="tex-font-style-bf">distinct positive</span> (greater than $0$) integers. </li><li> The array contains two elements $x$ and $y$ (these elements are <span class="tex-font-style-bf">known</span> for you) such that $x &lt; y$. </li><li> If you sort the array in increasing order (such that $a_1 &lt; a_2 &lt; \ldots &lt; a_n$), differences between all adjacent (consecutive) elements are equal (i.e. $a_2 - a_1 = a_3 - a_2 = \ldots = a_n - a_{n-1})$. </li></ul><p>It can be proven that such an array always exists under the constraints given below.</p><p>Among all possible arrays that satisfy the given conditions, we ask you to restore one which has the <span class="tex-font-style-bf">minimum possible</span> maximum element. In other words, you have to minimize $\max(a_1, a_2, \dots, a_n)$.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) �� the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains three integers $n$, $x$ and $y$ ($2 \le n \le 50$; $1 \le x &lt; y \le 50$) �� the length of the array and two elements that are present in the array, respectively.</p></div><div class="output-specification"><p>For each test case, print the answer: $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the $i$-th element of the required array. If there are several answers, you can print any (it also means that the order of elements doesn't matter).</p><p>It can be proven that such an array always exists under the given constraints.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) �� the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains three integers $n$, $x$ and $y$ ($2 \le n \le 50$; $1 \le x &lt; y \le 50$) �� the length of the array and two elements that are present in the array, respectively.</p>

## Output

<p>For each test case, print the answer: $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the $i$-th element of the required array. If there are several answers, you can print any (it also means that the order of elements doesn't matter).</p><p>It can be proven that such an array always exists under the given constraints.</p>

## Samples

```input1
5
2 1 49
5 20 50
6 20 50
5 3 8
9 13 22
```

```output1
1 49 
20 40 30 50 10
26 32 20 38 44 50 
8 23 18 13 3 
1 10 13 4 19 22 25 16 7
```



