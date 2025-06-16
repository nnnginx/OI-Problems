<p>Let's play a puzzle using eight cubes placed on a  <span>3 <tt>x</tt> 3</span> board leaving one empty square.</p>
<p>Faces of cubes are painted with three colors.  As a puzzle step, you can roll one of the cubes to the adjacent empty square.  Your goal is to make the specified color pattern visible from above by a number of such steps.</p>
<p>The rules of this puzzle are as follows.</p>
<p>&nbsp;</p>
<ol>
<li><strong>Coloring of Cubes:</strong> All the cubes are colored in the same way  as shown in Figure 3. The opposite faces have the same color.
<p>&nbsp;</p>
<div><img src="/content/zukow:YOKOC_1.png" border="0" alt="\epsfbox{p3618a.eps}" width="206" height="178" align="BOTTOM"></div>
<p>&nbsp;</p>
<div>Figure 3: Coloring of a cube</div>
<p>&nbsp;</p>
</li>
<li><strong>Initial Board State:</strong> Eight cubes are placed on the  <span>3 <tt>x</tt> 3</span> board leaving one empty square.  All the cubes have the same orientation as shown in Figure 4.  As shown in the figure, squares on the board are given <span><em>x</em></span> and <span><em>y</em></span> coordinates, (1, 1), (1, 2), ..., and (3, 3). The position of the initially empty square may vary.
<p>&nbsp;</p>
<div><img src="/content/zukow:YOKOC_2.png" border="0" alt="\epsfbox{p3618b.eps}" width="452" height="228" align="BOTTOM"></div>
<p>&nbsp;</p>
<div>Figure 4: Initial board state</div>
<p>&nbsp;</p>
</li>
<li><strong>Rolling Cubes:</strong> At each step, we can choose one of the cubes adjacent to the empty square and roll it into the empty square, leaving the original position empty.  Figure 5 shows an example.
<p>&nbsp;</p>
<div><img src="/content/zukow:YOKOC_3.png" border="0" alt="\epsfbox{p3618c.eps}" width="548" height="162" align="BOTTOM"></div>
<p>&nbsp;</p>
<div>Figure 5: Rolling a cube</div>
<p>&nbsp;</p>
</li>
<li><strong>Goal:</strong> The goal of this puzzle is to arrange the cubes so that their top faces form the specified color pattern by a number of cube rolling steps described above. </li>
</ol>
<p>Your task is to write a program that finds the minimum number of steps required to make the specified color pattern from the given initial state.</p>
<p>&nbsp;</p>
<h2><span style="color: #ff0000; font-size: medium;"><a name="SECTION0001001000000000000000"></a></span></h2>
<h3>Input</h3>
<p>The input is a sequence of datasets.  The end of the input is indicated by a line containing two zeros separated by a space.  The number of datasets is less than 16.  Each dataset is formatted as follows.</p>
<blockquote><span> 
<table border="0">
<tbody>
<tr>
<td align="LEFT" valign="BASELINE"><em>x</em></td>
<td align="LEFT" valign="BASELINE"><em>y</em></td>
<td align="LEFT" valign="BASELINE">&nbsp;</td>
</tr>
<tr>
<td align="LEFT" valign="BASELINE"><em>F</em><sub>11</sub></td>
<td align="LEFT" valign="BASELINE"><em>F</em><sub>21</sub></td>
<td align="LEFT" valign="BASELINE"><em>F</em><sub>31</sub></td>
</tr>
<tr>
<td align="LEFT" valign="BASELINE"><em>F</em><sub>12</sub></td>
<td align="LEFT" valign="BASELINE"><em>F</em><sub>22</sub></td>
<td align="LEFT" valign="BASELINE"><em>F</em><sub>32</sub></td>
</tr>
<tr>
<td align="LEFT" valign="BASELINE"><em>F</em><sub>13</sub></td>
<td align="LEFT" valign="BASELINE"><em>F</em><sub>23</sub></td>
<td align="LEFT" valign="BASELINE"><em>F</em><sub>33</sub></td>
</tr>
</tbody>
</table>
</span></blockquote>
<p>The first line contains two integers <span><em>x</em></span> and <span><em>y</em></span> separated by a space, indicating the position <span>(<em>x</em>, <em>y</em>)</span> of the initially empty square. The values of <span><em>x</em></span> and <span><em>y</em></span> are 1, 2, or 3.</p>
<p>The following three lines specify the color pattern to make.  Each line contains three characters  <span><em>F</em><sub>1j</sub>, <em>F</em><sub>2j</sub>,</span> and <span><em>F</em><sub>3j</sub></span>, separated by a space.  Character <span><em>F</em><sub>ij</sub></span> indicates the top color of the cube, if any, at position <span>(<em>i</em>, <em>j</em>)</span> as follows:</p>
<dl><dt><tt>B</tt>: Blue, </dt><dt><tt>W</tt>: White, </dt><dt><tt>R</tt>: Red, </dt><dt><tt>E</tt>: the square is Empty. </dt></dl>
<p>There is exactly one `<tt>E</tt>' character in each dataset.</p>
<h3>Output</h3>
<p>For each dataset, output the minimum number of steps to achieve the goal, when the goal can be reached within 30 steps. Otherwise, output ``<tt>-1</tt>'' for the dataset.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>&nbsp;<pre>1 2 
W W W 
E W W 
W W W 
2 1 
R B W 
R W W 
E W W 
3 3 
W B W 
B R E 
R B R 
3 3 
B W R 
B W R 
B E R 
2 1 
B B B 
B R B 
B R E 
1 1 
R R R 
W W W 
R R E 
2 1 
R R R 
B W B 
R R E 
3 2 
R R R 
W E W 
R R R
0 0
</pre>
<strong>Output:</strong>&nbsp;
<pre>0 
3 
13 
23 
29 
30 
-1 
-1
</pre>
</pre>