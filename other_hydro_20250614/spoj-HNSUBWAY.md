<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/HNSUBWAY/en/">English</a></td>
<td width="50%"><a href="/problems/HNSUBWAY/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Hanoi is constructing a subway system. The subway system consists of M stations which are numbered from 1 to M and K two-way subway lines connecting pairs of stations directly. Hanoi metropolitan area is covered by T separated resident blocks each described as convex polygons. Subway lines can run under resident blocks.  When running under resident blocks including their boundary, the speed of the subway train is v1 while its speed is v2 when running under other parts (v1 &lt; v2). The travel time between two stations a and b is the shortest time to go from a to b, possibly via intermediate stations (the transit time is not significant). They now have to select the central station from those existing stations so that the travel time from the central station to the farthest station, whose travel time to the central station is longest, is shortest.</p>
<p>The figure below describes a subway system with four subway stations and four subway lines.  There are three resident blocks in the metropolitan area. In this figure, there are two segments of subway lines under resident blocks where the subway train has to travel with speed of v1.</p>
<p><img src="./22788/file/Uidro8uw.png" alt=""></p>
<p>Given a subway system, your task is to write a program to find the central station and to find the travel time from the farthest station to the central station.</p>
<h3>Input</h3>
<p>The input file consists of several data sets. The first line of the input file contains the number of data sets which is a positive integer and is not bigger than 20. The following lines describe the data sets.</p>
<p>For each data set, the first line contains five integers M, K, T, v1, v2 (M &lt; 31, K &lt; 50, T &lt; 10, 0 &lt; v1 &lt; v2 &lt; 100) separated by space indicating number of stations, number of subway lines, number of resident blocks, the subway train speed when travelling under resident blocks, and the subway train speed when not travelling under resident blocks respectively. The ith line of the following M lines contains two integers Xi and Yi (-10000 ¡Ü Xi,Yi ¡Ü 10000) separated by space representing the coordinates of the ith station. The jth line of the following K lines contains two integers separated by space representing the two stations of the jth subway line. The gth line of the following T lines contains the description of the gth resident block. The line starts with an integer Vg (Vg &lt; 8) which is the number of vertices followed by Vg pairs of integers (with absolute value not exceeding 10000) separated by space indicating the coordinates of Vg vertices of the polygon in a traversal order around the polygon, representing the gth resident block.</p>
<h3>Output</h3>
<p>For each data set, write in one line an integer indicating the integer part of (tmax * 100) where tmax is the travel time from the farthest station to the central station.</p>
<h3>Example</h3>
<pre><strong>Sample Input</strong>
1
4 4 3 1 2
1 8
7 8
7 1
14 8
1 2
2 3
2 4
3 4
3 4 8 6 5 2 5
4 7 6 9 6 9 4 7 4
6 10 8 11 9 12 9 13 8 12 7 11 7	

<strong>Sample Output</strong>
500
</pre>
<p> </p>