<p>There is a building with flat square roof of size <i>3<sup>k</sup>*3</i><sup><i>k</i> </sup>and sides parallel to north-south and east-west directions. The
roof is covered with square tiles of size <i>1 </i>(with a side of length 1), but one of the tiles has been
removed and there is a hole in the roof (big enough to fall in). The tiles form a
rectangular mesh on the roof, so their positions may be specified with
coordinates. The tile at the southwestern corner has coordinates (<i>1,1</i>). The
first coordinate increases while going eastwards, and the second while going
northwards.
</p>

<p>Sleepwalker wanders across the roof, in each step moving from the tile he is
standing on to the adjacent one on the east(E), west(W), south(S), or 
north(N). The
sleepwalker roof ramble starts from the southwestern corner tile. The
description of the path is a word d<sub><i>k</i></sub>   built of the letters <tt>N, S, E, W
</tt>denoting respectively a step to the north, south, east and west. For <i> k = 1</i>
the word describing the path of sleepwalker is
</p>

<p>
d<sub>1</sub> = <tt>EENNWSWN</tt>
</p>

<p>For <i> k = 2</i> the word describing the path of sleepwalker is
</p><p>
</p><table>
<tbody><tr valign="top">
<td>d<sub>2</sub></td>
<td>=</td>
<td>
<tt>NNEESWSEENNEESWSEEEENNWSWNNEENNWSW -<br>
NNEENNWSWNWWWSSENESSSSWWNENWWSSW  -<br> 
WNENWNEENNWSWN.</tt></td>
</tr>
</tbody></table>
<p></p><p>(See the picture that shows how the sleepwalker would go across a roof of
dimension <i> 3*3</i> or <i>9*9</i>.) Generally, if <i>k&gt;=1</i>, the description of
a sleepwalker's path on the roof of dimension 
<i>3<sup>k+1</sup>*3<sup>k+1</sup>
</i>
is a word:
</p><p>d<sub>k+1</sub> =  a(d<sub>k</sub>) E a(d<sub>k</sub>) E d<sub>k</sub> N d <sub>k</sub> N d<sub>k</sub> W c(d<sub>k</sub>) S
b(d<sub>k</sub>) W b(d<sub>k</sub>) N d<sub>k</sub></p>where functions <b>a</b>,
<b> b</b>
and <b> c</b> denote the following permutations of letters specifying directions:

<pre>a: E-&gt;N W-&gt;S N-&gt;E S-&gt;W 
b: E-&gt;S W-&gt;N N-&gt;W S-&gt;E 
c: E-&gt;W W-&gt;E N-&gt;S S-&gt;N 
</pre>

<p>E.g. a(SEN)=WNE, b(SEN)=ESW, c(SEN)=NWS.
</p>

<p>We start observing sleepwalker at the time he stands on the tile of coordinates
(<i>u<sub>1</sub>, u<sub>2</sub></i>). After how many steps will sleepwalker fall into the hole made
after removing the tile of coordinates (<i>v<sub>1</sub>, v<sub>2</sub></i>)? 
</p>

<h3>Example</h3>

<p>There are sleepwalker's paths on roofs of dimension <i> 3*3</i> and <i> 9*9</i> on the
picture below. In the second case, the point at which the observation starts and the hole have
been marked. The sleepwalker has exactly <i> 20</i> steps to the hole (from the
moment the observation starts).
</p>

<center>
<table>
<tbody><tr valign="bottom">
<td><img src="/content/piotrek:lunatyk1.gif" padding="20" height="83" width="81"></td>
<td><img src="/content/piotrek:lunatyk2.gif" padding="20" height="206" width="204"></td>
</tr>
</tbody></table>
</center>

<h3>Task</h3> 

<p>
Write a program which:
</p><ul>
<li>reads from the standard input integer <i>k</i> denoting the size of the roof (<i>3<sup>k</sup>*3<sup>k</sup></i>),
  the position of the sleepwalker at the moment the observation starts and the position
  of the hole,
</li><li>computes the number of steps that the sleepwalker will make before he falls into the
  hole,
</li><li>writes the result to the standard output.
</li></ul> 

<h3>Input</h3>

<p>
The number of test cases t is in the first line of input, then t test cases follow separated by an empty line.
In the first line of each test case one integer <i>k</i>,
<i>
1&lt;=k&lt;=60</i>, denoting the size of the roof (<i>3<sup>k</sup>*3<sup>k</sup></i>) is written. In
each of the following two lines of the test case  two natural
numbers <i> x, y</i> separated with a space are written, <i> 1&lt;=x&lt;=3^k</i>, <i> 1&lt;=y&lt;=3^k</i>. The
numbers in the second line are the coordinates of the tile the sleepwalker is
standing on. The numbers in the third line are the coordinates of the hole. You
may assume, that with these data the sleepwalker will eventually fall into the hole
after some number of steps.
</p>

<h3>Output</h3>

<p>The only line of output for each test case should contain the number of steps on
the sleepwalker's path to the hole.
</p>

<h3>Example</h3>
<pre><b>Sample input:</b>
1
2
3 2
7 2

<b>Sample output</b>
20
</pre>