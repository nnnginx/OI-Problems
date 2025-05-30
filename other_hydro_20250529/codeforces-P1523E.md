## Description

<div><center> <img class="tex-graphics" height="378px" src="./32082/file/Daj9FacQ.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center><p>To monitor cryptocurrency exchange rates trader William invented a wonderful device consisting of $n$ lights arranged in a row. The device functions in the following way:</p><p>Initially, all lights on William's device are turned off. At the beginning of a new iteration the device randomly, with a uniform distribution, picks a light that is turned off and turns it on, telling William which cryptocurrency he should invest in. After this iteration if any $k$ consecutive lights contain more than one turned on light, then the device finishes working.</p><p>William doesn't like uncertainty, so he wants you to calculate the expected value of the number of lights that are turned on in the device after it finishes working.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10$). Description of the test cases follows.</p><p>The only line for each test case contains two integers $n$ and $k$ ($2 \le k \le n \le 10^5$), which are the total number of lights and the length of subsegment of lights that are being checked, respectively.</p></div><div class="output-specification"><p>For each test case print the answer, modulo $10^9+7$. </p><p>Formally, let $M = 10^9+7$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10$). Description of the test cases follows.</p><p>The only line for each test case contains two integers $n$ and $k$ ($2 \le k \le n \le 10^5$), which are the total number of lights and the length of subsegment of lights that are being checked, respectively.</p>

## Output

<p>For each test case print the answer, modulo $10^9+7$. </p><p>Formally, let $M = 10^9+7$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p>

## Samples

```input1
3
3 2
15 2
40 15
```

```output1
333333338
141946947
329622137
```




## Note

<p><span class="tex-font-style-bf">Explanation of the first sample test case:</span></p><p>Let's write out all possible sequences of light toggles, which will make the device complete its operation:</p><ol> <li> $(1, 2)$ &nbsp;！ $2$ lights are turned on </li><li> $(1, 3, 2)$ &nbsp;！ $3$ lights are turned on </li><li> $(2, 1)$ &nbsp;！ $2$ lights are turned on </li><li> $(2, 3)$ &nbsp;！ $2$ lights are turned on </li><li> $(3, 2)$ &nbsp;！ $2$ lights are turned on </li><li> $(3, 1, 2)$ &nbsp;！ $3$ lights are turned on </li></ol><p>Then the final expected value will be equal to $\frac{2}{6}$ + $\frac{3}{6}$ + $\frac{2}{6}$ + $\frac{2}{6}$ + $\frac{2}{6}$ + $\frac{3}{6}$ = $\frac{14}{6}$ = $\frac{7}{3}$. </p><p>Then the required output will be $333333338$, since $333333338 \cdot 3 \equiv 7 \pmod{10^9+7}$.</p>
