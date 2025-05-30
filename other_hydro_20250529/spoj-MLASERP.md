<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MLASERP/en/">English</a></td> 
<td width="50%"><a href="/problems/MLASERP/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<pre>The cows have a new laser-based system so they can have casual
conversations while out in the pasture which is modeled as a W x H
grid of points (1 &lt;= W &lt;= 100; 1 &lt;= H &lt;= 100).

The system requires a sort of line-of-sight connectivity in order
to sustain communication. The pasture, of course, has rocks and
trees that disrupt the communication but the cows have purchased
diagonal mirrors ('/' and '\' below) that deflect the laser beam
through a 90 degree turn. Below is a map that illustrates the
problem.

H is 8 and W is 7 for this map.  The two communicating cows are
notated as 'C's; rocks and other blocking elements are notated as
'*'s:

7 . . . . . . .         7 . . . . . . .
6 . . . . . . C         6 . . . . . /-C
5 . . . . . . *         5 . . . . . | *
4 * * * * * . *         4 * * * * * | *
3 . . . . * . .         3 . . . . * | .
2 . . . . * . .         2 . . . . * | .
1 . C . . * . .         1 . C . . * | .
0 . . . . . . .         0 . \-------/ .
  0 1 2 3 4 5 6           0 1 2 3 4 5 6

Determine the minimum number of mirrors M that must be installed
to maintain laser communication between the two cows, a feat which
is always possible in the given test data.

</pre>

<cen><h3>INPUT</h3></cen>
<pre>* Line 1: Two space separated integers: W and H

* Lines 2..H+1: The entire pasture.

SAMPLE INPUT  

7 8
.......
......C
......*
*****.*
....*..
....*..
.C..*..
.......
</pre>
<b>OUTPUT </b>
<pre>* Line 1: A single integer: M

SAMPLE OUTPUT 

3
</pre>
 <b>Any suggestted testcase will be welcomed.</b>