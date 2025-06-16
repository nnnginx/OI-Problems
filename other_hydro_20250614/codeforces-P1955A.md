## Description

<div><p>The price of one yogurt at the "Vosmiorochka" store is $a$ burles, but there is a promotion where you can buy two yogurts for $b$ burles.</p><p>Maxim needs to buy <span class="tex-font-style-bf">exactly</span> $n$ yogurts. When buying two yogurts, he can choose to buy them at the regular price or at the promotion price.</p><p>What is the minimum amount of burles Maxim should spend to buy $n$ yogurts?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le {10}^{4}$)&nbsp;！ the number of test cases.</p><p>The first and only line of each test case contains three integers $n$, $a$, and $b$ ($1 \le n \le 100$, $1 \le a, b \le 30$)&nbsp;！ the number of yogurts Maxim wants to buy, the price for one yogurt, and the price for two yogurts on promotion.</p></div><div class="output-specification"><p>For each test case, print in a separate line the minimum cost of buying $n$ yogurts at "Vosmiorochka".</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le {10}^{4}$)&nbsp;！ the number of test cases.</p><p>The first and only line of each test case contains three integers $n$, $a$, and $b$ ($1 \le n \le 100$, $1 \le a, b \le 30$)&nbsp;！ the number of yogurts Maxim wants to buy, the price for one yogurt, and the price for two yogurts on promotion.</p>

## Output

<p>For each test case, print in a separate line the minimum cost of buying $n$ yogurts at "Vosmiorochka".</p>





```input1|2,4
4
2 5 9
3 5 9
3 5 11
4 5 11
```




```output1
9
14
15
20
```



## Note

<p>In the third test case of the example, it is more advantageous to buy three yogurts for $15$ burles than two for $11$ and one for $5$.</p><p>In the fourth test case of the example, you need to buy four yogurts, each for $5$ burles.</p>
