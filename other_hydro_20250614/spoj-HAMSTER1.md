<p>There is a competition of flying hamsters in Hamsterburg. Each competing hamster is thrown from a sling. The judges rate the flight according to its length and height. Let X meters be the distance of the flight, and Y meters 每 maximum height to which the hamster rose during the flight. The hamster will receive K1*X + K2*Y points for such a flight. The initial speed of the hamsters is V0 m/s. Free fall acceleration is g = 10 m/s<sup>2</sup>. There is no air friction. The size of the hamster and the sling are negligible. When the hamster is thrown from the sling its height is 0 meters. You should determine the angle at which the hamster must be thrown so that he receives maximum points.</p>

<h3>Input</h3>
<p>The first line of input contains number t 每 the amount of tests. Then  t tests follow one per line. The description of each test consists of three integers separated by single spaces. The first integer is V0, the second 每 K1, the third 每 K2.</p>

<h3>Constraints</h3>
<p>1 &lt;= t &lt;= 10000<br>
1 &lt;= V0 &lt;= 100<br>
0 &lt;= K1, K2 &lt;= 1000<br>
0 &lt; K1 + K2

</p><h3>Output</h3>
<p>For each test output the angle in radians at which the hamster must be thrown, and the amount of points it will receive. The numbers should be separated with spaces. Print the numbers with exactly three digits in the fractional part.</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
10 10 0
10 0 10
10 10 10

<b>Output:</b>
0.785 100.000
1.571 50.000
0.908 128.078
</pre>