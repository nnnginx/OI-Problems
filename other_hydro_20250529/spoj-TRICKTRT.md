<p>Johnny and his friends have decided to spend Halloween night doing the usual candy collection from the households of their village. As the village is too big for a single group to collect the candy from all houses sequentially, Johnny and his friends have decided to split up so that each of them goes to a different house, collects the candy (or wreaks havoc if the residents don’t give out candy), and returns to a meeting point arranged in advance.</p>
<p>There are <em>n</em> houses in the village, the positions of which can be identified with their Cartesian coordinates on the Euclidean plane. Johnny’s gang is also made up of <em>n</em> people (including Johnny himself). They have decided to distribute the candy after everybody comes back with their booty. The houses might be far away, but Johnny’s interest is in eating the candy as soon as possible.</p>
<p>Keeping in mind that, because of their response to the hospitality of some villagers, some children might be wanted by the local authorities, they have agreed to fix the meeting point by the river running through the village, which is the line <em>y</em> = 0. Note that there may be houses on both sides of the river, and some of the houses may be houseboats (<em>y</em> = 0). The walking speed of every child is 1 meter per second, and they can move along any direction on the plane.</p>
<p>At exactly midnight, each child will knock on the door of the house he has chosen, collect the candy instantaneously, and walk back along the shortest route to the meeting point. Tell Johnny at what time he will be able to start eating the candy.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>Each test case starts with a line indicating the number <em>n</em> of houses (1 ≤ <em>n</em> ≤ 50&nbsp;000). The next <em>n</em> lines describe the positions of the houses; each of these lines contains two floating point numbers <em>x</em> and <em>y</em> (−200&nbsp;000 ≤ <em>x</em>, <em>y</em> ≤ 200&nbsp;000), the coordinates of a house in meters. All houses are at different positions.</p>
<p>A blank line follows each case. A line with <em>n</em> = 0 indicates the end of the input; do not write any output for this case.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>For each test case, print two numbers in a line separated by a space: the coordinate <em>x</em> of the meeting point on the line <em>y</em> = 0 that minimizes the time the last child arrives, and this time itself (measured in seconds after midnight). Your answer should be accurate to within an absolute or relative error of 10<sup>−5</sup>.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">2
1.5 1.5
3 0

1
0 0

4
1 4
4 4
-3 3
2 4

5
4 7
-4 0
7 -6
-2 4
8 -5

0
</pre>
</div>
<p><br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">1.500000000 1.500000000
0.000000000 0.000000000
1.000000000 5.000000000
3.136363636 7.136363636
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Javier Gómez Serrano</em></blockquote>