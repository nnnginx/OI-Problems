<p>Felix, the cat, decided to play in the afternoon with some melons, he built a ¡°melon launcher¡± and started pointing to targets. Soon he noticed that the melons sometimes overflies the victims or don't even get close to them.</p>
<p>The melon launcher can be rotated so it can shoot from an angle from 0 to 45 degrees.</p>
<p>Felix isn't good at maths, so he ask you to code a program that, given the target (in meters) distance and the speed (in meters / sec) you can give him the perfect angle for the melon launcher.</p>
<p>The gravity to be considered is of 9.806 meters / sec^2</p>
<p>PI value to be considered is 2*acos(0.0).</p>

<h3>Input</h3>
<p>The first line of input will contain an integer T denoting the T test cases, then, T cases will follow. Each of the following line will contain two integer numbers Ta and Sp, denoting the distance of the target and the speed of the melon respectively.</p>

<h3>Output</h3>
<p>Output the string ¡°<tt>Scenario #i: </tt>¡° where i is the test case you are analyzing followed by a single number D, denoting the Degrees necessary to do the launch, if the launching can't be done, output D as <tt>-1</tt>. the number must have a precision of 2 decimal digits.</p>

<h3>Example</h3>
<pre><b>Input:</b>
3
10 10
10 9
8 9

<b>Output:</b>
Scenario #1: 39.35
Scenario #2: -1
Scenario #3: 37.79</pre>

<h3>Constraints</h3>
<p>0 &lt; Ta, Sp &lt; 10000</p>