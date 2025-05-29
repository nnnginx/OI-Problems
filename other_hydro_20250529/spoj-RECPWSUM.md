<p>You are given a series defined by the following recurrence:</p>
<p style="text-align: left;"><strong>f<sub>0</sub> = x, f<sub>1</sub> = y</strong></p>
<p style="text-align: left;"><strong>f<sub>n</sub>&nbsp;= a * f<sub>n-1</sub> + b * f<sub>n-2</sub></strong></p>
<p style="text-align: left;">You are required to find the summation of the following series:</p>
<p style="text-align: left;"><strong>f<sub>0</sub><sup>k</sup>&nbsp;+ <strong>f<sub>1</sub><sup>k </sup>+ <strong><strong>f<sub>2</sub><sup>k&nbsp;</sup>+ ... + <strong><strong>f<sub>n</sub><sup>k</sup></strong></strong></strong></strong></strong></strong></p>
<p style="text-align: left;">The values <strong>a</strong>, <strong>b</strong>, <strong>x</strong>, <strong>y</strong>, <strong>n</strong>, <strong>k</strong> will be provided. Since the answer can be large, output it modulo <strong>1000000007</strong>.</p>
<h3>Input</h3>
<p>The first line contains a single integer <strong>T</strong> denoting the number of test cases. Each test case consists of <strong>six</strong> space separated integers on a single line, in the order: <strong>a</strong>, <strong>b</strong>,&nbsp;<strong>x</strong>, <strong>y,</strong>&nbsp;<strong>n,</strong>&nbsp;<strong>k</strong>.</p>
<h3>Output</h3>
<p>For each test case, output a single integer (on a separate line) denoting the summation of the series as mentioned above.</p>
<h3>Constraints</h3>
<p><strong>1 ¡Ü T <span style="font-weight: 700;">¡Ü 500</span></strong></p>
<p><strong>0 <span style="font-weight: 700;">¡Ü</span>&nbsp;a, b <span style="font-weight: 700;">¡Ü</span>&nbsp;100</strong></p>
<p><strong>0 <span style="font-weight: 700;">¡Ü</span>&nbsp;x, y <span style="font-weight: 700;">¡Ü</span>&nbsp;10<sup>9</sup></strong></p>
<p><strong>0 <span style="font-weight: 700;">¡Ü n <span style="font-weight: 700;">¡Ü 10<sup>15</sup></span></span></strong></p>
<p><strong>0 <span style="font-weight: 700;">¡Ü k <span style="font-weight: 700;">¡Ü 1000</span></span>&nbsp;</strong></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
1 1 0 1 3 0
1 1 0 1 3 1
1 1 0 1 4 2
1 1 0 1 4 3

<strong>Output:</strong>
4
4
15
37
</pre>
<h3>Explanation</h3>
<p>In all the sample test cases,&nbsp;<strong>f<sub>0</sub>&nbsp;= 0, f<sub>1</sub>&nbsp;= 1,&nbsp;f<sub>n</sub>&nbsp;= f<sub>n-1</sub>&nbsp;+ f<sub>n-2</sub></strong>, which is the regular <strong>Fibonacci</strong> series. The first few terms of the sequence are <strong>0, 1, 1, 2, 3, 5, ...</strong>.</p>
<ul>
<li>For the first case, the required sum is <span style="font-weight: 700;">0<sup>0</sup> + 1<sup>0</sup> + 1<sup>0</sup> + 2<sup>0</sup> = 4.</span></li>
<li>For the second case, the required sum is <strong>0<sup>1</sup> + 1<sup>1</sup> + 1<sup>1</sup> + 2<sup>1</sup> = 4</strong>.</li>
<li>For the third case, the required sum is <strong>0<sup>2</sup> + 1<sup>2</sup> + 1<sup>2</sup> + 2<sup>2</sup> + 3<sup>2</sup> = 15</strong>.</li>
<li>For the fourth case, the required sum is <strong>0<sup>3</sup> + 1<sup>3</sup> + 1<sup>3</sup> + 2<sup>3</sup> + 3<sup>3</sup> = 37</strong>.</li>
</ul>
<p><strong>Note</strong>: Time limit is set leniently to allow slow languages to pass.</p>