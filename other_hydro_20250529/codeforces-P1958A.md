## Description

<div><p>In Berland, coins of worth $1$, $3$ and $5$ burles are commonly used (burles are local currency).</p><p>Eva has to pay <span class="tex-font-style-bf">exactly</span> $n$ burles in a shop. She has an infinite amount of coins of all three types. However, she doesn't like to pay using coins worth $1$ burle ！ she thinks they are the most convenient to use.</p><p>Help Eva to calculate the minimum number of coins worth $1$ burle she has to use, if she has to pay exactly $n$ burles. Note that she can spend any number of coins worth $3$ and/or $5$ burles.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$) ！ the number of test cases.</p><p>Each test case consists of one line, containing one integer $n$ ($1 \le n \le 100$).</p></div><div class="output-specification"><p>For each test case, print one integer ！ the minimum number of $1$-burle coins Eva has to use.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$) ！ the number of test cases.</p><p>Each test case consists of one line, containing one integer $n$ ($1 \le n \le 100$).</p>

## Output

<p>For each test case, print one integer ！ the minimum number of $1$-burle coins Eva has to use.</p>





```input1|2,4,6
5
7
8
42
2
11
```




```output1
1
0
0
2
0
```



## Note

<p>In the first test case, Eva should use $1$ coin worth $1$ burle, and $2$ coins worth $3$ burles.</p><p>In the second test case, Eva should use $1$ coin worth $3$ burles and $1$ coin worth $5$ burles.</p><p>In the third test case, Eva should use $14$ coins worth $3$ burles.</p><p>In the fourth test case, Eva should use $2$ coins worth $1$ burle.</p><p>In the fifth test case, Eva should use $2$ coins worth $3$ burles and $1$ coin worth $5$ burles.</p>
