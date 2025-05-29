<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/FUKU11G/en/">English</a></td>
<td width="50%"><a href="/problems/FUKU11G/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p style="font-family: Times; font-size: medium;">You got an old map, which turned out to be drawn by the infamous pirate ``Captain Q". It shows the locations of a lot of treasure chests buried in an island.</p>
<p style="font-family: Times; font-size: medium;">The map is divided into square sections, each of which has a digit on it or has no digit. The digit represents the number of chests in its 9 neighboring sections (the section itself and its 8 neighbors). You may assume that there is at most one chest in each section.</p>
<p style="font-family: Times; font-size: medium;">Although you have the map, you can't determine the sections where the chests are buried. Even the total number of chests buried in the island is unknown. However, it is possible to calculate the minimum number of chests buried in the island. Your mission in this problem is to write a program that calculates it.</p>
<h3>Input</h3>
<p style="font-family: Times; font-size: medium;">The input is a sequence of datasets. Each dataset is formatted as follows.  h w  map  The first line of a dataset consists of two positive integers h and w. h is the height of the map and w is the width of the map. You may assume 1&lt;=h&lt;=15 and 1&lt;=w&lt;=15.</p>
<p style="font-family: Times; font-size: medium;">The following h lines give the map. Each line consists of w characters and corresponds to a horizontal strip of the map. Each of the characters in the line represents the state of a section as follows.</p>
<ul style="font-family: Times; font-size: medium;">
<li>'.': The section is not a part of the island (water). No chest is here. </li>
<li>'*': The section is a part of the island, and the number of chests in its 9 neighbors is not known. </li>
<li>'0' .. '9': The section is a part of the island, and the digit represents the number of chests in its 9 neighbors.</li>
</ul>
<p style="font-family: Times; font-size: medium;">You may assume that the map is not self-contradicting, i.e., there is at least one arrangement of chests. You may also assume the number of sections with digits is at least one and at most 15.  A line containing two zeros indicates the end of the input.</p>
<h3>Output</h3>
<p style="font-family: Times; font-size: medium;">For each dataset, output a line that contains the minimum number of chests. The output should not contain any other character.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre>5 6
*2.2**
..*...
..2...
..*...
*2.2**
6 5
.*2*.
..*..
..*..
..2..
..*..
.*2*.
5 6
.1111.
**...*
33....
**...0
.*2**.
6 9
....1....
...1.1...
....1....
.1..*..1.
1.1***1.1
.1..*..1.
9 9
*********
*4*4*4*4*
*********
*4*4*4*4*
*********
*4*4*4*4*
*********
*4*4*4***
*********
0 0</pre>
<strong>Output:</strong>
<pre>6
5
5
6
23</pre>
</pre>
<p> </p>