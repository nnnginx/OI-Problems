<p>As we all know, every day, there are hundreds of trucks passing through the highway. As some of the trucks might carry several tons of goods, the highway will be damaged unless it is frequently repaired. The administration of highway is worried about this, so it invented repairing cars to ensure that the cars can pass through the highway.</p>
<p>The highway has an initial durability. If a truck with x tons¡¯ goods pass the highway, its durability will be decreased by x. Once the highway¡¯s durability is less or equal to zero, it will be broken and can never be repaired. The trucks can¡¯t pass through the broken ones.</p>
<p>There are two kinds of repairing cars: T1 can increase the highway¡¯s durability by r, T2 can increase the highway¡¯s durability to p, if the highway¡¯s durability is less than p. Although the repairing cars can pass through the broken parts, the broken parts can¡¯t be repaired.</p>
<h3>Input</h3>
<p>The input consists of several test cases.</p>
<p>For every test case, there are three integers N (1&lt;=N&lt;=100000), M (1&lt;=M&lt;=100000), I (1&lt;=I&lt;=1000) in the first line, indicating the highway¡¯s length, the numbers of cars and the initial durability of the highway.</p>
<p>Each of the next M lines described the information of cars in the following format:<br>1 s t d&nbsp;-- There is a truck with d tons¡¯ goods wanted to pass the interval [s, t]. You should check whether the truck can pass it. Notice that if the truck can't pass the whole interval, it will give up the whole passing; otherwise it can pass the highway freely, even if the highway will be broken after the truck¡¯s passing.<br>2 s t r&nbsp;-- A T1 car will pass the interval [s, t] and increase its durability by r.<br>3 s t p&nbsp;-- A T2 car will pass the interval [s, t] and increase its durability to p.</p>
<p>You can assume that 1&lt;=s&lt;=t&lt;=N, 1&lt;=d, p, r&lt;=1000</p>
<p>The input ends with N=M=I=0.</p>
<h3>Output</h3>
<p>For each case, you should return how many trucks can successfully pass the interval.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 5 5
1 1 3 3
2 2 3 10
1 1 3 3
1 1 3 1
1 2 3 1
5 3 10
1 1 2 5
1 2 3 5
1 1 3 5
0 0 0

<strong>Output:</strong>
3
2
</pre>
<h3>Hint</h3>
<p>In the second test case, the third truck can¡¯t pass the road, because although the durability of interval [1, 2) and (2, 3] is larger than 0, in position 2, the durability is 0.</p>