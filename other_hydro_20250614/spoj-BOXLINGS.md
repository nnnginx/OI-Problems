<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Doctor Y, always eager to further his research in the field of boxology, is observing a family of boxen in their natural habitat ¨C a barrel of wine. He has noticed that in addition to the $N$&nbsp;($1 \leq N \leq&nbsp;200,000$) rectangular, two-dimensional boxen, there are $M$ ($1 \leq M \leq 200,000$) almost imperceptible points floating on the surface of the wine. He reasons that these must be baby boxen ¨C also known as boxlings.</p>
<p>Curious as to the customs of box families, Doctor Y wishes to count how many boxlings are floating on top of boxen. From his top-down view of the barrel, he has divided the surface of the wine into a two-dimensional Cartesian plane, and noted the positions of all the boxen and boxlings. Each box occupies a rectangular region parallel to the axes of the plane, with two of its opposite corners at coordinates ($x_1$, $y_1$) and ($x_2$, $y_2$). Doctor Y has observed that boxen sometimes overlap with one another. On the other hand, each boxling is so small that it occupies only a single point on the plane, with x-coordinate $a$ and y-coordinate $b$. All coordinates have absolute values no larger than $10^9$.</p>
<p>Having recorded the locations of all of the life forms on the surface of the wine, Doctor Y is interested in counting exactly how many boxlings are floating on top of at least one box. Note that if a boxling is on the very edge or corner of a box, it counts as being on top. Also note that two boxlings can occupy the exact same locations, in which case they should still be counted separately. It's also possible for a box to have zero area, in which case it's treated as a line (or point) and can still have boxlings on top of it.</p>
<p>With so many boxen and boxlings living in this wine barrel, Doctor Y doesn¡¯t feel like sitting there and counting them all by hand, crazy though he is. As such, he wants you to write a program to, given the locations of all the boxen and boxlings, count the number of boxlings that are floating on top of at least one box. Don¡¯t worry - your hard work will surely lead to exciting discoveries in the field of boxology.<span style="font-style: italic;">&nbsp;</span></p>
<h3>Input</h3>
<p>Line $1$: 2 integers, $N$ and $M$</p>
<p>Next $N$&nbsp;lines: 4 integers, $x_1$, $y_1$, $x_2$, and $y_2$, the coordinates of each box</p>
<p>Next $M$ lines: 2 integers, $a$ and $b$, the coordinates of each boxling</p>
<h3>Output</h3>
<p>A single integer ¨C the number of boxlings that are on top of at least one box.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">5 10</span>
<span style="font-family: 'courier new', courier;">-1 -1 2 5</span>
<span style="font-family: 'courier new', courier;">4 -3 5 3</span>
<span style="font-family: 'courier new', courier;">1 2 4 4</span>
<span style="font-family: 'courier new', courier;">5 -6 8 -4</span>
<span style="font-family: 'courier new', courier;">1 -2 8 0</span>
<span style="font-family: 'courier new', courier;">1 4</span>
<span style="font-family: 'courier new', courier;">5 4</span>
<span style="font-family: 'courier new', courier;">2 2</span>
<span style="font-family: 'courier new', courier;">3 1</span>
<span style="font-family: 'courier new', courier;">6 -5</span>
<span style="font-family: 'courier new', courier;">5 -1</span>
<span style="font-family: 'courier new', courier;">3 -3</span>
<span style="font-family: 'courier new', courier;">-1 -2</span>
<span style="font-family: 'courier new', courier;">-1 -1</span>
<span style="font-family: 'courier new', courier;">2 -1</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">6</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>Below is a top-down view of the surface of the wine:</p>
<p><img src="../../content/sourspinach:boxlings.bmp" alt="" width="275" height="325"></p>
<p>The coloured-in rectangles are the boxen, the red dots are boxlings that are on top of at least one box, and the blue dots are the other boxlings. Counting the red dots, it can be seen that there are six of them.</p>
<p>&nbsp;</p>