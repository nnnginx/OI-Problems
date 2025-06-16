## Description

<div><p><span class="tex-font-style-tt">ikrpprpp</span> found an array $a$ consisting of integers. He likes justice, so he wants to make $a$ fair&nbsp;！ that is, make it non-decreasing. To do that, he can perform an <span class="tex-font-style-it">act of justice</span> on an index $1 \le i \le n$ of the array, which will replace $a_i$ with $a_i ^ 2$ (the element at position $i$ with its square). For example, if $a = [2,4,3,3,5,3]$ and <span class="tex-font-style-tt">ikrpprpp</span> chooses to perform an act of justice on $i = 4$, $a$ becomes $[2,4,3,9,5,3]$.</p><p>What is the minimum number of acts of justice needed to make the array non-decreasing?</p></div><div class="input-specification"><p>First line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases. It is followed by the description of test cases.</p><p>For each test case, the first line contains an integer $n$&nbsp;！ size of the array $a$. The second line contains $n$ ($1 \le n \le 2 \cdot 10 ^5$) integers $a_1, a_2,\ldots, a_n$ ($1 \le a_i \le 10 ^ 6$). </p><p>The sum of $n$ over all test cases does not exceed $2 \cdot {10}^5$.</p></div><div class="output-specification"><p>For each testcase, print an integer&nbsp;！ minimum number of acts of justice required to make the array $a$ non-decreasing. If it is impossible to do that, print $-1$.</p></div>

## Input

<p>First line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases. It is followed by the description of test cases.</p><p>For each test case, the first line contains an integer $n$&nbsp;！ size of the array $a$. The second line contains $n$ ($1 \le n \le 2 \cdot 10 ^5$) integers $a_1, a_2,\ldots, a_n$ ($1 \le a_i \le 10 ^ 6$). </p><p>The sum of $n$ over all test cases does not exceed $2 \cdot {10}^5$.</p>

## Output

<p>For each testcase, print an integer&nbsp;！ minimum number of acts of justice required to make the array $a$ non-decreasing. If it is impossible to do that, print $-1$.</p>





```input1|2,3,6,7,10,11,14,15
7
3
1 2 3
2
3 2
3
3 1 5
4
1 1 2 3
3
4 3 2
9
16 2 4 2 256 2 4 2 8
11
10010 10009 10008 10007 10006 10005 10004 10003 10002 10001 10000
```




```output1
0
1
-1
0
3
15
55
```



## Note

<p>In the first test case, there's no need to perform acts of justice. The array is fair on its own!</p><p>In the third test case, it can be proven that the array cannot become non-decreasing.</p><p>In the fifth test case, <span class="tex-font-style-tt">ikrpprppp</span> can perform an act of justice on index 3, then an act of justice on index 2, and finally yet another act of justice on index 3. After that, $a$ will become $[4, 9, 16]$.</p>
