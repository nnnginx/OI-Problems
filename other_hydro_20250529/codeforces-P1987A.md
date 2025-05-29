## Description

<div><p><span class="tex-font-style-it">Oh no, the ForceCodes servers are running out of memory! Luckily, you can help them out by uploading some of your RAM!</span></p><p>You want to upload $n$ GBs of RAM. Every second, you will upload either $0$ or $1$ GB of RAM. However, there is a restriction on your network speed: in any $k$ consecutive seconds, you can upload only at most $1$ GB of RAM in total.</p><p>Find the minimum number of seconds needed to upload $n$ GBs of RAM!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first and only line of each test case contains two integers $n$ and $k$ ($1 \le n, k \le 100$)&nbsp;！ the number of GBs that you want to upload and the length of the time window respectively.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of seconds needed to upload $n$ GBs of RAM.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first and only line of each test case contains two integers $n$ and $k$ ($1 \le n, k \le 100$)&nbsp;！ the number of GBs that you want to upload and the length of the time window respectively.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of seconds needed to upload $n$ GBs of RAM.</p>





```input1|2,4,6
6
5 1
2 2
2 3
1 7
11 5
100 100
```




```output1
5
3
4
1
51
9901
```



## Note

<p>In the first test case, you can upload $1$ GB of RAM per second, so to upload $5$ GBs, you need $5$ seconds.</p><p>In the second test case, you can upload $1$ GB in the first second, $0$ GBs in the second second, and $1$ GB in the third second, which in total adds up to exactly $2$ GBs of uploaded RAM.</p><p>In the third test case, you can upload $1$ GB in the first second, $0$ GBs in the second second, $0$ GBs in the third second, and $1$ GB in the fourth second, which in total adds up to exactly $2$ GBs of uploaded RAM.</p>
