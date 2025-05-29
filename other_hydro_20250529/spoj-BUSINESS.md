<p style="font-family: Times; font-size: medium;">John Digger is the owner of a large illudium phosdex mine. The mine is made up of a series of tunnels that meet at various large junctions. Unlike some owners, Digger actually cares about the welfare of his workers and has a concern about the layout of the mine. Specifically, he worries that there may a junction which, in case of collapse, will cut off workers in one section of the mine from other workers (illudium phosdex, as you know, is highly unstable). To counter this, he wants to install special escape shafts from the junctions to the surface. He could install one escape shaft at each junction, but Digger doesn't care about his workers that much. Instead, he wants to install the minimum number of escape shafts so that if any of the junctions collapses, all the workers who survive the junction collapse will have a path to the surface.</p>
<p style="font-family: Times; font-size: medium;">Write a program to calculate the minimum number of escape shafts and the total number of ways in which this minimum number of escape shafts can be installed.</p>
<h3>Input</h3>
<p style="font-family: Times; font-size: medium;">The input consists of several test cases. The first line of each case contains a positive integer&nbsp;<span><em>N</em></span>&nbsp;<span>(<em>N</em><img src="file://5jjZf9Fd.png" border="0" alt="$ le$" width="18" height="31" align="MIDDLE">5<sup>&nbsp;.&nbsp;</sup>10<sup>4</sup>)</span>&nbsp;indicating the number of mine tunnels. Following this are&nbsp;<span><em>N</em></span>&nbsp;lines each containing two distinct integers&nbsp;<span><em>s</em></span>&nbsp;and&nbsp;<span><em>t</em></span>, where&nbsp;<span><em>s</em></span>&nbsp;and&nbsp;<span><em>t</em></span>&nbsp;are junction numbers. Junctions are numbered consecutively starting at 1. Each pair of junctions is joined by at most a single tunnel. Each set of mine tunnels forms one connected unit (that is, you can get from any one junction to any other).</p>
<p style="font-family: Times; font-size: medium;">The last test case is followed by a line containing a single zero.</p>
<h3>Output</h3>
<p style="font-family: Times; font-size: medium;">For each test case, display its case number followed by the minimum number of escape shafts needed for the system of mine tunnels and the total number of ways these escape shafts can be installed. You may assume that the result fits in a signed 64-bit integer.</p>
<p style="font-family: Times; font-size: medium;">Follow the format of the sample output.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre>9
1 3
4 1
3 5
1 2
2 6
1 5
6 3
1 6
3 2
6 
1 2
1 3
2 4
2 5
3 6
3 7
0</pre>
<strong>Output:</strong>
<pre>Case 1: 2 4
Case 2: 4 1</pre>
</pre>