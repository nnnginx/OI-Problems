## Description

<div><p>Masha works in an advertising agency. In order to promote the new brand, she wants to conclude contracts with some bloggers. In total, Masha has connections of $n$ different bloggers. Blogger numbered $i$ has $a_i$ followers.</p><p>Since Masha has a limited budget, she can only sign a contract with $k$ different bloggers. Of course, Masha wants her ad to be seen by as many people as possible. Therefore, she must hire bloggers with the maximum total number of followers.</p><p>Help her, find the number of ways to select $k$ bloggers so that the total number of their followers is maximum possible. Two ways are considered different if there is at least one blogger in the first way, which is not in the second way. Masha believes that all bloggers have different followers (that is, there is no follower who would follow two different bloggers).</p><p>For example, if $n=4$, $k=3$, $a=[1, 3, 1, 2]$, then Masha has two ways to select $3$ bloggers with the maximum total number of followers: </p><ul> <li> conclude contracts with bloggers with numbers $1$, $2$ and $4$. In this case, the number of followers will be equal to $a_1 + a_2 + a_4 = 6$. </li><li> conclude contracts with bloggers with numbers $2$, $3$ and $4$. In this case, the number of followers will be equal to $a_2 + a_3 + a_4 = 6$. </li></ul><p>Since the answer can be quite large, <span class="tex-font-style-bf">output it modulo $10^9+7$</span>.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 1000$)&nbsp;！ the number of bloggers and how many of them you can sign a contract with.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots a_n$ ($1 \le a_i \le n$)&nbsp;！ the number of followers of each blogger.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$.</p></div><div class="output-specification"><p>For each test case, on a separate line output one integer&nbsp;！ the number of ways to select $k$ bloggers so that the total number of their followers is maximum possible.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 1000$)&nbsp;！ the number of bloggers and how many of them you can sign a contract with.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots a_n$ ($1 \le a_i \le n$)&nbsp;！ the number of followers of each blogger.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$.</p>

## Output

<p>For each test case, on a separate line output one integer&nbsp;！ the number of ways to select $k$ bloggers so that the total number of their followers is maximum possible.</p>

## Samples

```input1
3
4 3
1 3 1 2
4 2
1 1 1 1
2 1
1 2
```

```output1
2
6
1
```




## Note

<p>The test case is explained in the statements.</p><p>In the second test case, the following ways are valid: </p><ul> <li> conclude contracts with bloggers with numbers $1$ and $2$. In this case, the number of followers will be equal to $a_1 + a_2 = 2$; </li><li> conclude contracts with bloggers with numbers $1$ and $3$. In this case, the number of followers will be equal to $a_1 + a_3 = 2$; </li><li> conclude contracts with bloggers with numbers $1$ and $4$. In this case, the number of followers will be equal to $a_1 + a_4 = 2$; </li><li> conclude contracts with bloggers with numbers $2$ and $3$. In this case, the number of followers will be equal to $a_2 + a_3 = 2$; </li><li> conclude contracts with bloggers with numbers $2$ and $4$. In this case, the number of followers will be equal to $a_2 + a_4 = 2$; </li><li> conclude contracts with bloggers with numbers $3$ and $4$. In this case, the number of followers will be equal to $a_3 + a_4 = 2$. </li></ul><p>In the third test case, the following ways are valid: </p><ul> <li> concludes a contract with a blogger with the number $2$. In this case, the number of followers will be equal to $a_2 = 2$. </li></ul>
