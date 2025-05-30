## Description

<div><p><span class="tex-font-style-bf">Please note the non-standard memory limit.</span></p><p>There are $n$ problems numbered with integers from $1$ to $n$. $i$-th problem has the complexity $c_i = 2^i$, tag $tag_i$ and score $s_i$.</p><p>After solving the problem $i$ it's allowed to solve problem $j$ if and only if $\text{IQ} &lt; |c_i - c_j|$ and $tag_i \neq tag_j$. After solving it your $\text{IQ}$ changes and becomes $\text{IQ} = |c_i - c_j|$ and you gain $|s_i - s_j|$ points.</p><p>Any problem can be the first. You can solve problems in any order and as many times as you want.</p><p>Initially your $\text{IQ} = 0$. Find the maximum number of points that can be earned.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ $(1 \le t \le 100)$ &nbsp;！ the number of test cases. </p><p>The first line of each test case contains an integer $n$ $(1 \le n \le 5000)$ &nbsp;！ the number of problems.</p><p>The second line of each test case contains $n$ integers $tag_1, tag_2, \ldots, tag_n$ $(1 \le tag_i \le n)$ &nbsp;！ tags of the problems.</p><p>The third line of each test case contains $n$ integers $s_1, s_2, \ldots, s_n$ $(1 \le s_i \le 10^9)$ &nbsp;！ scores of the problems.</p><p>It's guaranteed that sum of $n$ over all test cases does not exceed $5000$.</p></div><div class="output-specification"><p>For each test case print a single integer &nbsp;！ the maximum number of points that can be earned.</p></div>

## Input

<p>The first line contains a single integer $t$ $(1 \le t \le 100)$ &nbsp;！ the number of test cases. </p><p>The first line of each test case contains an integer $n$ $(1 \le n \le 5000)$ &nbsp;！ the number of problems.</p><p>The second line of each test case contains $n$ integers $tag_1, tag_2, \ldots, tag_n$ $(1 \le tag_i \le n)$ &nbsp;！ tags of the problems.</p><p>The third line of each test case contains $n$ integers $s_1, s_2, \ldots, s_n$ $(1 \le s_i \le 10^9)$ &nbsp;！ scores of the problems.</p><p>It's guaranteed that sum of $n$ over all test cases does not exceed $5000$.</p>

## Output

<p>For each test case print a single integer &nbsp;！ the maximum number of points that can be earned.</p>

## Samples

```input1
5
4
1 2 3 4
5 10 15 20
4
1 2 1 2
5 10 15 20
4
2 2 4 1
2 8 19 1
2
1 1
6 9
1
1
666
```

```output1
35
30
42
0
0
```




## Note

<p>In the first test case optimal sequence of solving problems is as follows: </p><ol> <li> $1 \rightarrow 2$, after that total score is $5$ and $\text{IQ} = 2$ </li><li> $2 \rightarrow 3$, after that total score is $10$ and $\text{IQ} = 4$ </li><li> $3 \rightarrow 1$, after that total score is $20$ and $\text{IQ} = 6$ </li><li> $1 \rightarrow 4$, after that total score is $35$ and $\text{IQ} = 14$ </li></ol><p>In the second test case optimal sequence of solving problems is as follows: </p><ol> <li> $1 \rightarrow 2$, after that total score is $5$ and $\text{IQ} = 2$ </li><li> $2 \rightarrow 3$, after that total score is $10$ and $\text{IQ} = 4$ </li><li> $3 \rightarrow 4$, after that total score is $15$ and $\text{IQ} = 8$ </li><li> $4 \rightarrow 1$, after that total score is $35$ and $\text{IQ} = 14$ </li></ol><p>In the third test case optimal sequence of solving problems is as follows: </p><ol> <li> $1 \rightarrow 3$, after that total score is $17$ and $\text{IQ} = 6$ </li><li> $3 \rightarrow 4$, after that total score is $35$ and $\text{IQ} = 8$ </li><li> $4 \rightarrow 2$, after that total score is $42$ and $\text{IQ} = 12$ </li></ol>
