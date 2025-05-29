## Description

<div><p>$n$ ships set out to explore the depths of the ocean. The ships are numbered from $1$ to $n$ and follow each other in ascending order; the $i$-th ship has a durability of $a_i$.</p><p>The Kraken attacked the ships $k$ times in a specific order. First, it attacks the first of the ships, then the last, then the first again, and so on.</p><p>Each attack by the Kraken reduces the durability of the ship by $1$. When the durability of the ship drops to $0$, it sinks and is no longer subjected to attacks (thus the ship ceases to be the first or last, and the Kraken only attacks the ships that have not yet sunk). If all the ships have sunk, the Kraken has nothing to attack and it swims away.</p><p>For example, if $n=4$, $k=5$, and $a=[1, 2, 4, 3]$, the following will happen:</p><ol> <li> The Kraken attacks the first ship, its durability becomes zero and now $a = [2, 4, 3]$; </li><li> The Kraken attacks the last ship, now $a = [2, 4, 2]$; </li><li> The Kraken attacks the first ship, now $a = [1, 4, 2]$; </li><li> The Kraken attacks the last ship, now $a = [1, 4, 1]$; </li><li> The Kraken attacks the first ship, its durability becomes zero and now $a = [4, 1]$. </li></ol><p>How many ships were sunk after the Kraken's attack?</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $1 \le k \le 10^{15}$)&nbsp;！ the number of ships and how many times the Kraken will attack the ships.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the durability of the ships.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the number of ships sunk by the Kraken on a separate line.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $1 \le k \le 10^{15}$)&nbsp;！ the number of ships and how many times the Kraken will attack the ships.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the durability of the ships.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the number of ships sunk by the Kraken on a separate line.</p>





```input1|2,3,6,7,10,11
6
4 5
1 2 4 3
4 6
1 2 4 3
5 20
2 7 1 8 2
2 2
3 2
2 15
1 5
2 7
5 2
```




```output1
2
3
5
0
2
2
```


