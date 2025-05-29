## Description

<div><p>A digit is <span class="tex-font-style-it">large</span> if it is between $5$ and $9$, inclusive. A positive integer is <span class="tex-font-style-it">large</span> if all of its digits are large.</p><p>You are given an integer $x$. Can it be the sum of two <span class="tex-font-style-it">large</span> positive integers with the <span class="tex-font-style-bf">same number of digits</span>?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;¡ª the number of test cases.</p><p>The only line of each test case contains a single integer $x$ ($10 \leq x \leq 10^{18}$).</p></div><div class="output-specification"><p>For each test case, output $\texttt{YES}$ if $x$ satisfies the condition, and $\texttt{NO}$ otherwise.</p><p>You can output $\texttt{YES}$ and $\texttt{NO}$ in any case (for example, strings $\texttt{yES}$, $\texttt{yes}$, and $\texttt{Yes}$ will be recognized as a positive response).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;¡ª the number of test cases.</p><p>The only line of each test case contains a single integer $x$ ($10 \leq x \leq 10^{18}$).</p>

## Output

<p>For each test case, output $\texttt{YES}$ if $x$ satisfies the condition, and $\texttt{NO}$ otherwise.</p><p>You can output $\texttt{YES}$ and $\texttt{NO}$ in any case (for example, strings $\texttt{yES}$, $\texttt{yes}$, and $\texttt{Yes}$ will be recognized as a positive response).</p>





```input1|2,4,6,8,10,12
11
1337
200
1393938
1434
98765432123456789
11111111111111111
420
1984
10
69
119
```




```output1
YES
NO
YES
YES
NO
YES
NO
YES
YES
NO
NO
```



## Note

<p>In the first test case, we can have $658 + 679 = 1337$.</p><p>In the second test case, it can be shown that no numbers of equal length and only consisting of large digits can add to $200$.</p><p>In the third test case, we can have $696\,969 + 696\,969 = 1\,393\,938$.</p><p>In the fourth test case, we can have $777 + 657 = 1434$.</p>
