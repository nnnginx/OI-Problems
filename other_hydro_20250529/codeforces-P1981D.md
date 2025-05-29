## Description

<div><p>Turtle just learned how to multiply two integers in his math class, and he was very excited.</p><p>Then Piggy gave him an integer $n$, and asked him to construct a sequence $a_1, a_2, \ldots, a_n$ consisting of integers which satisfied the following conditions:</p><ul> <li> For all $1 \le i \le n$, $1 \le a_i \le 3 \cdot 10^5$. </li><li> For all $1 \le i &lt; j \le n - 1$, $a_i \cdot a_{i + 1} \ne a_j \cdot a_{j + 1}$. </li></ul><p>Of all such sequences, Piggy asked Turtle to find the one with the <span class="tex-font-style-bf">minimum</span> number of <span class="tex-font-style-bf">distinct</span> elements.</p><p>Turtle definitely could not solve the problem, so please help him!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^6$) ！ the length of the sequence $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output $n$ integers $a_1, a_2, \ldots, a_n$ ！ the elements of the sequence $a$.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^6$) ！ the length of the sequence $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output $n$ integers $a_1, a_2, \ldots, a_n$ ！ the elements of the sequence $a$.</p><p>If there are multiple answers, print any of them.</p>





```input1|2,4
3
2
3
4
```




```output1
114514 114514
1 2 2
3 3 4 4
```



## Note

<p>In the third test case, $a = [3, 4, 2, 6]$ violates the second condition since $a_1 \cdot a_2 = a_3 \cdot a_4$. $a = [2, 3, 4, 4]$ satisfy the conditions but its number of distinct elements isn't minimum.</p>
