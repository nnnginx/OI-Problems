## Description

<div><p>In anticipation of a duel with his old friend Fernan, Edmond is preparing an energy drink called "<span class="tex-font-style-tt">Mishkin Energizer</span>". The drink consists of a string $s$ of length $n$, made up only of the characters <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">I</span>, and <span class="tex-font-style-tt">T</span>, which correspond to the content of three different substances in the drink.</p><p>We call the drink <span class="tex-font-style-it">balanced</span> if it contains an equal number of all substances. To boost his aura and ensure victory in the duel, Edmond must make the initial string balanced by applying the following operation: </p><ol> <li> Choose an index $i$ such that $s_i \neq s_{i+1}$ (where $i + 1$ must not exceed the <span class="tex-font-style-bf">current</span> size of the string). </li><li> Insert a character $x$, either <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">I</span>, or <span class="tex-font-style-tt">T</span>, between them such that $x \neq s_i$ and $x \neq s_{i+1}$. </li></ol><p>Help Edmond make the drink balanced and win the duel by performing <span class="tex-font-style-bf">no more than $\textbf{2n}$ operations</span>. If there are multiple solutions, any one of them can be output. If it is impossible, you must report this.</p></div><div class="input-specification"><p>Each test consists of several test cases. The first line of the input data contains one integer $t$ ($1 \le t \le 100$) ！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 100$) ！ the length of the string $s$.</p><p>The second line of each test case contains a string $s$ of length $n$, consisting only of the characters <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">I</span>, and <span class="tex-font-style-tt">T</span>.</p></div><div class="output-specification"><p>For each test case, output $-1$ if there is no solution. Otherwise, in the first line, output a single integer $m$ ($0 \le m \le 2n$) ！ the number of operations you performed.</p><p>Then the $l$-th of the following $m$ lines should contain a single integer $i$ ($1 \le i &lt; n+l-1$), indicating the operation of inserting a character between $s_i$ and $s_{i+1}$. It must hold that $s_i \neq s_{i+1}$.</p><p>If there are multiple solutions, any one of them can be output. Note that you do not need to minimize the number of operations in this problem.</p></div>

## Input

<p>Each test consists of several test cases. The first line of the input data contains one integer $t$ ($1 \le t \le 100$) ！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 100$) ！ the length of the string $s$.</p><p>The second line of each test case contains a string $s$ of length $n$, consisting only of the characters <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">I</span>, and <span class="tex-font-style-tt">T</span>.</p>

## Output

<p>For each test case, output $-1$ if there is no solution. Otherwise, in the first line, output a single integer $m$ ($0 \le m \le 2n$) ！ the number of operations you performed.</p><p>Then the $l$-th of the following $m$ lines should contain a single integer $i$ ($1 \le i &lt; n+l-1$), indicating the operation of inserting a character between $s_i$ and $s_{i+1}$. It must hold that $s_i \neq s_{i+1}$.</p><p>If there are multiple solutions, any one of them can be output. Note that you do not need to minimize the number of operations in this problem.</p>





```input1|2,3,6,7
3
5
TILII
1
L
3
LIT
```




```output1
4
1
2
3
4
-1
0
```



## Note

<p>In the first test case, the following sequence of operations can be performed: <span class="tex-font-style-tt">TILII</span> $\rightarrow$ <span class="tex-font-style-tt">T<span class="tex-font-style-bf">L</span>ILII</span> $\rightarrow$ <span class="tex-font-style-tt">TL<span class="tex-font-style-bf">T</span>ILII</span> $\rightarrow$ <span class="tex-font-style-tt">TLT<span class="tex-font-style-bf">L</span>ILII</span> $\rightarrow$ <span class="tex-font-style-tt">TLTL<span class="tex-font-style-bf">T</span>ILII</span>.</p><p>In the second test case, no operations can be performed, so the answer is $-1$.</p><p>In the third test case, the initial string already has equal quantities of all substances.</p>
