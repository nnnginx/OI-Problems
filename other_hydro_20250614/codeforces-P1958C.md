## Description

<div><p>It's pretty cold in Berland (yes, even in May). So Monocarp has to light his fireplace.</p><p>Monocarp has a big log of wood, which weighs $2^n$ grams. Monocarp has watched the weather forecast and decided that he has to burn $k$ grams of wood in the fireplace today, and the remaining $2^n-k$ grams of wood will be used tomorrow.</p><p>In one minute, Monocarp can use his saw to split one of his logs in half. Initially he has only one log, but of course, after splitting a log, he gets two new logs. If the weight of the log is $x$, then each of the resulting logs has weight equal to $\frac{x}{2}$. Monocarp can't split logs of weight $1$ gram.</p><p>Monocarp has to cut his log in such a way that some of the resulting logs weigh exactly $k$ grams in total (and since the total weight of wood doesn't change, the remaining logs will have a total weight equal to exactly $2^n-k$). Help him to calculate the minimum number of minutes he has to spend cutting the logs.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) �� the number of test cases.</p><p>Each test case consists of one line containing two integers $n$ and $k$ ($1 \le n \le 60$; $1 \le k \le 2^n-1$). </p></div><div class="output-specification"><p>For each test case, print one integer �� the minimum number of minutes Monocarp has to spend splitting the wood.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) �� the number of test cases.</p><p>Each test case consists of one line containing two integers $n$ and $k$ ($1 \le n \le 60$; $1 \le k \le 2^n-1$). </p>

## Output

<p>For each test case, print one integer �� the minimum number of minutes Monocarp has to spend splitting the wood.</p>





```input1|2,4
4
2 2
2 1
10 3
50 36679020707840
```




```output1
1
2
10
16
```



## Note

<p>In the first test case, Monocarp has to cut his log exactly once. Then he will have two logs weighing $2$ grams each.</p><p>In the second test case, Monocarp has to cut his log of $4$ grams once, then cut one of the resulting logs. He will have one log of weight $2$ and two logs of weight $1$, so he can use two logs to get exactly $3$ grams.</p>
