## Description

<div><p>Let's call an integer sequence <span class="tex-font-style-bf">beautiful</span> if the following conditions hold: </p><ul> <li> its length is at least $3$; </li><li> for every element except the first one, there is an element to the left less than it; </li><li> for every element except the last one, there is an element to the right larger than it; </li></ul><p>For example, $[1, 4, 2, 4, 7]$ and $[1, 2, 4, 8]$ are beautiful, but $[1, 2]$, $[2, 2, 4]$, and $[1, 3, 5, 3]$ are not.</p><p>Recall that a subsequence is a sequence that can be obtained from another sequence by removing some elements without changing the order of the remaining elements.</p><p>You are given an integer array $a$ of size $n$, where <span class="tex-font-style-bf">every element is from $1$ to $3$</span>. Your task is to calculate the number of beautiful subsequences of the array $a$. Since the answer might be large, print it modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 3$).</p><p>Additional constraint on the input: the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the number of beautiful subsequences of the array $a$, taken modulo $998244353$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 3$).</p><p>Additional constraint on the input: the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;！ the number of beautiful subsequences of the array $a$, taken modulo $998244353$.</p>





```input1|2,3,6,7
4
7
3 2 1 2 2 1 3
4
3 1 2 2
3
1 2 3
9
1 2 3 2 1 3 2 2 3
```




```output1
3
0
1
22
```



## Note

<p>In the first test case of the example, the following subsequences are beautiful:</p><ul> <li> $[a_3, a_4, a_7]$; </li><li> $[a_3, a_5, a_7]$; </li><li> $[a_3, a_4, a_5, a_7]$. </li></ul>
