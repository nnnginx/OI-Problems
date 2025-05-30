## Description

<div><p>There is a road with length $l$ meters. The start of the road has coordinate $0$, the end of the road has coordinate $l$.</p><p>There are two cars, the first standing at the start of the road and the second standing at the end of the road. They will start driving simultaneously. The first car will drive from the start to the end and the second car will drive from the end to the start.</p><p>Initially, they will drive with a speed of $1$ meter per second. There are $n$ flags at <span class="tex-font-style-bf">different</span> coordinates $a_1, a_2, \ldots, a_n$. Each time when any of two cars drives through a flag, the speed of that car increases by $1$ meter per second.</p><p>Find how long will it take for cars to meet (to reach the same coordinate). </p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$): the number of test cases.</p><p>The first line of each test case contains two integers $n$, $l$ ($1 \leq n \leq 10^5$, $1 \leq l \leq 10^9$): the number of flags and the length of the road.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ in the <span class="tex-font-style-bf">increasing</span> order ($1 \leq a_1 &lt; a_2 &lt; \ldots &lt; a_n &lt; l$).</p><p>It is guaranteed that the sum of $n$ among all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print a single real number: the time required for cars to meet.</p><p>Your answer will be considered correct, if its absolute or relative error does not exceed $10^{-6}$. More formally, if your answer is $a$ and jury's answer is $b$, your answer will be considered correct if $\frac{|a-b|}{\max{(1, b)}} \leq 10^{-6}$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$): the number of test cases.</p><p>The first line of each test case contains two integers $n$, $l$ ($1 \leq n \leq 10^5$, $1 \leq l \leq 10^9$): the number of flags and the length of the road.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ in the <span class="tex-font-style-bf">increasing</span> order ($1 \leq a_1 &lt; a_2 &lt; \ldots &lt; a_n &lt; l$).</p><p>It is guaranteed that the sum of $n$ among all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print a single real number: the time required for cars to meet.</p><p>Your answer will be considered correct, if its absolute or relative error does not exceed $10^{-6}$. More formally, if your answer is $a$ and jury's answer is $b$, your answer will be considered correct if $\frac{|a-b|}{\max{(1, b)}} \leq 10^{-6}$.</p>

## Samples

```input1
5
2 10
1 9
1 10
1
5 7
1 2 3 4 6
2 1000000000
413470354 982876160
9 478
1 10 25 33 239 445 453 468 477
```

```output1
3.000000000000000
3.666666666666667
2.047619047619048
329737645.750000000000000
53.700000000000000
```




## Note

<p>In the first test case cars will meet in the coordinate $5$.</p><p>The first car will be in the coordinate $1$ in $1$ second and after that its speed will increase by $1$ and will be equal to $2$ meters per second. After $2$ more seconds it will be in the coordinate $5$. So, it will be in the coordinate $5$ in $3$ seconds.</p><p>The second car will be in the coordinate $9$ in $1$ second and after that its speed will increase by $1$ and will be equal to $2$ meters per second. After $2$ more seconds it will be in the coordinate $5$. So, it will be in the coordinate $5$ in $3$ seconds.</p><p>In the second test case after $1$ second the first car will be in the coordinate $1$ and will have the speed equal to $2$ meters per second, the second car will be in the coordinate $9$ and will have the speed equal to $1$ meter per second. So, they will meet after $\frac{9-1}{2+1} = \frac{8}{3}$ seconds. So, the answer is equal to $1 + \frac{8}{3} = \frac{11}{3}$.</p>
