<p>Every year there is the same problem at Halloween: Each neighbor is only willing to give a certain total number of sweets on that day, no matter how many children call on him, so it may happen that a child will get nothing if it is too late. To avoid conflicts, the children have decided they will put all sweets together and then divide them evenly among themselves. From last year's experience of Halloween they know how many sweets they get from each neighbour. Since they care more about justice than about the number of sweets they get, they want to select a subset of the neighbours to visit, so that in sharing every child receives the same number of sweets. They will not be satisfied if they have any sweets left which cannot be divided.</p>
<p>Your job is to help the children and present a solution.</p>
<h3>Input</h3>
<p>The input contains several test cases. <br> The first line of each test case contains two integers <strong>c</strong> and <strong>n</strong> (<em>1 �� c �� n �� 100000</em>), the number of children and the number of neighbours, respectively. The next line contains <strong>n</strong> space separated integers <strong>a<sub>1</sub> , ... , a<sub>n</sub></strong> (<em>1 �� a<sub>i</sub> �� 100000 </em>), where <strong>a<sub>i</sub></strong> represents the number of sweets the children get if they visit neighbour <strong>i</strong>.</p>
<p>The last test case is followed by two zeros.</p>
<h3>Output</h3>
<p>For each test case output one line with the indices of the neighbours the children should select (here, index <strong>i</strong> corresponds to neighbour <strong>i</strong> who gives a total number of <strong>a<sub>i</sub></strong> sweets). If there is no solution where each child gets at least one sweet, print "no sweets" instead. Note that if there are several solutions where each child gets at least one sweet, you may print any of them.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4 5
1 2 3 7 5
3 6
7 11 2 5 13 17
0 0


<strong>Output:</strong>
3 5
2 3 4
</pre>