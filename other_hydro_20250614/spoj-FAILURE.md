<p>To help their clients deal with faulty Cash Machines, the board of The Planar Bank has decided to stick a label expressing sincere regret and sorrow of the bank about the failure on every ATM. The very same label would gently ask the customer to calmly head to the nearest Machine (that should hopefully work fine).</p>
<p>In order to do so, a list of two-dimensional locations of all n ATMs has been prepared, and your task is to find for each of them the one closest with respect to the Euclidean distance.</p>
<h3>Input</h3>
<p>The input contains several test cases. The very first line contains the number of cases t (t  ¡Ü 15) that follow. Each test cases begin with the number of Cash Machines n (2 ¡Ü n ¡Ü 10<sup>5</sup>). Each of the next n lines contain the coordinates of one Cash Machine x, y (0 ¡Ü x, y ¡Ü 10<sup>9</sup>) separated by a space. No two points in one test case will coincide.</p>
<h3>Output</h3>
<p>For each test case output n lines. i-th of them should contain the squared distance between the i-th ATM from the input and its nearest neighbour.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
10
17 41
0 34
24 19
8 28
14 12
45 5
27 31
41 11
42 45
36 27
15
0 0
1 2
2 3
3 2
4 0
8 4
7 4
6 3
6 1
8 0
11 0
12 2
13 1
14 2
15 0
<strong>Output:</strong>
200
100
149
100
149
52
97
52
360
97
5
2
2
2
5
1
1
2
4
5
5
2
2
2
5
</pre>