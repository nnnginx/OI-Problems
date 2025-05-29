<p>As you might already know, Ada the Ladybug is a farmer. She has multiple farmhouses and some fields which always connect two adjacent farmhouses. She plans to buy some scarecrows to scare crows!</p>
<p>A scarecrow placed on a farmhouse scares all crows from all adjacent fields. A crow on a field can be disasterous, so Ada has to arrange the scarecrows in such way that they cover all the fields. As scarecrows are pretty expensive she wants to minimize the number of them. Can you count it for her?</p>
<p><strong>Note: </strong> Even thought it might look like that from description, the formed "graph" doesn't have to be planar! Also multi-fields and self-field are not allowed.</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>1 ¡Ü T ¡Ü 100</strong></p>
<p>Each of the next <strong>T</strong> test-cases begins with two integers <strong>0 ¡ÜM ¡Ü     150, 1 ¡Ü N ¡Ü     150</strong>, the number of farmhouses and the number of fields.</p>
<p>Each of next <strong>M</strong> lines contains two numbers <strong>0¡Ü     A<sub>i</sub>,A<sub>j</sub> &lt; N</strong>, the farmhouses, which are connected by a field.</p>
<h3>Output</h3>
<p>For each test-case output the minimal number of scarecrows Ada has to buy, to cover all fields.</p>
<h3>Example Input</h3>
<pre>6
3 3
1 2
1 0
2 0
4 3
1 2
1 3
1 0
5 6
0 2
0 3
1 3
1 2
1 4
2 4
5 8
0 1
0 3
0 4
1 2
1 4
3 4
3 2
2 4
4 2
0 1
2 3
6 9
0 4
4 3
1 2
2 0
2 3
5 3
4 1
4 2
5 0
</pre>
<h3>Example Output</h3>
<pre>2
1
3
3
2
3</pre>
<h3>Example Input 2</h3>
<pre>2
17 7
12 9
11 8
9 16
11 2
5 14
7 6
8 14
16 23
10 13
11 3
7 14
14 3
9 11
7 8
0 9
8 14
10 8
0 4
6 15
6 12
2 5
10 2
7 11
13 12
15 13
5 3
15 0
6 2
12 9
5 1
1 4
</pre>
<h3>Example Output 2</h3>
<pre>4
9
</pre>