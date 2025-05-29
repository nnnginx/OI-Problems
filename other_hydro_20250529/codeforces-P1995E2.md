## Description

<div><p><span class="tex-font-style-bf">This is the hard version of a problem. The only difference between an easy and a hard version is the constraints on $t$ and $n$. You can make hacks only if both versions of the problem are solved.</span></p><p>Arthur is giving a lesson to his famous $2 n$ knights. Like any other students, they're sitting at the desks in pairs, but out of habit in a circle. The knight $2 i - 1$ is sitting at the desk with the knight $2 i$.</p><p>Each knight has <span class="tex-font-style-it">intelligence</span>, which can be measured by an integer. Let's denote the intelligence of the $i$-th knight as $a_i$. Arthur wants the maximal difference in total intelligence over all pairs of desks to be as small as possible. More formally, he wants to minimize $\max\limits_{1 \le i \le n} (a_{2 i - 1} + a_{2 i}) - \min\limits_{1 \le i \le n} (a_{2 i - 1} + a_{2 i})$.</p><p>However, the Code of Chivalry only allows swapping the opposite knights in the circle, i.e., Arthur can simultaneously perform $a_i := a_{i + n}$, $a_{i + n} := a_i$ for any $1 \le i \le n$. Arthur can make any number of such swaps. What is the best result he can achieve?</p></div><div class="input-specification"><p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;！ the number of test cases. It is followed by descriptions of the test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100\,000$)&nbsp;！ the number of desks.</p><p>The second line consists of $2n$ integers $a_1, a_2, \ldots, a_{2 n}$ ($1 \le a_i \le 10^9$)&nbsp;！ the intelligence values of the knights.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $100\,000$.</p></div><div class="output-specification"><p>For each test case, output a single line containing one integer&nbsp;！ the minimal difference Arthur can achieve.</p></div>

## Input

<p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;！ the number of test cases. It is followed by descriptions of the test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100\,000$)&nbsp;！ the number of desks.</p><p>The second line consists of $2n$ integers $a_1, a_2, \ldots, a_{2 n}$ ($1 \le a_i \le 10^9$)&nbsp;！ the intelligence values of the knights.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $100\,000$.</p>

## Output

<p>For each test case, output a single line containing one integer&nbsp;！ the minimal difference Arthur can achieve.</p>





```input1|2,3,6,7,10,11
5
2
6 6 4 4
1
10 17
3
1 10 1 10 1 10
3
3 3 4 5 5 4
5
1 2 3 4 5 6 7 8 9 10
```




```output1
0
0
0
2
4
```



## Note

<p>In the first test case, Arthur can swap the second and the fourth knights. Then the total intelligence at both desks will be $10$.</p><p>In the third test case, Arthur can make $0$ operations, which will result in the total intelligence of $11$ at each of the desks.</p><p>In the fourth test case, Arthur can swap knights with indices $2$ and $5$ and achieve the difference of $2$. It can be proven that he cannot improve his result any further.</p>
