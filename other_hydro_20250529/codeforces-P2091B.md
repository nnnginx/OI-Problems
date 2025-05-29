## Description

<div><p>At the IT Campus "NEIMARK", there are training sessions in competitive programming&nbsp;！ both individual and team-based!</p><p>For the next team training session, $n$ students will attend, and the skill of the $i$-th student is given by a positive integer $a_i$.</p><p>The coach considers a team strong if its <span class="tex-font-style-it">strength</span> is at least $x$. The <span class="tex-font-style-it">strength</span> of a team is calculated as the number of team members multiplied by the minimum skill among the team members.</p><p>For example, if a team consists of $4$ members with skills $[5, 3, 6, 8]$, then the team's <span class="tex-font-style-it">strength</span> is $4 \cdot min([5, 3, 6, 8]) = 12$.</p><p>Output the maximum possible number of strong teams, given that each team must have at least one participant and every participant must belong to exactly one team.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $x$ ($1 \leq n \leq 2 \cdot 10^5$, $1 \leq x \leq 10^9$)&nbsp;！ the number of students in training and the minimum <span class="tex-font-style-it">strength</span> of a team to be considered strong.</p><p>The second line of each test case contains $n$ integers $a_i$ ($1 \leq a_i \leq 10^9$)&nbsp;！ the skill of each student.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the maximum possible number of teams with <span class="tex-font-style-it">strength</span> at least $x$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $x$ ($1 \leq n \leq 2 \cdot 10^5$, $1 \leq x \leq 10^9$)&nbsp;！ the number of students in training and the minimum <span class="tex-font-style-it">strength</span> of a team to be considered strong.</p><p>The second line of each test case contains $n$ integers $a_i$ ($1 \leq a_i \leq 10^9$)&nbsp;！ the skill of each student.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the maximum possible number of teams with <span class="tex-font-style-it">strength</span> at least $x$.</p>





```input1|2,3,6,7,10,11
5
6 4
4 5 3 3 2 6
4 10
4 2 1 3
5 3
5 3 2 3 2
3 6
9 1 7
6 10
6 1 3 6 3 2
```




```output1
4
0
4
2
1
```


