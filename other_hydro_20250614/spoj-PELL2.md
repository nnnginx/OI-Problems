<p>D is a given positive integer, consider the equation :<br> X² = D×Y² + 1, with X and Y positive integers.<br>
Find the minimum numbers (X,Y) within all solutions.<br>
Sometimes it's possible, sometimes not!
</p>
<p>Examples :<br>
If D=2,  3² = 2×2² + 1, so X=3 and Y=2.<br>
If D=3,  2² = 3×1² + 1, so X=2 and Y=1.<br>
If D=4, it's impossible!
</p>

<h3>Input</h3>
<p>The input begins with the number T of test cases in a single line.<br>
In each of the next T lines there is one integer D.
</p>

<h3>Output</h3>
<p>For each test case, if possible print X and Y the answer of the problem for D, else "-1".
</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
2
3
4

<b>Output:</b>
3 2
2 1
-1
</pre>

<h3>Constraints</h3>
<p>T &lt;= 1000<br>
1 &lt; D &lt;= 10^7, the numbers D were randomly chosen. (but <a href="http://www.spoj.com/problems/PELL4C/">XerK</a> modified one of them!)<br>
190 bytes of sub-optimal python code can get AC in less than 2.5 seconds, there's many rooms to make faster code.<br>
If you have TLE, you should first consider <a href="http://www.spoj.com/problems/EQU2/">EQU2</a> first.</p>
<p>Edit(2017-02-11, after compiler updates) : New TL  at 1.5s. The Python awaited solution ends under 0.8s, pike or java around 1.4s. Some old AC might not keep their AC : here it's mid-pelling. The 'mid' is to be kept in consideration.</p>