<p></p><table>
<tbody>
<tr>
<td><img alt="tex2html_wrap62" src="/content/ak15:279img1.gif" align="bottom" height="449" width="585"> </td>
<td><img alt="tex2html_wrap64" src="/content/ak15:279img2.gif" align="bottom" height="402" width="190"> </td>
</tr>
</tbody>
</table>
<p>A disk can be rotated between horizontal and vertical only if it is
positioned over the
indentation marked `0' <em>and</em> the disk on its right is vertical
. The right-most
disk can always rotate if it is in position `0' since it has no disk on
its right. </p>
<p>The aim is to free the slide by moving it so its left edge aligns
with the `Win' mark: </p>
<p align="center"><img src="/content/ak15:279img3.gif"> </p>
<p>Your task is to write a program which will take several part-solved
puzzles and compute
the number of steps needed to move the slide to position `Win' for each
puzzle. </p>
<h3>Input</h3>
<p>There will be several puzzles in the input file. The first line of
the file will
contain an integer <i>n</i> specifying the number of puzzles. There
will then be <i>n</i>
lines, each of the form: </p>
<p><em>length orientations position</em> </p>
<p>where <i>length</i>(length &lt; 30) is an integer indicating the
number of disks on the
slide, <i>orientations</i> is a string of <i>length</i> characters
from the set {<tt>h</tt>,<tt>v</tt>}
giving the orientation of each disk from left to right (<tt>h</tt> stands for horizontal, and <tt>v</tt> for vertical), and <i>position</i>
is an integer
from 0 to <i>length</i> specifying the numbered mark which aligns with
the left edge of
the slide. </p>
<h3>Output</h3>
<p>For each puzzle, your program should output one integer on a line
which counts the
minimum number of steps needed to win the puzzle. A step is either a
movement of the
slide, one unit left or right, or the rotation of a disk. </p>
<h3>Example</h3>

<pre><b>Input:</b>

3
2 vv 2
7 vhhhvhh 4
29 vvvvvvvvvvvvvvvvvvvvvvvvvvvvv 29

<b>Output:</b>

7
357
1073741823
</pre>