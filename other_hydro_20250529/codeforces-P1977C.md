## Description

<div><p>Nikita is a student passionate about number theory and algorithms. He faces an interesting problem related to an array of numbers.</p><p>Suppose Nikita has an array of integers $a$ of length $n$. He will call a subsequence$^\dagger$ of the array <span class="tex-font-style-it">special</span> if its <a href="https://en.wikipedia.org/wiki/Least_common_multiple">least common multiple (LCM)</a> is not contained in $a$. The LCM of an empty subsequence is equal to $0$.</p><p>Nikita wonders: what is the length of the longest <span class="tex-font-style-it">special</span> subsequence of $a$? Help him answer this question!</p><p>$^\dagger$ A sequence $b$ is a subsequence of $a$ if $b$ can be obtained from $a$ by the deletion of several (possibly, zero or all) elements, without changing the order of the remaining elements. For example, $[5,2,3]$ is a subsequence of $[1,5,7,8,2,4,3]$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 2000$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2000$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the length of the longest <span class="tex-font-style-it">special</span> subsequence of $a$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 2000$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2000$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the length of the longest <span class="tex-font-style-it">special</span> subsequence of $a$.</p>





```input1|2,3,6,7,10,11
6
5
1 2 4 8 16
6
3 2 10 20 60 1
7
2 3 4 6 12 100003 1200036
9
2 42 7 3 6 7 7 1 6
8
4 99 57 179 10203 2 11 40812
1
1
```




```output1
0
4
4
5
8
0
```



## Note

<p>In the first test case, the LCM of any non-empty subsequence is contained in $a$, so the answer is $0$.</p><p>In the second test case, we can take the subsequence $[3, 2, 10, 1]$, its LCM is equal to $30$, which is not contained in $a$.</p><p>In the third test case, we can take the subsequence $[2, 3, 6, 100\,003]$, its LCM is equal to $600\,018$, which is not contained in $a$.</p>
