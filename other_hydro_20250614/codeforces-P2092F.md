## Description

<div><p>Let us define the <span class="tex-font-style-it">beauty</span> of a binary string $z$ as the number of indices $i$ such that $1 \le i &lt; |z|$ and $z_i \neq z_{i+1}$.</p><p>While waiting for his friends from the CCB, Andryusha baked a pie, represented by a binary string $s$ of length $n$. To avoid offending anyone, he wants to divide this string into $k$ substrings such that each digit belongs to exactly one substring, and the beauties of all substrings are the same.</p><p>Andryusha does not know the exact number of friends from the CCB who will come to his house, so he wants to find the number of values of $k$ for which it is possible to split the pie into exactly $k$ parts with equal beauties.</p><p>However, Andryusha's brother, Tristan, decided that this formulation of the problem is too simple. Therefore, he wants you to find the number of such values of $k$ <span class="tex-font-style-bf">for each prefix of the string</span>. In other words, for each $i$ from $1$ to $n$, you need to find the number of values of $k$ for which it is possible to split the prefix $s_1 s_2 \ldots s_i$ into exactly $k$ parts with equal beauties.</p></div><div class="input-specification"><p>Each test consists of several test cases. The first line of the input data contains one integer $t$ ($1 \le t \le 10^5$) ！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^6$) ！ the length of the binary string.</p><p>The second line of each test case contains a binary string of length $n$, consisting only of digits <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output a single line containing $n$ integers $c_i$ ($0 \le c_i \le n$) ！ the number of values of $k$ for which it is possible to split the prefix $s_1 s_2 \ldots s_i$ into exactly $k$ parts with equal beauties.</p></div>

## Input

<p>Each test consists of several test cases. The first line of the input data contains one integer $t$ ($1 \le t \le 10^5$) ！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^6$) ！ the length of the binary string.</p><p>The second line of each test case contains a binary string of length $n$, consisting only of digits <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output a single line containing $n$ integers $c_i$ ($0 \le c_i \le n$) ！ the number of values of $k$ for which it is possible to split the prefix $s_1 s_2 \ldots s_i$ into exactly $k$ parts with equal beauties.</p>





```input1|2,3,6,7
3
5
00011
10
0101010101
7
0010100
```




```output1
1 2 3 4 5
1 2 2 3 2 4 2 4 3 4
1 2 3 3 4 3 4
```



## Note

<p>In the third case, the values of $k$ that satisfy the conditions are: </p><ol> <li> $i = 1$: $k \in \{1\}$, </li><li> $i = 2$: $k \in \{1, 2\}$, </li><li> $i = 3$: $k \in \{1, 2, 3\}$, </li><li> $i = 4$: $k \in \{1, 3, 4\}$, </li><li> $i = 5$: $k \in \{1, 2, 4, 5\}$, </li><li> $i = 6$: $k \in \{1, 5, 6\}$, </li><li> $i = 7$: $k \in \{1, 5, 6, 7\}$. </li></ol>
