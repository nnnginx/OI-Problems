## Description

<div><p>The little boy Nikita was given some cubes as a present. He decided to build a tower out of them.</p><p>Initially, the tower doesn't have any cubes. In one move, Nikita either puts exactly $1$ cube on top of the tower or removes exactly $1$ cube from the top of the tower. Is it possible that after $n$ moves, the resulting tower has exactly $m$ cubes?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 100$)&nbsp;�� the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 100$).</p></div><div class="output-specification"><p>For each test case, output "Yes" (without quotes) if Nikita can obtain a tower with $m$ cubes, and "No" (without quotes) otherwise.</p><p>You can output each letter in any case (lowercase or uppercase). For example, the strings "yEs", "yes", "Yes", and "YES" will be accepted as a positive answer.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 100$)&nbsp;�� the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 100$).</p>

## Output

<p>For each test case, output "Yes" (without quotes) if Nikita can obtain a tower with $m$ cubes, and "No" (without quotes) otherwise.</p><p>You can output each letter in any case (lowercase or uppercase). For example, the strings "yEs", "yes", "Yes", and "YES" will be accepted as a positive answer.</p>





```input1|2,4
3
3 3
2 4
5 3
```




```output1
Yes
No
Yes
```



## Note

<p>In the first test case, Nikita can put $1$ cube on top of the tower $3$ times in a row, so the answer is "Yes".</p><p>In the second test case, Nikita can only end up with either a tower with no blocks or a tower with $2$ blocks, so the answer is "No".</p>
