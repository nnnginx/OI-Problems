## Description

<div><p>You have a hand of $n$ cards, where each card has a number written on it, and a fixed integer $k$. You can perform the following operation any number of times:</p><ul> <li> Choose any $k$ cards from your hand that all have the same number. </li><li> Exchange these cards for $k-1$ cards, each of which can have <span class="tex-font-style-bf">any</span> number you choose (including the number written on the cards you just exchanged). </li></ul><p>Here is one possible sequence of operations for the first example case, which has $k=3$:</p><center> <img class="tex-graphics" src="./34607/file/l3tGbuc4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>What is the minimum number of cards you can have in your hand at the end of this process?</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 500$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 100$, $2 \le k \le 100$)&nbsp;！ the number of cards you have, and the number of cards you exchange during each operation, respectively.</p><p>The next line of each test case contains $n$ integers $c_1, c_2, \ldots c_n$ ($1 \le c_i \le 100$)&nbsp;！ the numbers written on your cards.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of cards you can have left in your hand after any number of operations.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 500$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 100$, $2 \le k \le 100$)&nbsp;！ the number of cards you have, and the number of cards you exchange during each operation, respectively.</p><p>The next line of each test case contains $n$ integers $c_1, c_2, \ldots c_n$ ($1 \le c_i \le 100$)&nbsp;！ the numbers written on your cards.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of cards you can have left in your hand after any number of operations.</p>





```input1|2,3,6,7,10,11,14,15
7
5 3
4 1 1 4 4
1 10
7
7 2
4 2 1 100 5 2 3
10 4
1 1 1 1 1 1 1 1 1 1
5 2
3 8 1 48 7
6 2
10 20 30 10 20 40
6 3
10 20 30 10 20 40
```




```output1
2
1
1
3
5
1
6
```



## Note

<p>The first example case corresponds to the picture above. The sequence of operations displayed there is optimal, so the answer is $2$.</p><p>In the second example case, no operations can be performed, so the answer is $1$.</p><p>In the fourth example case, you can repeatedly select $4$ cards numbered with $1$ and replace them with $3$ cards numbered with $1$, until there are $3$ cards left.</p>
