<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/PK11I/en/">English</a></td>
<td width="50%"><a href="/problems/PK11I/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<div>
<p><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">You are given a tree (a connected graph with no cycles), and the edges of the tree which are for some reason directed; your task is to add </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">minimum </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">number of special paths in the tree such that it's possible to go from any node to another. The rules for the special paths are noted below: </span></p>
<ol style="list-style-type: decimal;">
<li style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">
<p><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">A special path consists of some continuous edges (from the tree) and nodes. </span></p>
</li>
<li style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">
<p><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">In a special path, the edges should be in opposite directions as they are in the tree. </span></p>
</li>
<li style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">
<p><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">A node or an edge can be visited at most once in a special path. </span></p>
</li>
<li style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">
<p><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">Multiple special paths may have common nodes or edges.&nbsp;</span></p>
</li>
</ol></div>
<p><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">For example, in the picture below, a tree is drawn, the black arrows represent the edges and their directions, circles represent nodes. Then we need two special paths. One path is </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">2-1-0 </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">(green arrow), another is </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">3-1 </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">(blue arrow). Instead of the path </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">3-1 </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">we can add </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">3-1-0. </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">You cannot add a path like </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">1-3 </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">or </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">0-1-2 </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">because of rule 2. You cannot add </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">0-2 </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">or </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">2-3-0 </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">because of rule 1.&nbsp;</span></p>
<p>&nbsp;</p>
<p style="text-align: center;"><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';"><img src="file://74d80Hpf.png" alt="" width="118" height="123"></span></p>
<p>&nbsp;</p>
<div>
<p><span style="font-size: 14.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">Input<br> </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">Input starts with an integer </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">T (¡Ü 30), </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">denoting the number of test cases. </span></p>
<p><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">Each case starts with a line containing an integer </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">N (2 </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">¡Ü </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">N </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">¡Ü </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">20000), </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">where </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">N </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">denotes the number of nodes. The nodes are numbered from </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">0 </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">to </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">N-1. </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">Each of the next </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">N-1 </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">lines contains two integers </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">u v (0 </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">¡Ü </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">u, v &lt; N, u </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">¡Ù </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">v) </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">meaning that there is an edge from </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">u </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">to </span><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">v.&nbsp;</span></p>
</div>
<div>
<p><span style="font-size: 14.000000pt; font-family: 'TimesNewRomanPS'; font-weight: 700;">Output </span></p>
<p><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">For each case, print the case number and the minimum number of special paths required such that it's possible to go from any node to another.&nbsp;</span></p>
</div>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">2&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">4&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">0 1</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">1 2&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">1 3&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">5&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">0 1&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">1 2&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">1 3&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">0 4&nbsp;</span></p>

<strong>Output:</strong>
<pre><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">Case 1: 2
Case 2: 3
</span></pre>
</pre>
<p> </p>