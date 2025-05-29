<p>A small group of archaeologists is working in the Antarctic. Their sensors have detected a number of caves in which there are interesting fossils. However, a thick layer of ice blocks the entrance to each cave. The archaeologists possess the equipment needed to burn a tunnel in the layer of ice, but the fuel is extremely expensive. In order to determine the size of each fossil the group has launched a number of probes through small bore-holes. Each probe which hit the fossil emits a signal consisting of its x and y coordinates. Your task is to determine the smallest possible size of the tunnel, which is equal to the maximal distance between any two probes (so that the fossil won¡¯t be damaged during extraction). The drilling equipment needs to be provided with the squared value of this distance.

</p><p>Given the list of coordinates of the points containing probes, find the square of the maximal distance between any two probes. 
</p><h3>Input</h3>
<pre><p>t [the number of tests &lt;= 20]
[empty line]
n [the number of active probes &lt;= 100000]
x1 y1 [coordinates of the first probe]
...
xn xn
[integer coordinates from -50000000 to 50000000]
[empty line]
[input for the next test cases...]
</p></pre>
<p>
Text grouped in [ ] does not appear in the input file.

</p><h3>Output</h3>
<pre>o1 [the square of the maximal distance in the first set]
[output for the next test cases...]
</pre>
<h3>Example</h3>

<pre><b>Input:</b>
5

1
2 -3

4
0 0
-2 2
2 2
1 0

6
-4 2
2 2
5 0
0 5
6 1
-1 -1

10
0 0
5 1
9 2
12 3
14 4
15 5
16 7
17 10
18 14
19 19

10
2 -3
-1 2
0 5
-5 -1
-4 2
4 0
1 3
4 3
-3 -4
0 -2

<b>Output:</b>
0
16
101
722
98
</pre>