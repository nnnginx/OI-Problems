<p>
Lucky is fond of Number theory,
 one day he was solving a problem related to Euler Totient Function (phi) and
 found an interesting property of phi :
 phi(1) = 1, and for x &gt; 1: phi(x) &lt; x.<br>

 So if we define a sequence with a<sub>0</sub> = x, and for n &gt; 0: a<sub>n</sub> = phi(a<sub>n-1</sub>), this sequence will be constant equal to 1 starting from some point. Lets define depth(x) as minimal n such that a<sub>n</sub> = 1.&nbsp;<br>

 Now he is wondering how many numbers in a given range have depth equal to given number <strong>k</strong>.
 As you are a good programmer help Lucky with his task.
</p>


<h3>Input</h3>
<p>Your input will consist of a single integer&nbsp;<strong>T</strong>
&nbsp;followed by a newline and&nbsp;<strong>T</strong>&nbsp;test cases.<br>

 Each test cases consists of a single line containing integers 
<strong>m</strong>, <strong>n</strong>, and <strong>k</strong>.
</p>

<h3>Output</h3>
<p>
Output for each test case one line containing the count of all numbers whose depth equals to <strong>k</strong> in given range [<strong>m</strong>, <strong>n</strong>].</p>

<h3>Constraints</h3>
<pre>T &lt; 10001
1 ¡Ü m ¡Ü n ¡Ü 10^6
0 ¡Ü k &lt; 20
</pre>


<h3>Example</h3>
<pre><strong>Input:</strong>
5
1 3 1
1 10 2
1 10 3
1 100 3
1 1000000 17

<strong>Output:</strong>
1
3
5
8
287876</pre>

<p>Explanation ::suppose number is 5 ; its depth will be 3. ( 5 -&gt; 4 -&gt; 2 -&gt; 1 )</p>
<p>Note ::Depth for 1 is 0.</p>