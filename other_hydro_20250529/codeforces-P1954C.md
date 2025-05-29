## Description

<div><p>You are given two integers $x$ and $y$ of the same length, consisting of digits from $1$ to $9$.</p><p>You can perform the following operation any number of times (possibly zero): swap the $i$-th digit in $x$ and the $i$-th digit in $y$.</p><p>For example, if $x=73$ and $y=31$, you can swap the $2$-nd digits and get $x=71$ and $y=33$.</p><p>Your task is to maximize the product of $x$ and $y$ using the aforementioned operation any number of times. If there are multiple answers, print any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $x$ ($1 \le x &lt; 10^{100}$).</p><p>The second line of each test case contains a single integer $y$ ($1 \le y &lt; 10^{100}$).</p><p>Additional constraint on input: the integers $x$ and $y$ consist only of digits from $1$ to $9$.</p></div><div class="output-specification"><p>For each test case, print two lines&nbsp;！ the first line should contain the number $x$ after performing the operations; similarly, the second line should contain the number $y$ after performing the operations. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $x$ ($1 \le x &lt; 10^{100}$).</p><p>The second line of each test case contains a single integer $y$ ($1 \le y &lt; 10^{100}$).</p><p>Additional constraint on input: the integers $x$ and $y$ consist only of digits from $1$ to $9$.</p>

## Output

<p>For each test case, print two lines&nbsp;！ the first line should contain the number $x$ after performing the operations; similarly, the second line should contain the number $y$ after performing the operations. If there are multiple answers, print any of them.</p>





```input1|2,3,6,7
3
73
31
2
5
3516
3982
```




```output1
71
33
5
2
3912
3586
```


