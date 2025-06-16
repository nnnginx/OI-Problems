<p><em>Original statement in spanish at <a href="http://www.dc.uba.ar/events/icpc/download/problems/taip2011-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/taip2011-problems.pdf</a></em></p>
<p>The International Canvas Preparation Committee (ICPC) has a peculiar procedure for setting up its canvases. The procedure depends on a bidimensional view of the canvases.</p>
<p>A given canvas is set up using <strong>N</strong> poles of different heights. To set up the canvases, the ICPC uses the following procedure. First, <strong>N+2</strong> points are marked on the floor, all on the same line, so that two consecutive points are always separated by a distance of exactly two feet. Afterwards, a pole is placed vertically over each of the <strong>N</strong> central points. Finally, the canvas is extended over the poles, joining the upper end of each pole with the upper end of neighboring poles. The first and last poles are joined with the free points on the floor.</p>
<p>The next figure shows 3 possible ways of setting up a canvas using the instructions mentioned before, with pole heights of 4, 5, 7, 8 and 9.</p>
<p><img src="../../../content/pabloh:taip2011A.png" alt=""></p>
<p>After years of hard work, the ICPC came to the conclusion that in order to obtain useful and sturdy canvases, it is necessary that the angle formed by two consecutive patches of canvas at the end of a pole, measured towards the inside, is <em>strictly</em> less than 180 degrees. In the figure shown, only the canvas on the left satisfies this condition. The canvas in the middle has an angle greater than 180 degrees at poles of heights 4 and 7, while the canvas on the right has an angle of exactly 180 degrees at the pole of height 8. We say a canvas is valid when it adheres to the ICPC recommendation.</p>
<p>Of course, given the number of poles and their heights, there are a lot of different ways of placing them, some of which will produce valid canvases and some of which will not. The task at hand is to, given this data, count the number of different valid canvases which can be set up. Two valid canvases are considered different if the sequence of heights of the poles in one of them, read from left to right, is different from the sequence of heights of the other one, read in the same way.</p>
<h3>Input</h3>
<p>The input contains several test cases. Each test case is described on two consecutive lines. The first line contains one integer <strong>N</strong> which indicates the number of poles (1 &lt;= <strong>N</strong> &lt;= 60). The second line contains <strong>N</strong> integers <strong>H_i</strong> representing the heights of the poles in feet (1 &lt;= <strong>H_i</strong> &lt;= 10<sup>9</sup> for 1 &lt;= <strong>i</strong> &lt;= <strong>N</strong>). The last line of the input contains a single -1 and should not be processed as a test case.</p>
<h3>Output</h3>
<p>For each test case output a single line with an integer representing the number of different valid canvases which can be set up using the given poles.</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>5
4 5 7 8 9
7
33 65 57 64 63 61 49
1
1000000000
3
2 2 3
3
1 3 1
4
2 2 2 2
-1
</pre>
<p><strong>Output:</strong></p>
<pre>2
16
1
1
0
0
</pre>