<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/TREZOR/en/">English</a></td> 
<td width="50%"><a href="/problems/TREZOR/vn/">Vietnamese</a></td> 
</tr></tbody></table>



<p>Mirko decided to open a new business – bank vaults. A branch of the bank can be visualized in a plane,vaults being points in the plane. Mirko's branch contains exactly L·(A+1+B) vaults, so that each point
with integer coordinates inside the rectangle with corners (1, −A) and (L, B) contains one vault.</p>
<p>The vaults are watched by two guards – one at (0, −A), the other at (0, B). A guard can see a vault if
there are no other vaults on the line segment connecting them.</p>
<p>A vault is not secure if neither guard can see it, secure if only one guard can see it and super-secure if
both guards can see it.</p>
<p>Given A, B and L, output the number of insecure, secure and super-secure vaults.</p>

<h3>Input</h3>
<p>The first line contains integers A and B separated by a space (1 ≤ A ≤ 2000, 1 ≤ B ≤ 2000).</p>
<p>The second line contains the integer L (1 ≤ L ≤ 1 000 000 000).</p>

<h3>Output</h3>
<p>Output on three separate lines the numbers of insecure, secure and super-secure vaults.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1 1
3

<b>Output:</b>
2
2
5
</pre>


<pre><b>Input:</b>
2 3
4

<b>Output:</b>
0
16
8
</pre>

<pre><b>Input:</b>
7 11
1000000

<b>Output:</b>
6723409
2301730
9974861
</pre>