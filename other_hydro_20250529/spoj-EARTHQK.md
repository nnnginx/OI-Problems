<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/EARTHQK/en/">English</a></td> 
<td width="50%"><a href="/problems/EARTHQK/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>
In 3010, a group of people from the Earth has moved to live in the planet Alpha. Because the climatic condition of the planet is very severe, only a certain part of land can be cultivated.
</p>
<p> 
Suppose that the surface of the planet is a plane, and the cultivable land has the shape of a non self-cutting polygon which has N vertices with coordinates (X1, Y1), (X2, Y2), ..., (Xn , Yn), listed in a traversal order around the polygon. On the cultivable land, the group of people from Earth lives in a research station at position (Xp, Yp).
</p>
<img src="./22265/file/UJAj8Ggf.png">
<p>
On the planet Alpha, earthquakes often occur. Each time an earthquake occurs, a crack is created that people can not move through. This crack can go through the cultivable land and divide the cultivable land into separated parts. Luckily, the crack never crosses the research station. The example in the figure above shows two cracks divide the cultivable land into three separated parts, and the area of cultivable land that the group of people living in the research station can reach after two earthquakes is 22.
</p>
<p>
Let's assume that there are M earthquakes occurred, which are numbered from 1 to M. Each earthquake generated a crack that is described by a line passing through two points (Xj1, Yj1) and (Xj2, Yj2) (j=1..M).
</p>
<p> 
Your task is to write a program to calculate the area of cultivable land that the group of people living in the research station in position (Xp, Yp) can reach after M earthquakes.
</p>
<h3>Input</h3>
<p>
The input file consists of several data sets. The first line of the input file contains the number of data sets which is a positive integer and is not bigger than 20. The following lines describe the data sets.
</p>
<p>
For each data test, the first line contains the integer N (3 ��  N ��  1000). The ith line of the following N lines contains two integers Xi and Yi (-10000 �� Xi,Yi �� 10000) separated by space, denoting the coordinates of ith vertex of the polygon, representing the cultivable land. The next line contains two integers (Xp,Yp) (-10000 �� Xp,Yp �� 10000) separated by space, denoting the coordinates of the research station. The next line contains the integer M (1 �� M �� 1000). The jth line of the following M lines contains four integers Xj1, Yj1, Xj2, and Yj2 separated by space, describing the line representing the crack created by the jth earthquake.
</p>
<h3>Output</h3>
<p>
For each data test, write in one line an integer indicating the integer part of (s * 100) where s is the area of reachable cultivable land after M earthquakes.
</p>

<h3>Example</h3>
<pre><b>Sample Input</b>
2
3
0 0
2 0
0 2
0 0
1
1 1 1 0
6
1 1
9 1
9 5
5 5
5 8
1 8
5 3
2
1 1 5 8
7 1 7 2	

<b>Sample Output</b>
150
2200
</pre>