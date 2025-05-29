<p style="text-align: justify;">Somewhere in the neighborhood we have a very nice mountain that gives a splendid view over the surrounding area. There is one problem though: climbing this mountain is very difficult, because of rather large height differences. To make more people able to climb the mountain and enjoy the view, we would like to make the climb easier. To do so, we will model the mountain as follows: the mountain consists of n adjacent stacks of stones, and each of the stacks is hi high. The successive height differences are therefore h<sub>i+1</sub> − h<sub>i </sub>(for 1 &lt;=  i &lt;=  n − 1). We would like all absolute values of these height differences to be smaller than or equal to some number d.</p>
<p style="text-align: justify;"><br>We can do this by increasing or decreasing the height of some of the stacks. The first stack (the starting point) and the last stack (the ending point) should remain at the same height as they are initially. Since adding and removing stones requires a lot of effort, we would like to minimize the total number of added stones plus the total number of removed stones. What is this minimum number?</p>
<h3>Input</h3>
<p style="text-align: justify;">On the first line one positive number: the number of testcases, at most 100. After that per testcase:</p>
<ul style="text-align: justify;">
<li>One line with two integers n (2 &lt;= n &lt;= 100) and d (0  &lt;= d &lt;= 10^9): the number of stacks of stones and the maximum allowed height difference.</li>
<li style="text-align: justify;">One line with n integers hi (0 &lt;= h<sub>i </sub>&lt;= 10^9): the heights of the stacks.</li>
</ul>
<p style="text-align: justify;">&nbsp;</p>
<h3 style="text-align: justify;">Output</h3>
<p style="text-align: justify;">Per testcase:<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; One line with the minimum number of stones that have to be added or removed or “impossible” if it is impossible to achieve the goal.</p>
<p style="text-align: justify;">&nbsp;</p>
<h3 style="text-align: justify;">Example</h3>
<pre style="text-align: justify;"><strong>Input:</strong><br>3<br>10 2<br>4 5 10 6 6 9 4 7 9 8<br>3 1<br>6 4 0<br>4 2<br>3 0 6 3<br><br><strong>Output:</strong><br>6<br>impossible<br>4<br></pre>
<div id="_mcePaste" style="overflow: hidden; position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; text-align: justify;">Problem text...</div>
<p>&nbsp;</p>
<div id="_mcePaste" style="overflow: hidden; position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; text-align: justify;">Problem text...</div>