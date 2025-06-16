## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://youtu.be/kSjj0LlsqnI"><span class="tex-font-style-it">Ngọt - LẦN CUỐI (đi bên em xót xa người ơi)</span></a></div><div class="epigraph-source">ඞ</div></div><p>There are $n$ lamps numbered $1$ to $n$ lined up in a row, initially turned off. You can perform the following operation any number of times (possibly zero): </p><ul> <li> Choose two <span class="tex-font-style-bf">non-adjacent</span>${}^\dagger$ lamps that are currently turned off, then turn them on. </li></ul><p>Determine whether you can reach configuration $s$, where $s_i = 1$ means the $i$-th lamp is turned on, and $s_i = 0$ otherwise.</p><p>${}^\dagger$ Only lamp $i$ and $i + 1$ are adjacent for all $1 \le i &lt; n$. Note that lamp $n$ and $1$ are <span class="tex-font-style-bf">not</span> adjacent when $n \ne 2$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 50$)&nbsp;— the number of lamps.</p><p>The second line of each test case contains a binary string $s$ of size $n$&nbsp;— the final desired configuration.</p></div><div class="output-specification"><p>For each test case, print on one line <span class="tex-font-style-tt">"YES"</span> if we can reach the configuration $s$ via applying the given operation any number of times. Otherwise, print <span class="tex-font-style-tt">"NO"</span>.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 50$)&nbsp;— the number of lamps.</p><p>The second line of each test case contains a binary string $s$ of size $n$&nbsp;— the final desired configuration.</p>

## Output

<p>For each test case, print on one line <span class="tex-font-style-tt">"YES"</span> if we can reach the configuration $s$ via applying the given operation any number of times. Otherwise, print <span class="tex-font-style-tt">"NO"</span>.</p>





```input1|2,3,6,7,10,11
5
10
1101010110
10
1001001110
6
000000
1
1
12
111111111111
```




```output1
YES
NO
YES
NO
YES
```



## Note

<p>In the first test case, the sequence of operation could have been as follows (note that initially $s$ is all zero): $\mathtt{0000000000} \to \mathtt{\color{red}{1}0000000\color{red}{1}0} \to \mathtt{1\color{red}{1}00000\color{red}{1}10} \to \mathtt{110\color{red}{1}0\color{red}{1}0110}$.</p><p>In the third test case, we don't have to do any operation.</p><p>In the fourth test case, we cannot do any operation, but we need the first lamp to be on. Therefore, it is impossible to achieve the desired state.</p>
