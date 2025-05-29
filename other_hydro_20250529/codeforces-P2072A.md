## Description

<div><p>Natsume Akito has just woken up in a new world and immediately received his first quest! The system provided him with an array $a$ of $n$ zeros, an integer $k$, and an integer $p$.</p><p>In one operation, Akito chooses two integers $i$ and $x$ such that $1 \le i \le n$ and $-p \le x \le p$, and performs the assignment $a_i = x$.</p><p>Akito is still not fully accustomed to controlling his new body, so help him calculate the minimum number of operations required to make the sum of all elements in the array equal to $k$, or tell him that it is impossible.</p></div><div class="input-specification"><p>The first line of input contains one integer $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>The only line of each test case contains three integers $n$, $k$, $p$ ($1 \le n \le 50$, $-2500 \le k \le 2500$, $1 \le p \le 50$) ！ the length of the array, the required sum, and the boundary of the segment from which numbers can be replaced.</p></div><div class="output-specification"><p>For each test case, output the minimum number of operations to achieve the final sum $k$ in the array, or $-1$ if it is impossible to achieve the sum $k$.</p></div>

## Input

<p>The first line of input contains one integer $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>The only line of each test case contains three integers $n$, $k$, $p$ ($1 \le n \le 50$, $-2500 \le k \le 2500$, $1 \le p \le 50$) ！ the length of the array, the required sum, and the boundary of the segment from which numbers can be replaced.</p>

## Output

<p>For each test case, output the minimum number of operations to achieve the final sum $k$ in the array, or $-1$ if it is impossible to achieve the sum $k$.</p>





```input1|2,4,6,8
8
21 100 10
9 -420 42
5 -7 2
13 37 7
10 0 49
1 10 9
7 -7 7
20 31 1
```




```output1
10
-1
4
6
0
-1
1
-1
```



## Note

<p>In the fifth example, the sum of the array is initially zero, so no operations are needed.</p><p>In the sixth example, the maximum sum in the array that we can achieve is $9$ (by assigning the number $9$ to the single element), so the sum $10$ cannot be obtained by any operations.</p><p>In the seventh example, only one operation $a_3 = -7$ is needed.</p>
