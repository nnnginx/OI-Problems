## Description

<div><p>You have been offered to play a game. In this game, there are $n$ possible outcomes, and for each of them, you must bet a certain <span class="tex-font-style-bf">integer</span> amount of coins. In the event that the $i$-th outcome turns out to be winning, you will receive back the amount of coins equal to your bet on that outcome, multiplied by $k_i$. Note that <span class="tex-font-style-bf">exactly one</span> of the $n$ outcomes will be winning.</p><p>Your task is to determine how to distribute the coins in such a way that you will come out ahead in the event of <span class="tex-font-style-bf">any</span> winning outcome. More formally, the total amount of coins you bet on all outcomes must be <span class="tex-font-style-bf">strictly less</span> than the number of coins received back for each possible winning outcome.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 50$)&nbsp;！ the number of outcomes.</p><p>The second line of each test case contains $n$ integers $k_1,k_2,\ldots,k_n$ ($2 \le k_i \le 20$)&nbsp;！ the multiplier for the amount of coins if the $i$-th outcome turns out to be winning.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $-1$ if there is no way to distribute the coins as required. Otherwise, output $n$ integers $x_1, x_2,\ldots, x_n$ ($1 \le x_i \le 10^{9}$)&nbsp;！ your bets on the outcomes.</p><p>It can be shown that if a solution exists, there is always a solution that satisfies these constraints.</p><p>If there are multiple suitable solutions, output any of them.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 50$)&nbsp;！ the number of outcomes.</p><p>The second line of each test case contains $n$ integers $k_1,k_2,\ldots,k_n$ ($2 \le k_i \le 20$)&nbsp;！ the multiplier for the amount of coins if the $i$-th outcome turns out to be winning.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output $-1$ if there is no way to distribute the coins as required. Otherwise, output $n$ integers $x_1, x_2,\ldots, x_n$ ($1 \le x_i \le 10^{9}$)&nbsp;！ your bets on the outcomes.</p><p>It can be shown that if a solution exists, there is always a solution that satisfies these constraints.</p><p>If there are multiple suitable solutions, output any of them.</p>





```input1|2,3,6,7,10,11
6
3
3 2 7
2
3 3
5
5 5 5 5 5
6
7 9 3 17 9 13
3
6 3 2
5
9 4 6 8 3
```




```output1
27 41 12 
1 1 
-1
1989 1547 4641 819 1547 1071 
-1
8 18 12 9 24
```



## Note

<p>In the first test case, the coins can be distributed as follows: $27$ coins on the first outcome, $41$ coins on the second outcome, $12$ coins on the third outcome. Then the total amount of coins bet on all outcomes is $27 + 41 + 12 = 80$ coins. If the first outcome turns out to be winning, you will receive back $3 \cdot 27 = 81$ coins, if the second outcome turns out to be winning, you will receive back $2 \cdot 41 = 82$ coins, if the third outcome turns out to be winning, you will receive back $7 \cdot 12 = 84$ coins. All these values are strictly greater than $80$.</p><p>In the second test case, one way is to bet one coin on each of the outcomes.</p>
