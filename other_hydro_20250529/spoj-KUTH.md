<p>One day Mirko was cleaning up his room and found a straightedge and a compass. He went to the school the next day and challenged his friend Slavko to a geometric construction battle. Mirko knows how to construct some angles using the straightedge and compass and knows how to subtract and add any two angels he constructs. Slavko now shouts random angles and Mirko must draw them as fast as possible. You are observing this battle and would like to know if Mirko can construct the angles Slavko shouts at all.</p>
<h3>Input</h3>
<p>The first line of input contains two integers, N (1 ¡Ü N ¡Ü 100000), number of angles Mirko knows how to construct initially and K (1 ¡Ü K ¡Ü 100000), number of angles Slavko selected. The second line of input contains N positive real numbers with exactly 6 decimal digits, all smaller than 360, the angles Mirko knows how to construct initially. The third line contains K positive real numbers with exactly 6 decimal digits, all smaller than 360, the angles Slavko selected.</p>
<h3>Output</h3>
<p>Output consist of K lines, one for each angle Slavko selected. The i-th line should contain "YES" if Mirko can construct the i-th angle, and "NO" otherwise.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 1
30.000000 70.000000
40.000000

<strong>Output:</strong>
YES

<strong>Input:</strong>
1 1
100.000000
60.000000

<strong>Output:</strong>
YES

<strong>Input:</strong>
3 2
10.000000 20.000000 30.000000
5.000000 70.000000

<strong>Output:</strong>
NO
YES
</pre>