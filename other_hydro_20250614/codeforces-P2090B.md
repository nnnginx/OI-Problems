## Description

<div><p>Ecrade has an $n \times m$ grid, originally empty, and he has pushed several (possibly, zero) balls in it.</p><p>Each time, he can push one ball into the grid either from the leftmost edge of a particular row or the topmost edge of a particular column of the grid.</p><p>When a ball moves towards a position:</p><ul> <li> If there is no ball originally at that position, the incoming ball will stop and occupy the position. </li><li> If there is already a ball at that position, the incoming ball will stop and occupy the position, while the original ball will continue moving to the next position in the same direction. </li></ul><p>Note that if a row or column is full (i.e., all positions in that row or column have balls), he cannot push a ball into that row or column.</p><p>Given the final state of whether there is a ball at each position of the grid, you need to determine whether it is possible for Ecrade to push the balls to reach the final state.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10\,000$) ¡ª the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 50$).</p><p>This is followed by $n$ lines, each containing exactly $m$ characters and consisting only of $0$ and $1$, describing the final state of the grid. There is a ball at one position of the grid if and only if the corresponding position of the given input is $1$.</p><p>It is guaranteed that the sum of $n\cdot m$ over all test cases does not exceed $10\,000$.</p></div><div class="output-specification"><p>For each test case, output "Yes" (without quotes) if it is possible for Ecrade to push the balls to reach the final state, and "No" (without quotes) otherwise.</p><p>You can output "Yes" and "No" in any case (for example, strings "YES", "yEs" and "yes" will be recognized as a positive response).</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10\,000$) ¡ª the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 50$).</p><p>This is followed by $n$ lines, each containing exactly $m$ characters and consisting only of $0$ and $1$, describing the final state of the grid. There is a ball at one position of the grid if and only if the corresponding position of the given input is $1$.</p><p>It is guaranteed that the sum of $n\cdot m$ over all test cases does not exceed $10\,000$.</p>

## Output

<p>For each test case, output "Yes" (without quotes) if it is possible for Ecrade to push the balls to reach the final state, and "No" (without quotes) otherwise.</p><p>You can output "Yes" and "No" in any case (for example, strings "YES", "yEs" and "yes" will be recognized as a positive response).</p>





```input1|2,3,4,5,10,11,12,13,18,19,20,21
5
3 3
001
001
110
3 3
010
111
010
3 3
111
111
111
3 3
000
000
000
3 3
000
000
001
```




```output1
YES
YES
YES
YES
NO
```



## Note

<p>For simplicity, if Ecrade pushes a ball from the leftmost edge of the $i$-th row, we call the operation $\text{ROW}\ i$; if he pushes a ball from the topmost edge of the $i$-th column, we call the operation $\text{COL}\ i$.</p><p>For intuitive understanding, a non-zero number $x$ in the matrix given below represents the $x$-th ball that is pushed in.</p><p>In the first test case, a possible series of operations:</p><p>$\begin{pmatrix}0&amp;0&amp;0\\0&amp;0&amp;0\\0&amp;0&amp;0\end{pmatrix}\xrightarrow{\text{ROW}\ 3}\xrightarrow{\text{ROW}\ 3} \begin{pmatrix}0&amp;0&amp;0\\0&amp;0&amp;0\\2&amp;1&amp;0\end{pmatrix}\xrightarrow{\text{COL}\ 3}\xrightarrow{\text{COL}\ 3} \begin{pmatrix}0&amp;0&amp;4\\0&amp;0&amp;3\\2&amp;1&amp;0\end{pmatrix}$</p><p>In the second test case, a possible series of operations:</p><p>$\begin{pmatrix}0&amp;0&amp;0\\0&amp;0&amp;0\\0&amp;0&amp;0\end{pmatrix}\xrightarrow{\text{ROW}\ 2}\xrightarrow{\text{ROW}\ 2}\xrightarrow{\text{ROW}\ 2} \begin{pmatrix}0&amp;0&amp;0\\3&amp;2&amp;1\\0&amp;0&amp;0\end{pmatrix}\xrightarrow{\text{COL}\ 2}\xrightarrow{\text{COL}\ 2} \begin{pmatrix}0&amp;5&amp;0\\3&amp;4&amp;1\\0&amp;2&amp;0\end{pmatrix}$</p><p>In the third test case, a possible series of operations:</p><p>$\begin{pmatrix}0&amp;0&amp;0\\0&amp;0&amp;0\\0&amp;0&amp;0\end{pmatrix}\xrightarrow{\text{ROW}\ 1}\xrightarrow{\text{ROW}\ 2}\xrightarrow{\text{ROW}\ 3} \begin{pmatrix}1&amp;0&amp;0\\2&amp;0&amp;0\\3&amp;0&amp;0\end{pmatrix}\xrightarrow{\text{COL}\ 3}\xrightarrow{\text{COL}\ 3}\xrightarrow{\text{COL}\ 3} \begin{pmatrix}1&amp;0&amp;6\\2&amp;0&amp;5\\3&amp;0&amp;4\end{pmatrix}\xrightarrow{\text{ROW}\ 1}\xrightarrow{\text{ROW}\ 2}\xrightarrow{\text{ROW}\ 3} \begin{pmatrix}7&amp;1&amp;6\\8&amp;2&amp;5\\9&amp;3&amp;4\end{pmatrix}$</p>
