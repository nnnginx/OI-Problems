<p>Ben just learned about range-queries. He was so fascinated of them that he even wanted to create his own problem involving range-queries. He was thinking about the power function: let pow(a, b) = a<sup>b</sup>. But this function was a) too boring and b) not a function over a range. So he just took an array of size n namely a<sub>0</sub>, ..., a<sub>(n - 1)</sub>&nbsp;and defined the superpower of a range:</p>
<p>superpower(l, r) = pow(pow(... pow(pow(a<sub>l</sub>, a<sub>(l + 1)</sub>), a<sub>(l + 2)</sub>) ..., a<sub>(r - 1)</sub>), a<sub>r</sub>).</p>
<p>Or more formally:</p>
<p>superpower(x, x) = a<sub>x</sub></p>
<p>superpower(l, r) = pow(superpower(l, r - 1), a<sub>r</sub>)&nbsp; &nbsp; &nbsp;if l != r</p>
<p>He then suddenly realised that his problem also needs updates to be a good query-problem. So he decided to add normal updates of the form "change the number at position k to v". But while trying small values for his arrays, he realized that already the results for these small values were getting really big, so he decided he only wants them modulo m. But as Ben is not as expierienced in making problems as in not-listening to his teacher (who is btw. talking about associativity of operations for some data structures right now), he doesn't know that taking prime numbers as modulos is the normal way of doing it. So he just chooses any number m but with the restriction that it's coprime to all the numbers in his array.</p>
<p>Suddenly he realised that the problem invented by himself was too difficult for him to solve as his own solution didn't work. Help Ben!</p>
<h3>Input</h3>
<p>On the first line, there are three numbers n, q, m: the size of the array, the number of queries and the number for the modulo.</p>
<p>Then on the second line, n numbers follow: a<sub>0</sub>, a<sub>1</sub>, ..., a<sub>(n - 1)</sub>&nbsp;</p>
<p>Then each each of the next q lines consists of a char and two numbers:</p>
<p>if the char is q, then the two numbers l and r follow: Ben wants to know superpower(l, r) modulo m.</p>
<p>if the char is u, then the two numbers k and v follow: Ben wants to update a<sub>k</sub> to v.</p>
<h3>Output</h3>
<p>For each query of type q, output the superpower of the range modulo m.</p>
<h3>Constraints</h3>
<p>1 &lt;= n, q &lt;= 1e5</p>
<p>2 &lt;= m &lt;= 1e15</p>
<p>At any time, all the values in the array are &lt;= 1e9 and are coprime to m.</p>
<p>&nbsp;</p>
<h3>Edit (6.5.2020):&nbsp;</h3>
<p>I know that with m &lt;= 1e15, there may be overflows if not handled correctly. In C++ in gcc, there is the __int128 type which is essentially a 128-bit integer. The master solution uses __int128 everywhere, so you can use it without running into TLE.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 142px; width: 1px; height: 1px; overflow: hidden;">10 10 77</div>10 10 77
2 6 3 9 5 4 8 3 4 5
q 0 9
q 3 6
q 2 7
u 1 4
u 4 9
q 0 8
q 4 7
q 4 8
u 5 5
q 2 7
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 142px; width: 1px; height: 1px; overflow: hidden;">2 6 3 9 5 4 8 3 4 5</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 142px; width: 1px; height: 1px; overflow: hidden;">q 2 7</div>
<strong>Output:</strong>
1
23
1
36
64
71
1

</pre>