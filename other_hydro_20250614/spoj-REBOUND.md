<p>It is well known that, in byteland, when you throw a cake, the angle of reflexion is not the angle of incidence. Measured from the ground, the angle is the double, in byteland!</p>
<p><img title="rebound" src="../../content/francky:rebound-fig2" alt="rebound"></p>
<p>You stand at point A(0, z), and you want to throw a cake in Leo's face. Leo stands at B(x, y) and is a very dangerous man, so you decide to use the ground in order to make your cake rebound.</p>
<p>Your shot is precise only if you can use an integer value t in the intervall [0, x], in order to reflect on C(t, 0). Sometimes it's possible, sometimes not!</p>
<h3>Input</h3>
<p>The input begins with the number T of test cases in a single line. In each of the next T lines there are three integers x, y and z, explaining the locations : you A(0, z), Leo B(x, y).</p>
<h3>Output</h3>
<p>For each test case, find and print the only integer t such 0 &lt;= t &lt;= x, that allow this perfect shot. If it's not possible, output "Not this time.".</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
5 4 1
6 5 2
7 3 1

<strong>Output:</strong>
2
Not this time.
3
</pre>
<p>Comment : the last case is the one illustrated above.</p>
<h3>Constraints</h3>
<pre>1 &lt; T &lt; 100 000
0 &lt; x &lt; 1 000 000 000
0 &lt; y &lt; 1 000 000 000
0 &lt; z &lt; 1 000 000 000</pre>

<p>
Edit(2017-02-11) : New time limit (after compiler changes). 
</p>