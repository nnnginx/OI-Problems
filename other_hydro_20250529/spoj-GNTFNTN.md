<p>The Dystopian government has installed a giant fountain in front of the parliament building. The fountain consists of N levels stacked one on top of the other and is situated on top of a large tank of infinite capacity. The levels of the fountain are numbered 1 to N from top to bottom. The top l<sub>1</sub> levels are identical with capacity c<sub>1</sub>, the next l<sub>2</sub> levels identical with capacity c<sub>2</sub>,... the final l<sub>K</sub> levels with capacity c<sub>K</sub>. Here l<sub>1</sub> + l<sub>2</sub> + ... l<sub>K</sub> = N.</p>
<p>When water is added to level i beyond its capacity, the excess water overflows to level i+1. Water overflowing from level N is collected in the tank. Water is added to the levels in the following fashion. First, w<sub>1</sub> amount of water is added to each level i such that s<sub>1</sub> ¡Ü i ¡Ü e<sub>1</sub>. Then w<sub>2</sub> amount of water is added to each s<sub>2</sub> ¡Ü i ¡Ü e<sub>2</sub>... Finally w<sub>M</sub> amount is added to s<sub>M</sub> ¡Ü i ¡Ü e<sub>M</sub>. Note that water might be added to the same level multiple times in this fashion.  You have to find out the amount of water that has overflowed to the tank at the bottom, and the total number of levels of the fountain that are completely filled</p>
<h3>Input</h3>
<p>The first line of the input contains T (¡Ü10), the number of test cases. Following this are the descriptions of the test cases.</p>
<p>The first line of the description of a test case contains space separated integers N (¡Ü2x10<sup>8</sup>), K (¡Ü2000) and M (¡Ü10<sup>4</sup>). Following this are K lines, each containing a space separated pair of integers. These are the (l<sub>i</sub>,c<sub>i</sub>) pair as explained in the problem statement. Here l<sub>1</sub> + l<sub>2</sub> + ... l<sub>K</sub> = N and c<sub>i</sub> ¡Ü 10<sup>8</sup>. This is followed by M lines, each containing a space separated triplet of integers. These are (s<sub>i</sub>,e<sub>i</sub>,w<sub>i</sub>) as explained in the problem statement. 1 ¡Ü s<sub>i</sub> ¡Ü e<sub>i</sub> ¡Ü N and w<sub>i</sub> ¡Ü 10<sup>6</sup></p>
<h3>Output</h3>
<p>For each test case output a space separated pair of integers : The total amount of water that has overflowed to the tank and the number of levels of the fountain that are completely filled.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
10 2 1
5 6
5 3
3 9 5

<strong>Output:</strong>
5 5
</pre>