<p>One of DB and TN common interests is traveling. One day, they went to Grand Line and found One Piece !</p>
<p>The One Piece treasure has n gold coins (n is even). Both them like gold coins, but they evaluate them as different values. So they decided to divide those coins by following method :</p>
<p>DB and TN do n / 2 steps, at each step, DB choose 2 coins, TN takes the coin that she evaluates it greater, and DB take the rest coin.</p>
<p>Let¡¯s help DB find how to take the maximum value at possible.</p>

<h3>Input</h3>
<p>First line : a single integer n (n is even) ¨C the number of coins</p>

<p>Second line : n integers a<sub>1</sub>, a<sub>2</sub>, ¡­, a<sub>n. </sub>a<sub>i</sub> is the value of i<sup>th</sup> coin that TN evaluates.</p>

<p>Third line : n integers b<sub>1</sub>, b<sub>2</sub>, ¡­, b<sub>n. </sub>b<sub>i</sub> is the value of i<sup>th</sup> coin that DB evaluates.</p>

<h3>Output</h3>
<p>First line : an integer S ¨C the maximum value DB can take.</p>

<p>
Last n / 2 lines : i<sup>th</sup> line contains two number x and y (1 ¡Ü x, y ¡Ü n), are the indexes of two <br>coins that DB choose on i<sup>th</sup> step. Each coin must be chose exact one time.
</p>

<p>If there are multiple ways, just print any of them.</p>

<h3>Constraints</h3>
<p>2 ¡Ü n ¡Ü 500 000</p>
<p>1 ¡Ü a<sub>i</sub> ¡Ü 10<sup>9</sup></p>
<p>1 ¡Ü b<sub>i</sub> ¡Ü 10<sup>9</sup></p>
<p>Note that a<sub>1</sub>, a<sub>2</sub>, ¡­, a<sub>n</sub> are n distinct integers.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
6
6 10 11 18 5 14
1 7 6 12 15 1

<strong>Output:</strong>&nbsp;
28
5 1
2 6
3 4</pre>

<p><strong>Warning: large Input/Output data, be careful with certain languages</strong></p>