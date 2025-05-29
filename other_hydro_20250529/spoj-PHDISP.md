<p>One day, mathematician and philosopher were engaged in a heated dispute.<br><br>

Philosopher said:<br>
- Ideal line has only length and no width, therefore, no line can have an area.<br>
Mathematician replied:<br>
- That's as it may be, but still you can ll a square with a line in such a way that there will be no gaps.<br>
And you can't deny that a square has an area, and he grinned.<br>
But Philosopher still wasn't convinced:<br>
- Show me this line, then.<br>
- With pleasure... - responded Mathematician and scribbled some equations on a piece of paper:<br>
<img src="/content/turbo:img0001.jpg"><br>
- With t increasing, the point (x, y) will move around the square, forming a line.<br>
- So what? - asked Philosopher. How is it going to ll the entire square?<br>
- Indeed, it will, - said Mathematician, - Whichever point inside the square you draw, the line will eventually cross that point.<br>
- No, - replied Philosopher indignantly, - Anyway, I don't believe. When will the line cross this point? - and he put a thick dot inside the square.<br>
Give Philosopher an answer. <br>
</p>

<h3>Input</h3>
<p><i>t</i> ¨C number of tests [<i>t</i> &lt;= 150], than t test cases follows.<br>
The first line of each test case contains the coordinates (x0, y0) of the dot center (-1 &lt;= x0, y0 &lt;= 1). The second line contains eps &lt;= 0.0001 - the radius of the dot (the dot is essentially a small circle).
</p>

<h3>Output</h3>
<p>For each test case output any value of t in the segment [0, 10^12], which corresponds to the line crossing the dot, or "FAIL", if the line doesn't cross the dot.

</p><h3>Example</h3>

<pre><b>Sample input:</b>
1
0.744 0.554
0.01

<b>Sample output:</b>
5.3

</pre>