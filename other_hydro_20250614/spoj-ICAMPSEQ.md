<p>Let's say we have 4 N-elements sequences of real numbers: A[], B[], C[], D[] .<br>
Funtion F(i, j) is defined: F(i, j) = |A<sub>i</sub> - A<sub>j</sub>| + |B<sub>i</sub> - B<sub>j</sub>| + |C<sub>i</sub> - C<sub>j</sub>| + |D<sub>i</sub> - D<sub>j</sub>| (1 ¡Ü i, j ¡Ü N).<br>
Your task is very easy: you have to find the maximum of F(i, j).

</p><h3>Input</h3>
<p>The first line: N (N ¡Ü 100000).<br>
Following are N lines: the i-th line contains four real numbers A<sub>i</sub>, B<sub>i</sub>, C<sub>i</sub>, D<sub>i</sub>. (-10<sup>9</sup> ¡Ü A<sub>i</sub>, B<sub>i</sub>, C<sub>i</sub>, D<sub>i</sub> ¡Ü 10<sup>9</sup>)

</p><h3>Output</h3>
<p>Only one line is the maximum of F(i, j).<br>
(The result takes exactly 3 decimal places)
</p><h3>Example</h3>

<pre><b>Input:</b>
2
1.0 1.0 2.0 0.5
1.0 1.0 0.5 2.0


<b>Output:</b>
3.000

</pre>