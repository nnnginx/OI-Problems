<p>For two given integers n and k find (Z<sub>n</sub> + Z<sub>n-1</sub> - 2Z<sub>n-2</sub>) mod 10000007, where Z<sub>n</sub> = S<sub>n</sub> + P<sub>n</sub> and S<sub>n</sub> = 1<sup>k</sup> + 2<sup>k</sup> + 3<sup>k</sup> + �� + n<sup>k</sup> and P<sub>n</sub> = 1<sup>1</sup> + 2<sup>2</sup> + 3<sup>3</sup> + �� + n<sup>n</sup>.</p>

<h3>Input</h3>
<p>There are several test cases (�� 10000). In each case two space separated positive integers n and k are given.<br> For last test case n and k are given&nbsp;as 0 0, which is&nbsp;not to be processed.</p>

<h3>Constraints</h3>
<p>
1 &lt; n &lt; 200000000<br>
0 &lt; k &lt; 1000000
</p>

<h3>Output</h3>
<p>For each case print the asked value in separate line.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
10 3
9 31
83 17
5 2
0 0

<strong>Output:</strong>
4835897
2118762
2285275
3694</pre>