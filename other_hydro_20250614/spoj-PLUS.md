<p>A man called Gerit Teeman was fascinated by the plus symbol and, to be honest, this symbol is actually quite interesting!</p>

<p>Begin by drawing an one. This will be the center of the plus symbol. Above this center draw the number two, below three, to the left four and the the right five. If you then 'replace' the center (either up, down, left or right), do the same, but when a place is already filled you leave it untouched.</p>

<p>To illustrate this we pick the place with the number two: Above it draw a two, the bottom is already filled so we leave it untouched, to the left we draw a four and the the right we draw a five. See the picture below:<br><img style="vertical-align: middle;" title="example 1" src="/content/zukow:plusex1.png" alt="example" width="597" height="167"></p>

<p>It is not hard to see that the sum of the first plus symbol is 15 (the first symbol only containing 1 is NOT a plus symbol). The sum of the second symbol is already more difficult, summing up to 26. Now here comes the catch: depending on which number you pick to expand on, the number on positions can change. If we would have picked five to expand on instead of two, we will get the following:<br><img style="vertical-align: middle;" title="example 2" src="/content/zukow:plusex2.png" alt="example" width="610" height="144"></p>

<p>As you can see the numbers differ from that of the first example. This time the sum is 25! On top of that, there can be multiple 'replaces', generating more number in the symbol. Your task is, depending on which way you expand to, give the sum of all the elements of plus symbol that you would obtain.</p>
<br>

<h1>Input
<p>First line contains an integer T (1 &lt;= T &lt;= 100) number of test cases. Each of the next T lines contains a string with letters 'L', 'R', 'U', 'D' and 'S' (separated by commas) which respectively mean left, right, up, down and stop. You should expand to the given direction, based on your last created expansion's center. Stop means you should finish and output the total sum to that point. The number of letters in the string will never exceed 10000.</p>
<p>Note that the first example was created by the string "U,S" and the second by the string "R,S".</p>
<br>

</h1><h1>Output
<p>For each test case output a single integer in a separate line: the total sum of all numbers contained in the created symbol.</p>
<br>

</h1><h1>Sample:</h1>
<pre><b>Input:</b>
2
U,S
S

<b>Output:</b>
26
15
</pre>