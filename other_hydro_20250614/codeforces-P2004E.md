## Description

<div><p>Two players, Alice and Bob, are playing a game. They have $n$ piles of stones, with the $i$-th pile initially containing $a_i$ stones.</p><p>On their turn, a player can choose any pile of stones and take any positive number of stones from it, with one condition:</p><ul> <li> let the current number of stones in the pile be $x$. It is not allowed to take from the pile a number of stones $y$ such that the greatest common divisor of $x$ and $y$ is not equal to $1$. </li></ul><p>The player who cannot make a move loses. Both players play optimally (that is, if a player has a strategy that allows them to win, no matter how the opponent responds, they will win). Alice goes first.</p><p>Determine who will win.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) ¡ª the number of test cases.</p><p>Each test case consists of two lines:</p><ul> <li> the first line contains a single integer $n$ ($1 \le n \le 3 \cdot 10^5$); </li><li> the second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^7$). </li></ul><p>Additional constraint on the input: the sum of $n$ across all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output <span class="tex-font-style-tt">Alice</span> if Alice wins, or <span class="tex-font-style-tt">Bob</span> if Bob wins.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) ¡ª the number of test cases.</p><p>Each test case consists of two lines:</p><ul> <li> the first line contains a single integer $n$ ($1 \le n \le 3 \cdot 10^5$); </li><li> the second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^7$). </li></ul><p>Additional constraint on the input: the sum of $n$ across all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, output <span class="tex-font-style-tt">Alice</span> if Alice wins, or <span class="tex-font-style-tt">Bob</span> if Bob wins.</p>





```input1|2,3,6,7
3
3
3 2 9
4
3 3 6 1
5
1 2 3 4 5
```




```output1
Bob
Alice
Bob
```


