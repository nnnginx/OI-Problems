<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MCONVOI/en/">English</a></td>
<td width="50%"><a href="/problems/MCONVOI/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<pre>An  elephant  lives by  a  lake with N plants on  the  surface. The  lake  <br>can be modeled by  a  coordinate plane, with plants at points with <br>integer coordinates. <br>Every morning  after waking  up,  the  elephant  performs  his <br>morning  exercise,  happily  jumping  from plant  to plant. For  <br>reasons best  left undiscussed,  the elephant can always jump only  to <br>another plant with both coordinates larger than the coordinates of<br>the plant it is currently on. In other words, from plant (x1, y1) the <br>elephant can jump to plant (x2, y2) only if x2 &gt; x1 and y2 &gt; y1. <br>The elephant can start his exercise at any plant on the lake. <br>Write a program that, given the coordinates of all plants, calculates<br>the length of the longest sequence of  plants  the  elephant  can  visit.  <br>Additionally,  calculate  the  number  of  different  such  longest <br>sequences. Because this second number can be large, calculate it <br>modulo 1 000 000 007.  <br></pre>
<h3>Input</h3>
<pre>The first line contains the integer N (1 ¡Ü N ¡Ü 300 000), the number of plants. <br>Each of the following N  lines contains the coordinates of one plant, <br>two  integers between 0 and 10^9.<br>No two plants will have the same pair of coordinates. <br></pre>
<h3>Output</h3>
<pre>On the first line output the length of the longest sequence of plants<br>the elephant can jump on. <br>On the second line output the number of such sequences of maximum length, <br>modulo 1 000 000  007. <br></pre>
<h3>Sample</h3>
<pre>Sample input<br>input <br>11 <br>8 6 <br>7 4 <br>5 4 <br>5 1 <br>5 6 <br>6 2 <br>3 2 <br>4 3 <br>4 5 <br>3 5 <br>2 4 <br>output <br>4 <br>3 <br><br>input <br>6 <br>1 3 <br>2 2 <br>3 1 <br>5 3 <br>4 4 <br>3 5 <br>output <br>2 <br>7 <br></pre>
<p> </p>