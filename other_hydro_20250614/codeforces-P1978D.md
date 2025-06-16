## Description

<div><p>Elections are taking place in Berland. There are $n$ candidates participating in the elections, numbered from $1$ to $n$. The $i$-th candidate has $a_i$ fans who will vote for him. Additionally, there are $c$ people who are undecided about their favorite candidate, let's call them <span class="tex-font-style-it">undecided</span>. Undecided people will vote for the candidate with the lowest number.</p><p>The candidate who receives the maximum number of votes wins the elections, and if multiple candidates receive the same maximum number of votes, the candidate with the lowest number among them wins.</p><p>You found these elections too boring and predictable, so you decided to exclude some candidates from them. If you do not allow candidate number $i$ to participate in the elections, all $a_i$ of his fans will become undecided, and will vote for the candidate with the lowest number.</p><p>You are curious to find, for each $i$ from $1$ to $n$, the minimum number of candidates that need to be excluded from the elections for candidate number $i$ to win the elections.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 2 \cdot 10^4$) �� the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $c$ ($1 \le n \le 2 \cdot 10^5$, $0 \le c \le 10^9$) �� the number of candidates in the elections and the number of undecided people.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$) �� the number of fans for each candidate.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $n$ integers, the $i$-th of which should be equal to the minimum number of candidates that need to be excluded from the elections for candidate number $i$ to win.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 2 \cdot 10^4$) �� the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $c$ ($1 \le n \le 2 \cdot 10^5$, $0 \le c \le 10^9$) �� the number of candidates in the elections and the number of undecided people.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$) �� the number of fans for each candidate.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output $n$ integers, the $i$-th of which should be equal to the minimum number of candidates that need to be excluded from the elections for candidate number $i$ to win.</p>





```input1|2,3,6,7,10,11
5
3 1
2 0 3
2 3
0 10
5 3
5 4 3 2 1
4 5
3 10 7 1
6 0
2 2 2 3 3 3
```




```output1
0 1 2
1 0
0 1 2 3 4
1 0 2 3
1 1 2 0 4 5
```



## Note

<p>In the first test case: </p><ul><li> If all candidates are allowed, candidate number $1$ will receive $3$ votes ($1$ undecided person will vote for him), candidate number $2$ will receive $0$ votes, and candidate number $3$ will receive $3$ votes. Therefore, candidate number $1$ wins (he received the same number of votes as candidate $3$, but his number is lower), so the answer for him is $0$.</li><li> If candidate number $1$ is not allowed, his $2$ fans will become undecided. Then candidate number $2$ will receive $3$ votes ($3$ undecided people will vote for him) and candidate number $3$ will receive $3$ votes. Therefore, candidate number $2$ wins (he received the same number of votes as candidate $3$, but his number is lower), so the answer for him is $1$.</li><li> If candidates with numbers $1$ and $2$ are not allowed, candidate number $3$ wins, so the answer for him is $2$.</li></ul><p>In the second test case, candidate number $1$ will win if candidate number $2$ is not allowed to participate.</p>
