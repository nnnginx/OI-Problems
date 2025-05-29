## Description

<div><p>Monsters are approaching the city, and to protect it, Akito must create a protective field around the city. As everyone knows, protective fields come in various levels. Akito has chosen the field of level $n$. To construct the field, a special phrase is required, which is the $n$-th row of the Great Magical Triangle, represented as a two-dimensional array. We will call this array $T$.</p><p>The triangle is defined as follows: </p><ul> <li> In the $i$-th row, there are $i$ integers. </li><li> The single integer in the first row is $k$. </li><li> Let the $j$-th element of the $i$-th row be denoted as $T_{i,j}$. Then $$T_{i,j} = \begin{cases} T_{i-1,j-1} \oplus T_{i-1,j}, &amp;\textrm{if } 1 &lt; j &lt; i \\ T_{i-1,j}, &amp;\textrm{if } j = 1 \\ T_{i-1,j-1}, &amp;\textrm{if } j = i \end{cases}$$ </li></ul> where $a \oplus b$ is the bitwise <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">exclusive "OR"</a>(<span class="tex-font-style-tt">XOR</span>) of the integers $a$ and $b$.<p>Help Akito find the integers in the $n$-th row of the infinite triangle before the monsters reach the city.</p></div><div class="input-specification"><p>The first line contains the integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>In the only line of each test case, there are two integers $n$ and $k$ ($1 \le n \le 10^6,\ 1 \le k &lt; 2^{31}$) ！ the row index that Akito needs and the integer in the first row of the Great Magical Triangle, respectively.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output $n$ integers ！ the elements of the $n$-th row of the Great Magical Triangle.</p></div>

## Input

<p>The first line contains the integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>In the only line of each test case, there are two integers $n$ and $k$ ($1 \le n \le 10^6,\ 1 \le k &lt; 2^{31}$) ！ the row index that Akito needs and the integer in the first row of the Great Magical Triangle, respectively.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output $n$ integers ！ the elements of the $n$-th row of the Great Magical Triangle.</p>





```input1|2,4,6
5
1 5
2 10
3 16
9 1
1 52
```




```output1
5
10 10
16 0 16
1 0 0 0 0 0 0 0 1
52
```



## Note

<p>In the first example, the first row of the Great Magical Triangle is $[5]$ by definition.</p><p>In the second example, $T_{2,1} = T_{1,1} = 10$ and $T_{2,2} = T_{1, 1} = 10$.</p>
