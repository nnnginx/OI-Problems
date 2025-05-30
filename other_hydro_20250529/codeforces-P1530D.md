## Description

<div><p>Every December, VK traditionally holds an event for its employees named "Secret Santa". Here's how it happens.</p><p>$n$ employees numbered from $1$ to $n$ take part in the event. Each employee $i$ is assigned a different employee $b_i$, to which employee $i$ has to make a new year gift. Each employee is assigned to exactly one other employee, and nobody is assigned to themselves (but two employees may be assigned to each other). Formally, all $b_i$ must be distinct integers between $1$ and $n$, and for any $i$, $b_i \ne i$ must hold.</p><p>The assignment is usually generated randomly. This year, as an experiment, all event participants have been asked who they wish to make a gift to. Each employee $i$ has said that they wish to make a gift to employee $a_i$.</p><p>Find a valid assignment $b$ that maximizes the number of fulfilled wishes of the employees.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>Each test case consists of two lines. The first line contains a single integer $n$&nbsp;($2 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of participants of the event.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$&nbsp;($1 \le a_i \le n$; $a_i \ne i$)&nbsp;！ wishes of the employees in order from $1$ to $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print two lines.</p><p>In the first line, print a single integer $k$&nbsp;($0 \le k \le n$)&nbsp;！ the number of fulfilled wishes in your assignment.</p><p>In the second line, print $n$ distinct integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le n$; $b_i \ne i$)&nbsp;！ the numbers of employees assigned to employees $1, 2, \ldots, n$.</p><p>$k$ must be equal to the number of values of $i$ such that $a_i = b_i$, and must be as large as possible. If there are multiple answers, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>Each test case consists of two lines. The first line contains a single integer $n$&nbsp;($2 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of participants of the event.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$&nbsp;($1 \le a_i \le n$; $a_i \ne i$)&nbsp;！ wishes of the employees in order from $1$ to $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print two lines.</p><p>In the first line, print a single integer $k$&nbsp;($0 \le k \le n$)&nbsp;！ the number of fulfilled wishes in your assignment.</p><p>In the second line, print $n$ distinct integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le n$; $b_i \ne i$)&nbsp;！ the numbers of employees assigned to employees $1, 2, \ldots, n$.</p><p>$k$ must be equal to the number of values of $i$ such that $a_i = b_i$, and must be as large as possible. If there are multiple answers, print any.</p>





```input1
2
3
2 1 2
7
6 4 6 2 4 5 6
```




```output1
2
3 1 2
4
6 4 7 2 3 5 1
```



## Note

<p>In the first test case, two valid assignments exist: $[3, 1, 2]$ and $[2, 3, 1]$. The former assignment fulfills two wishes, while the latter assignment fulfills only one. Therefore, $k = 2$, and the only correct answer is $[3, 1, 2]$.</p>
