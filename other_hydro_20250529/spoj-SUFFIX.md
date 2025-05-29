<p>Find the smallest natural number X such that, if we write X in bases B<sub>1</sub>, B<sub>2</sub>, ..., B<sub>N</sub>, we get strings with suffixes S<sub>1</sub>, S<sub>2</sub>, ..., S<sub>N</sub>, respectively.</p>
<p>The possible digits are 0123456789ABCDEFG...XYZ, with values 0..35. Of course, the number written in base B consists only of the digits with values between 0 and B - 1.</p>
<h3>Input</h3>
<p>In the first line of input there is an integer N (1 ¡Ü N ¡Ü 10) from the task description.</p>
<p>In k<sup>th</sup> of the next N lines there is an integer B<sub>k</sub> (2 ¡Ü B<sub>k</sub> ¡Ü 36) and a suffix S<sub>k</sub>&nbsp;from the task description.</p>
<p>The given bases will be pairwise distinct. Also, the product of the powers B<sub>k</sub>&nbsp;^ lenght(S<sub>k</sub>) will be less than 10<sup>18</sup>.</p>
<h3>Output</h3>
<p>Print the required X, written in base 10.</p>
<h3>Example</h3>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;"><strong>input</strong>
3
5 22
11 A2
18 4

<strong>output</strong>
112</pre>
<pre><span style="font-family: 'Courier New', Courier, monospace;"><span style="font-size: 12px;"><strong>input
</strong>5
2 110
32 E
25 M3
28 2
7 2<strong>

output
</strong>53678</span></span></pre>