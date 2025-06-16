## Description

<div><p>To celebrate his recovery, k1o0n has baked an enormous $n$ metres long potato casserole.</p><p>Turns out, Noobish_Monk just can't stand potatoes, so he decided to ruin k1o0n's meal. He has cut it into $k$ pieces, of lengths $a_1, a_2, \dots, a_k$ meters.</p><p>k1o0n wasn't keen on that. Luckily, everything can be fixed. In order to do that, k1o0n can do one of the following operations: </p><ul> <li> Pick a piece with length $a_i \ge 2$ and divide it into two pieces with lengths $1$ and $a_i - 1$. As a result, the number of pieces will increase by $1$; </li><li> Pick a slice $a_i$ and another slice with length $a_j=1$ ($i \ne j$) and merge them into one piece with length $a_i+1$. As a result, the number of pieces will decrease by $1$. </li></ul><p>Help k1o0n to find the minimum number of operations he needs to do in order to merge the casserole into one piece with length $n$.</p><p>For example, if $n=5$, $k=2$ and $a = [3, 2]$, it is optimal to do the following:</p><ol> <li> Divide the piece with length $2$ into two pieces with lengths $2-1=1$ and $1$, as a result $a = [3, 1, 1]$. </li><li> Merge the piece with length $3$ and the piece with length $1$, as a result $a = [4, 1]$. </li><li> Merge the piece with length $4$ and the piece with length $1$, as a result $a = [5]$.</li></ol></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). </p><p>Description of each test case consists of two lines. The first line contains two integers $n$ and $k$ ($2 \le n \le 10^9$, $2 \le k \le 10^5$)&nbsp;！ length of casserole and the number of pieces.</p><p>The second line contains $k$ integers $a_1, a_2, \ldots, a_k$ ($1 \le a_i \le n - 1$, $\sum a_i = n$)&nbsp;！ lengths of pieces of casserole, which Noobish_Monk has cut.</p><p>It is guaranteed that the sum of $k$ over all $t$ test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the minimum number of operations K1o0n needs to restore his pie after the terror of Noobish_Monk.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). </p><p>Description of each test case consists of two lines. The first line contains two integers $n$ and $k$ ($2 \le n \le 10^9$, $2 \le k \le 10^5$)&nbsp;！ length of casserole and the number of pieces.</p><p>The second line contains $k$ integers $a_1, a_2, \ldots, a_k$ ($1 \le a_i \le n - 1$, $\sum a_i = n$)&nbsp;！ lengths of pieces of casserole, which Noobish_Monk has cut.</p><p>It is guaranteed that the sum of $k$ over all $t$ test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the minimum number of operations K1o0n needs to restore his pie after the terror of Noobish_Monk.</p>





```input1|2,3,6,7
4
5 3
3 1 1
5 2
3 2
11 4
2 3 1 5
16 6
1 6 1 1 1 6
```




```output1
2
3
9
15
```


