<p> Farmer John has decided to construct electric fences. He has fenced his fields into a number of bizarre shapes and now must find the optimal place to locate the electrical supply to each of the fences.
<br><br>
A single wire must run from some point on each and every fence to the source of electricity. Wires can run through other fences or across other wires. Wires can run at any angle. Wires can run from any point on a fence (i.e., the ends or anywhere in between) to the electrical supply.
<br><br>
Given the locations of all F (1 &lt;= F &lt;= 150) fences (fences are always parallel to a grid axis and run from one integer gridpoint to another, 0 &lt;= X,Y &lt;= 100), your program must calculate both the total length of wire required to connect every fence to the central source of electricity and also the optimal location for the electrical source.
<br><br>
The optimal location for the electrical source might be anywhere in Farmer John's field, not necessarily on a grid point. 

</p><h3>Input</h3>
<p>The first line contains F, the number of fences.
<br>F subsequent lines each contain two X,Y pairs each of which denotes the endpoints of a fence.

</p><h3>Output</h3>
<p> On a single line, print three space-separated floating point numbers, each with a single decimal place. Presume that your computer's output library will round the number correctly.
<br><br>
The three numbers are:
<br><br>
* the X value of the optimal location for the electricity,
<br>* the Y value for the optimal location for the electricity, and
<br>* the total (minimum) length of the wire required. 

</p><h3>Example</h3>

<pre><b>Input:</b>
3
0 0 0 1
2 0 2 1
0 3 2 3

<b>Output:</b>
1.0 1.6 3.7
</pre>