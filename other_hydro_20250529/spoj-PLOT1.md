<p>Given a function y=f(x) in RPN-notation plot it with stars (*) and then (!) its derivation with crosses (+)&nbsp;for 0&lt;=x&lt;=20 with ¦¤x=1 in a diagram with 21*21 points (0&lt;=x,y&lt;=20). Empty fields are marked with dots (.). For plotting the real number y should be rounded to integer (-0.5 -&gt; -1, -0.4 -&gt; 0, 0.4 -&gt; 0, 0.5 -&gt; 1). The function and its derivation are continuous between 0 and 20.<br>The function definition uses only the following characters: 0123456789x.+-*/^<br>'^' means 'power of'. Items are separated by space.</p>
<h3>Input</h3>
<p>In the first line the number N of functions, then N lines with one function.</p>
<h3>Output</h3>
<p>The plot of each function and its derivation&nbsp;in 21 lines.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1<br>x 1 -

<strong>Output:</strong>
.....................<br>....................*<br>...................*.<br>..................*..<br>.................*...<br>................*....<br>...............*.....<br>..............*......<br>.............*.......<br>............*........<br>...........*.........<br>..........*..........<br>.........*...........<br>........*............<br>.......*.............<br>......*..............<br>.....*...............<br>....*................<br>...*.................<br>+++++++++++++++++++++<br>.*...................<br></pre>