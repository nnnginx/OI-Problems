## Description

<div><p>Turtle was playing with a sequence $a_1, a_2, \ldots, a_n$ consisting of positive integers. Unfortunately, some of the integers went missing while playing.</p><p>Now the sequence becomes incomplete. There may exist an arbitrary number of indices $i$ such that $a_i$ becomes $-1$. Let the new sequence be $a'$.</p><p>Turtle is sad. But Turtle remembers that for every integer $i$ from $1$ to $n - 1$, either $a_i = \left\lfloor\frac{a_{i + 1}}{2}\right\rfloor$ or $a_{i + 1} = \left\lfloor\frac{a_i}{2}\right\rfloor$ holds for the original sequence $a$.</p><p>Turtle wants you to help him complete the sequence. But sometimes Turtle makes mistakes, so you need to tell him if you can't complete the sequence.</p><p>Formally, you need to find another sequence $b_1, b_2, \ldots, b_n$ consisting of positive integers such that:</p><ul> <li> For every integer $i$ from $1$ to $n$, if $a'_i \ne -1$, then $b_i = a'_i$. </li><li> For every integer $i$ from $1$ to $n - 1$, either $b_i = \left\lfloor\frac{b_{i + 1}}{2}\right\rfloor$ or $b_{i + 1} = \left\lfloor\frac{b_i}{2}\right\rfloor$ holds. </li><li> For every integer $i$ from $1$ to $n$, $1 \le b_i \le 10^9$. </li></ul><p>If there is no sequence $b_1, b_2, \ldots, b_n$ that satisfies all of the conditions above, you need to report $-1$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$) ！ the length of the sequence.</p><p>The second line of each test case contains $n$ integers $a'_1, a'_2, \ldots, a'_n$ ($a'_i = -1$ or $1 \le a'_i \le 10^8$) ！ the elements of the sequence $a'$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, if there is no sequence $b_1, b_2, \ldots, b_n$ that satisfies all of the conditions, output a single integer $-1$.</p><p>Otherwise, output $n$ integers $b_1, b_2, \ldots, b_n$ ！ the elements of the sequence $b_1, b_2, \ldots, b_n$ you find. The sequence should satisfy that $1 \le b_i \le 10^9$ for every integer $i$ from $1$ to $n$. If there are multiple answers, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$) ！ the length of the sequence.</p><p>The second line of each test case contains $n$ integers $a'_1, a'_2, \ldots, a'_n$ ($a'_i = -1$ or $1 \le a'_i \le 10^8$) ！ the elements of the sequence $a'$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, if there is no sequence $b_1, b_2, \ldots, b_n$ that satisfies all of the conditions, output a single integer $-1$.</p><p>Otherwise, output $n$ integers $b_1, b_2, \ldots, b_n$ ！ the elements of the sequence $b_1, b_2, \ldots, b_n$ you find. The sequence should satisfy that $1 \le b_i \le 10^9$ for every integer $i$ from $1$ to $n$. If there are multiple answers, print any of them.</p>





```input1|2,3,6,7,10,11,14,15,18,19
9
8
-1 -1 -1 2 -1 -1 1 -1
4
-1 -1 -1 -1
6
3 -1 -1 -1 9 -1
4
-1 5 -1 6
4
2 -1 -1 3
4
1 2 3 4
2
4 2
5
-1 3 -1 3 6
13
-1 -1 3 -1 -1 -1 -1 7 -1 -1 3 -1 -1
```




```output1
4 9 4 2 4 2 1 2
7 3 6 13
3 1 2 4 9 18
-1
-1
-1
4 2
6 3 1 3 6
3 1 3 1 3 7 3 7 3 1 3 1 3
```



## Note

<p>In the first test case, $[4, 2, 1, 2, 1, 2, 1, 3]$ can also be the answer, while $[4, 2, 5, 10, 5, 2, 1, 3]$ and $[4, 2, 1, 2, 1, 2, 1, 4]$ cannot.</p><p>In the second test case, $[1, 2, 5, 2]$ can also be the answer.</p><p>From the fourth to the sixth test cases, it can be shown that there is no answer, so you should output $-1$.</p>
