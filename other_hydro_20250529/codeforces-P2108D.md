## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>You found the numbers $k$ and $n$ in the attic, but lost two arrays $A$ and $B$.</p><p>You remember that:</p><ul> <li> $|A| + |B| = n$, the total length of the arrays is $n$. </li><li> $|A| \geq k$ and $|B| \geq k$, the length of each array is at least $k$. </li><li> The arrays consist only of numbers from $1$ to $k$. </li><li> If you take any $k$ consecutive elements from array $A$, they will all be different. Also, if you take any $k$ consecutive elements from array $B$, they will all be different. </li></ul><p>Fortunately, a kind spirit that settled in the attic found these arrays and concatenated them into an array $C$ of length $n$. That is, the elements of array $A$ were first written into array $C$, followed by the elements of array $B$.</p><p>You can ask the kind spirit up to $250$ questions. Each question contains an index $i$ ($1 \leq i \leq n$). In response, you will receive the $i$-th element of the concatenated array $C$.</p><p>You need to find the lengths of arrays $A$ and $B$, or report that it is impossible to determine them uniquely.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 300$). The description of the test cases follows. </p><p>The only line of each test case contains two integers $n$ and $k$ ($1 \leq k \leq 50$, $2 k \leq n \leq 10^{6}$).</p><p>Note that the sum of $n$ across test cases is <span class="tex-font-style-bf">not limited</span>.</p></div><div><h2>Interaction</h2><p>The interaction for each test case begins with reading the integer $n$.</p><p>Then you can make up to $250$ queries.</p><p>To make a query, output a string in the format "<span class="tex-font-style-tt">? x</span>" (without quotes) ($1 \leq x \leq n$). After each query, read an integer&nbsp;¡ª the answer to your query.</p><p>If you make too many queries, you will receive a verdict of <span class="tex-font-style-tt">Wrong answer</span>.</p><p>To report your answer, output a string in the format "<span class="tex-font-style-tt">! a b</span>" (without quotes), where $a$ and $b$ are the lengths of arrays $A$ and $B$ that you found, respectively. The answer is not counted when counting the number of queries.</p><p>If it is impossible to determine the lengths of the arrays uniquely, output "<span class="tex-font-style-tt">! -1</span>" (without quotes). Note that if you answer $-1$ while there is a sequence of at most $250$ queries that uniquely determines the lengths of arrays, you will get a <span class="tex-font-style-tt">Wrong answer</span> verdict.</p><p>It is guaranteed that there are arrays $A$ and $B$ that do not contradict the statement, for which the interactor output is correct.</p><p>The interactor is <span class="tex-font-style-bf">not</span> adaptive, which means that the answer is known before the participant makes queries and does not depend on the queries made by the participant.</p><p>If your program makes more than $250$ queries, your program should immediately terminate to receive the verdict <span class="tex-font-style-tt">Wrong answer</span>. Otherwise, you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p>After outputting a query, do not forget to output a newline and flush the output buffer. Otherwise, you will receive a verdict of "<span class="tex-font-style-tt">IL</span>" (<span class="tex-font-style-tt">Idleness limit exceeded</span>). To flush the buffer, use: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see the documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>Hacks are disabled for this problem.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 300$). The description of the test cases follows. </p><p>The only line of each test case contains two integers $n$ and $k$ ($1 \leq k \leq 50$, $2 k \leq n \leq 10^{6}$).</p><p>Note that the sum of $n$ across test cases is <span class="tex-font-style-bf">not limited</span>.</p>





```input1
6
5 2

1

2

2

18 4

2

4

1

1

4

3 1

10 5

9 3

3

3

2

12 4

1

3

1

3

1

3
```




```output1
? 1

? 2

? 3

! 2 3

? 9

? 13

? 10

? 14

? 6

! 9 9

! -1

! 5 5

? 3

? 6

? 9

! 6 3

? 1

? 2

? 5

? 6

? 9

? 10

! -1
```



## Note

<p>Consider the first example. We queried the first $3$ elements out of $5$. Now we know that the array $C$ looks like $[1, 2, 2, ?, ?]$. We know for sure that the third element is not from array $A$&nbsp;¡ª because according to the condition, any $k$ consecutive elements (in our case $k = 2$) in array $A$ are different. Thus, the third element is definitely located in array $B$. This means that the length of array $A$ is $2$, and the length of array $B$ is $3$.</p><p>The picture shows arrays from all test cases. The elements whose values were requested are marked in yellow.</p><center> <img class="tex-graphics" src="./37118/file/XoZykqjc.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
