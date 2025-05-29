## Description

<div><p>Alice and Bob have bought a ribbon consisting of $n$ parts. Now they want to paint it.</p><p>First, Alice will paint every part of the ribbon into one of $m$ colors. For each part, she can choose its color arbitrarily.</p><p>Then, Bob will choose <span class="tex-font-style-bf">at most $k$</span> parts of the ribbon and repaint them <span class="tex-font-style-bf">into the same color</span> (he chooses the affected parts and the color arbitrarily).</p><p>Bob would like all parts to have the same color. However, Alice thinks that this is too dull, so she wants to paint the ribbon in such a way that Bob cannot make all parts have the same color.</p><p>Is it possible to paint the ribbon in such a way?</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>Each test case consists of one line containing three integers $n$, $m$ and $k$ ($1 \le m, k \le n \le 50$) ！ the number of parts, the number of colors and the number of parts Bob can repaint, respectively.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if Alice can paint the ribbon so that Bob cannot make all parts have the same color. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p><p>You can print every letter in any register. For example, <span class="tex-font-style-tt">Yes</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">yEs</span> will all be recognized as positive answer.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>Each test case consists of one line containing three integers $n$, $m$ and $k$ ($1 \le m, k \le n \le 50$) ！ the number of parts, the number of colors and the number of parts Bob can repaint, respectively.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if Alice can paint the ribbon so that Bob cannot make all parts have the same color. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p><p>You can print every letter in any register. For example, <span class="tex-font-style-tt">Yes</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">yEs</span> will all be recognized as positive answer.</p>





```input1|2,4,6
5
1 1 1
5 1 1
5 2 1
5 2 2
5 5 3
```




```output1
NO
NO
YES
NO
YES
```



## Note

<p>In the first test case, a ribbon consists of $1$ part. So all its parts will always have the same color.</p><p>In the second test case, there is only $1$ color.</p><p>In the third test case, Alice can paint the ribbon as follows: $[1, 2, 1, 2, 1]$. It's impossible to change the color of at most $1$ part so that all parts have the same color.</p><p>In the fourth test case, no matter how Alice paints the ribbon, Bob will always be able to repaint $2$ parts so that all parts have the same color.</p><p>In the fifth test case, Alice can paint the ribbon as follows: $[1, 2, 3, 4, 5]$. It's impossible to change the color of at most $3$ parts so that all parts have the same color.</p>
