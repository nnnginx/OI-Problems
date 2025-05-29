<div align="justify">
<p>
Farmer john owns a single cow and he loves it a lot. The cow has a disease and is going to die. To survive, the cow needs medicine of a particular type each day. Let us say the cow needs <b>medicine</b>[i] to survive the i<sup>th</sup> day. (medicine[i] will be terminated by -1, which is an unavailable medicine, and the cow has to invariably die that day). <br>
To help the cow, john has decided to buy pastures of some medical value. Farmer sees a two-dimensional grid of pastures, each cell having exactly one medical herb. Now he needs to buy a sub-rectangular region of the grid, whose area cannot exceed <b>A</b> (<b>A</b> &gt; 1). With this region the farmer intends to feed his cow, as long as possible.
</p>
<br>
<b>Input Format:</b><br>
The input file consists of multiple testcases. <br>
The first line of each testcase contains three integers, <b>R</b>, <b>C</b> and <b>A</b>.<br>
The second line consists of sequence of integers describing <b>medicine</b>[i]. This list will be terminated by -1.<br>
The next <b>R</b> lines contain <b>C</b> integers each, specifying the medicinal type of the herb in that cell. (1 &lt;= <b>R,C</b> &lt;= 200). All herbs are specified by non negative integers.<br>
Input terminates with a line containing three zeros and must not be processed.<br>
<br>
<b>Output Format:</b><br>
For each testcase print a single line containing 5 integers: <br>
<i><b>days r1 c1 r2 c2</b></i><br>
(1 &lt;= r1 &lt;= r2 &lt;= R, 1 &lt;= c1 &lt;= c2 &lt;= C)<br>
<ul>
<li><b><i>days</i></b> is the number of days the cow survives. We wish to maximise this.
</li><li>If there are more than one solutions print the one with minimal r1.
</li><li>If there are more than one solutions still, print the one with minimal c1.
</li><li>If there are more than one solutions still, print the one with minimal r2.
</li><li>If there are more than one solutions still, print the one with minimal c2.
</li></ul>
<br>
<b>Sample Input:</b><br>
<pre>3 4 6
12 30 12 100 22 -1
30 12 5 3
12 30 100 5
22 3 22 100
3 4 6
2 30 12 100 22 -1
30 12 5 3
12 30 100 5
22 3 22 100
3 4 6
12 30 12 100 22 -1
30 12 5 3
12 30 100 5
22 12 22 100
0 0 0
</pre>

<b>Sample Output:</b><br>
<pre>4 1 1 2 3
0 1 1 1 1
5 1 2 3 3
</pre>
</div>