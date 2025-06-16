<p>Ada the Ladybug was on a trip with her friends. They each bought a souvenir there. As all of them are mathematicians, everybody bought a number. They want to modify the numbers to have some connection between each other. They have decided to modify the numbers sou they would have their <strong>GCD</strong> greater than 1 ( <strong>gcd(a<sub>1</sub>,a<sub>2</sub>,a<sub>3</sub>,...,a<sub>N</sub>)&gt;1</strong>). Anyway it is not easy to change a number - the only thing they can do is to go to a proffesor in mathematics, which could forge a number <strong>A</strong> into number <strong>A+1</strong> or <strong>A-1</strong>. As this operation is not cheap, they want to minimize number of such operations. A number might be forged any number of times.</p>
<p>NOTE: <strong>gcd(a,0)==a</strong> (so gcd of two 0 is also 0)</p>
<h3>Input</h3>
<p>The first line contains an integer <strong> 1 ¡Ü N ¡Ü 3*10<sup>5</sup></strong>, the number of friend who were on trip (and also the number of numbers).</p>
<p>The second line contains <strong>N</strong> integers <strong>0 ¡Ü a<sub>i</sub> ¡Ü     10<sup>6</sup></strong></p>
<h3>Output</h3>
<p>Print a single line with minimum number of operations to make a connection between all numbers.</p>
<h3>Example Input</h3>
<pre>5
3 9 7 6 31
</pre>
<h3>Example Output</h3>
<pre>2
</pre>
<h3>Example Input 2</h3>
<pre>9
3 4 5 7 8 9 11 12 13
</pre>
<h3>Example Output 2</h3>
<pre>6
</pre>
<h3>Example Input 3</h3>
<pre>5
7 7 11 17 1
</pre>
<h3>Example Output 3</h3>
<pre>5
</pre>