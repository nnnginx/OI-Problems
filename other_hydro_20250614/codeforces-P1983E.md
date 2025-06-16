## Description

<div><p>Alice and Bob are playing a game. There are $n$ balls, out of which $k$ are special. Each ball has a value associated with it. </p><p>The players play turn by turn. In each turn, the player randomly picks a ball and adds the value of the ball to their score, which is $0$ at the beginning of the game. The selected ball is removed from the game. If the ball was special, the same player takes the next turn if at least one ball is remaining. If the ball picked was not special, the next player plays their turn.</p><p>They play this game until no balls are remaining in the game. Alice plays first.</p><p>Find the expected score that both the players have at the end of the game modulo $10^9+7$. </p><p>Formally, let $M = 10^9+7$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p></div><div class="input-specification"><p>There are multiple test cases. The first line of the input contains an integer $t$, the number of test cases ($1 \le t \le 2 \cdot 10^5$).</p><p>Each test case description is on a new line. The first line of the test case contains two integers $n$ and $k$ in the respective order separated by a space ($1 \le k \le n \le 4 \cdot 10^5$).</p><p>The second line of the test case contains $n$ integers: $v_1, v_2, \ldots, v_n$, the value for each ball separated by spaces. The first $k$ balls are special ($1 \le v_i \le 10^7$).</p><p>The sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>Output two integers per test case in a new line, the expected score of Alice and the expected score of Bob modulo $10^9+7$.</p></div>

## Input

<p>There are multiple test cases. The first line of the input contains an integer $t$, the number of test cases ($1 \le t \le 2 \cdot 10^5$).</p><p>Each test case description is on a new line. The first line of the test case contains two integers $n$ and $k$ in the respective order separated by a space ($1 \le k \le n \le 4 \cdot 10^5$).</p><p>The second line of the test case contains $n$ integers: $v_1, v_2, \ldots, v_n$, the value for each ball separated by spaces. The first $k$ balls are special ($1 \le v_i \le 10^7$).</p><p>The sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p>

## Output

<p>Output two integers per test case in a new line, the expected score of Alice and the expected score of Bob modulo $10^9+7$.</p>





```input1|2,3
1
5 2
10 20 5 15 25
```




```input2|2,3,6,7,10,11
5
1 1
732507
2 2
5817860 5398510
5 1
2122894 4951549 2750585 7821535 3214167
8 4
1405323 5069867 6883092 6972029 328406 2478975 7628890 9973340
4 2
9662050 3566134 3996473 9872255
```




```input3|2,3,6,7,10,11
5
3 3
1095611 8219204 7773462
2 1
8176490 2774103
3 1
9178636 5138057 3367761
12 9
7597698 6843019 2298534 1522386 4969588 1340345 3967362 9152890 6689668 9986080 4745473 7407325
10 5
6986368 2397882 5804127 6980694 3740836 3215836 5195724 3179261 4136769 4544231
```




```output1
45 30
```




```output2
732507 0
11216370 0
810642660 210218077
722402997 318336932
349086489 678010430
```




```output3
17088277 0
6862348 4088245
677038671 340645790
36949997 29570371
725118051 321063684
```



## Note

<p>In the first test case, Alice's expected score is $45$, and Bob's is $30$ at the end of the game.</p>
