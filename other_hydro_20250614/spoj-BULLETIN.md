<p>The ACM Student Chapter has just been given custody of a number of
school bulletin boards. Several members
agreed to clear off the old posters.  They found posters
plastered many levels deep.  They made a bet about
how much area was left clear, what was the greatest depth of posters on
top of each other, and
how much of the area was covered to this greatest depth.  To
determine each bet's winner, they
made very accurate measurements of all the poster positions as they
removed them.  Because of the large number of posters, they now
need a program to do the calculations.  That is your job. </p><p>A
simple illustration is shown above:  a bulletin board 45 units
wide by 40 high, with three posters, one with corners at coordinates
(10, 10) and (35, 20), another with corners at (20, 25) and (40, 35), and the last 
with corners at (25, 5) and (30, 30).  The total area not covered
by any poster is 1300.  The maximum number of posters on top of
each other is 2.  The total area covered by exactly 2 posters
is 75.</p>


<h3>Input</h3>
<p>The input will
consist of one to twenty data
sets, followed by a line containing only 0.  On each
line the data will consist of blank separated nonnegative integers.
 </p>
<p>The first line of a dataset contains integers <span style="font-style: italic;">n w h</span>,
where <span style="font-style: italic;">n</span>
is the number of posters on the bulletin board,  <span style="font-style: italic;"></span><span style="font-style: italic;">w</span> and <span style="font-style: italic;">h</span> are the width
and height of the bulletin board<span style="font-style: italic;"></span>.  Constraints are 0 &lt; <span style="font-style: italic;">n</span> ¡Ü

100;&nbsp;0 &lt;<span style="font-style: italic;"> w</span>&nbsp;¡Ü 50000; 0 &lt; <span style="font-style: italic;">h</span> ¡Ü 40000.  </p>
<p>The dataset ends with n lines, each describing the location of
one poster.  Each poster is rectangular and has horizontal
and vertical sides.  The x and y coordinates are measured from one
corner of the bulletin board.  Each line contains four numbers  <span style="font-style: italic;">xl</span> <span style="font-style: italic;">yl</span> <span style="font-style: italic;">xh</span> and <span style="font-style: italic;">yh</span>, where <span style="font-style: italic;">xl</span> and <span style="font-style: italic;">yl</span>, are the lowest values of the x and y coordinates in one corner of the poster and <span style="font-style: italic;">xh</span> and <span style="font-style: italic;">yh</span> are the highest values in the diagonally opposite corner.  Each poster fits on the bulletin board, so 0

¡Ü <span style="font-style: italic;">xl</span>  &lt; <span style="font-style: italic;">xh</span>
¡Ü <span style="font-style: italic;">w</span>, and 0
¡Ü <span style="font-style: italic;">yl</span>  &lt; <span style="font-style: italic;">yh</span>
¡Ü <span style="font-style: italic;">h</span>.  </p>

<h3>Output</h3>
<p>There is one line of output for
each data set containing three integers, the total area of the bulletin board that is not covered by any poster, <span style="font-style: italic;"></span>the maximum depth of posters on top of each other, and <span style="font-style: italic;"></span>the total area covered this maximum number of times.  </p>Caution:  An approach examining every pair of integer coordinates might need to deal with 2 billion coordinate pairs.<br>

<h3>Example</h3>

<pre><b>Input:</b>
3 45 40
10 10 35 20
20 25 40 35
25 5 30 30
1 20 30
5 5 15 25
2 2000 1000
0 0 1000 1000
1000 0 2000 1000
3 10 10
0 0 10 10
0 0 10 10
0 0 10 10
0

<b>Output:</b>
1300 2 75
400 1 200
0 1 2000000
0 3 100

</pre>