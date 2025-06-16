<div align="justify">
<p>
A cargo shipment containing N (1 &lt;= <b>N</b> &lt;= 10<sup>5</sup>) boxes, has just arrived and it requires some regrouping. 
All the cargo is currently placed on a long circular conveyor belt of length <b>L</b> metres (1 &lt;= <b>L</b> &lt;= 10<sup>9</sup>), 
which you can control and perform the following operations.
</p><ul>
<li>Rotate the wheel clock wise or anti-clockwise (free of cost).
</li><li>Hold the cargo at some point and not let it move, while the belt is rolling. 
This causes the cargo behind it to come closer to this cargo by one step. 
Any consecutive sequence of cargo is grouped together and called as a luggage. The aim of the program is to group all cargo as a single luggage. Now the cost of this holding operation for one second is equal to the weight of the <i>luggage</i> that is held fixed. Also please note that you can hold the luggage only at ends of the luggage and never at inbetween points.
</li></ul>
Each unit of cargo weighs exactly one Kg. The conveyor belt rotates at a speed of one meters per second.<br>
This cost function directly reflects the human effort required to group the cargo. Workers would be happy if you can write a program that prints the minimal required effort to group the cargo, assuming an intelligent sequence of operations. <br>
<p></p>
<br>
<b>Input Format:</b><br>
The input file consists of multiple testcases. <br>
The first line of each testcase contains two integers, <b>N</b> and <b>L</b>. <br>
The following <b>N</b> lines contain one integer each specifying the position of the <b>i<sup>th</sup></b> cargo on the belt. The positions will be between 0 &amp; <b>L-1</b>. <br>
Input terminates with a line containing N=0 and L=0 which must not be processed. <br>
<br>
<b>Output Format:</b><br>
For each testcase print one integer in a single line, which is the minimal required cost for grouping all the cargo into a single luggage.<br>
<br>
<b>Sample Input:</b><br>
<pre>3 5
0
1
3
2 3
0
1
5 20
2
7
12
9
13
0 0
</pre>

<b>Sample Output:</b><br>
<pre>1
0
10
</pre>

NOTE: Please use 64-bit integers.
</div>