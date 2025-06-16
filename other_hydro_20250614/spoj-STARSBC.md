<p>Fernando won a compass for his birthday, and now his favorite hobby is drawing stars: ﬁrst, he marks <strong>N</strong> points on a circumference, dividing it into <strong>N</strong> equal arcs; then, he connects each point to the <em>k-th</em> next point, until returning to the ﬁrst point.<br> <br> Depending on the value of <em>k</em>, Fernando may or may not reach all  points marked on the circumference; when that happens, the star is  called complete. For example, when <strong>N</strong> = 8, the possible stars are shown in the ﬁgure below. Stars (a) and (c) are complete,  	while stars (b) and (d) are not.</p>
<p><img src="../../../content/simes:Starsbc.png" alt="Stars for N=8 and k in {1-4}"></p>
<p>&nbsp;</p>
<p>Depending on the value of <strong>N</strong>, it may be possible to draw many diﬀerent stars; Fernando asked you to write a program that, given <strong>N</strong>, determines the number of complete stars he can draw.</p>
<h3>Input</h3>
<p>The input contains several test cases. Each test case contains a single line, containing a single integer&nbsp;<strong>N</strong>&nbsp;(3 ≤&nbsp;<strong>N</strong>&nbsp;&lt; 2<sup>31</sup>),&nbsp;indicating the number of arcs in which the circumference was divided.</p>
<h3>Output</h3>
<p>For each test case, your program must print a single line containing a  single integer, indicating the number of complete stars that can be  drawn.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>4<br>5<br>18<br>36<br>360<br>2147483647

<strong>Output:</strong>
1<br>1<br>2<br>3<br>6<br>48<br>1073741823
</pre>