## Description

<div><p>In 2077, a sport called hobby-droning is gaining popularity among robots.</p><p>You already have a drone, and you want to win. For this, your drone needs to fly through a course with $n$ obstacles.</p><p>The $i$-th obstacle is defined by two numbers $l_i, r_i$. Let the height of your drone at the $i$-th obstacle be $h_i$. Then the drone passes through this obstacle if $l_i \le h_i \le r_i$. Initially, the drone is on the ground, meaning $h_0 = 0$.</p><p>The flight program for the drone is represented by an array $d_1, d_2, \ldots, d_n$, where $h_{i} - h_{i-1} = d_i$, and $0 \leq d_i \leq 1$. This means that your drone either does not change height between obstacles or rises by $1$. You already have a flight program, but some $d_i$ in it are unknown and marked as $-1$. Replace the unknown $d_i$ with numbers $0$ and $1$ to create a flight program that passes through the entire obstacle course, or report that it is impossible.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>In the first line of each test case, an integer $n$ ($1 \le n \le 2 \cdot 10^5)$ is given&nbsp;！ the size of the array $d$.</p><p>In the second line of each test case, there are $n$ integers $d_1, d_2, \ldots, d_n$ ($-1 \leq d_i \leq 1$)&nbsp;！ the elements of the array $d$. $d_i = -1$ means that this $d_i$ is unknown to you.</p><p>Next, there are $n$ lines containing $2$ integers $l_i,r_i$ ($0\leq l_i\leq r_i\leq n$)&nbsp;！ descriptions of the obstacles.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $n$ integers $d_1,d_2,\ldots,d_n$, if it is possible to correctly restore the array $d$, or $-1$ if it is not possible.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>In the first line of each test case, an integer $n$ ($1 \le n \le 2 \cdot 10^5)$ is given&nbsp;！ the size of the array $d$.</p><p>In the second line of each test case, there are $n$ integers $d_1, d_2, \ldots, d_n$ ($-1 \leq d_i \leq 1$)&nbsp;！ the elements of the array $d$. $d_i = -1$ means that this $d_i$ is unknown to you.</p><p>Next, there are $n$ lines containing $2$ integers $l_i,r_i$ ($0\leq l_i\leq r_i\leq n$)&nbsp;！ descriptions of the obstacles.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output $n$ integers $d_1,d_2,\ldots,d_n$, if it is possible to correctly restore the array $d$, or $-1$ if it is not possible.</p>





```input1|2,3,4,5,6,7,13,14,15,16,27,28,29
5
4
0 -1 -1 1
0 4
1 2
2 4
1 4
3
0 -1 -1
0 1
2 2
0 3
2
-1 -1
0 0
2 2
8
-1 -1 1 -1 -1 0 0 -1
0 0
0 1
0 2
0 2
1 3
0 4
2 5
4 5
1
0
1 1
```




```output1
0 1 1 1 
-1
-1
0 1 1 0 1 0 0 1 
-1
```



## Note

<p>In the first test case, one possible answer is $d=[0,1,1,1]$. The array $h$ will be $[0,0+1,0+1+1,0+1+1+1]=[0,1,2,3]$. This array meets the conditions of the problem.</p><p>In the second test case, it can be proven that there is no suitable array $d$, so the answer is $-1$.</p>
