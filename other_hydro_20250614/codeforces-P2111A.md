## Description

<div><p>There are three energy crystals numbered $1$, $2$, and $3$; let's denote the energy level of the $i$-th crystal as $a_i$. Initially, all of them are discharged, meaning their energy levels are equal to $0$. Each crystal needs to be charged to level $x$ <span class="tex-font-style-bf">(exactly $x$, not greater)</span>.</p><p>In one action, you can increase the energy level of any one crystal by any positive amount; however, the energy crystals are synchronized with each other, so an action can only be performed if the following condition is met afterward:</p><ul> <li> for each pair of crystals $i$, $j$, it must hold that $a_{i} \ge \lfloor\frac{a_{j}}{2}\rfloor$. </li></ul><p>What is the minimum number of actions required to charge all the crystals?</p></div><div class="input-specification"><p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10^{4}$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains a single integer $x$ ($1 \le x \le 10^{9}$).</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of actions required to charge all energy crystals to level $x$.</p></div>

## Input

<p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10^{4}$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains a single integer $x$ ($1 \le x \le 10^{9}$).</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of actions required to charge all energy crystals to level $x$.</p>





```input1|2,4,6,8
7
1
5
14
2025
31415
536870910
1000000000
```




```output1
3
7
9
23
31
59
61
```



## Note

<p>In the first test case, one possible sequence of actions is:</p><p>$$[0, 0, 0] \to [\color{red}{1}, 0, 0] \to [1, 0, \color{red}{1}] \to [1, \color{red}{1}, 1]$$</p><p>One of the possible sequences of actions in the second test case is:</p><p>$$[0, 0, 0] \to [\color{red}{1}, 0, 0] \to [1, \color{red}{1}, 0] \to [1, 1, \color{red}{2}] \to [\color{red}{3}, 1, 2] \to [3, \color{red}{5}, 2] \to [\color{red}{5}, 5, 2] \to [5, 5, \color{red}{5}]$$</p>
