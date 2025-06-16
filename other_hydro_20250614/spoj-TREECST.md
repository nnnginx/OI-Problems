<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/

TREECST/en/">English</a></td>
<td width="50%"><a href="/problems/

TREECST/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Moles are tidy and hard-working animals. Our mole likes to   keep its underground residence in utmost order, so that everyone living there knows where to find   things.</p>
<p>To achieve this, the mole connected rooms with tunnels so   that there is a single unique way to get from one room to any other room. The distance between two rooms   is the number of halls passed on the way from one to the other.</p>
<p>Despite all the effort, some of the mole's guests are   complaining that it takes too long to walk between certain pairs of rooms.</p>
<p>The mole decided to reconstruct her residence, closing   one tunnel and opening a new one, so that the distance between the farthest two rooms is the smallest   possible, but so that it is still possible to reach every room from every other room.</p>
<p>Write a program which determines the distance between   the farthest two rooms after reconstruction, which tunnel to close and which to open.</p>
<h3>Input</h3>
<p>The first line contains an integer N (1 ≤ N ≤ 300 000), the   number of rooms. The rooms are numbered 1 to N.</p>
<p>Each of the next N−1 lines contains two integers, the   numbers of rooms a tunnel connects.</p>
<h3>Output</h3>
<p>Output on separate lines, in order:</p>
<ul>
<li>The distance between the two farthest rooms after   reconstruction.</li>
<li>A pair of integers representing a previously existing tunnel,   which should be closed.</li>
<li>A pair of integers, the rooms between which a new tunnel   should be opened.</li>
</ul>
<p>Note: The solution will not necessarily be unique. Output   any reconstruction plan which achieves the smallest distance between the farthest two rooms.</p>
<h3>Example</h3>
<pre><strong>Input</strong>
4
1 2
2 3
3 4

<strong>Output</strong>
2
3 4
4 2

<strong>Input</strong>
7
1 3
2 3
2 7
4 3
7 5
3 6

<strong>Output</strong>
3
2 3
7 3

</pre>
<p> </p>