<p>
Our superhero Carry Adder has uncovered the secret method that the evil Head Crash uses to generate the entrance code to his fortress in Oakland. The code is always the number of distinct binary search trees with some number of nodes, that have a specific property. To keep this code short, he only uses the least significant nine digits. The property is that, for each node, the height of the right subtree of that node is within one of the height of the left subtree of that node. Here, the height of a subtree is the length of the longest path from the root of that subtree to any leaf of that subtree. A subtree with a single node has a height of 0, and by convention, a subtree containing no nodes is considered to have a height of −1.
</p>

<h3>Input</h3>
<p>
Input will be formatted as follows. Each test case will occur on its own line. Each line will contain only a single integer, N, the number of nodes. The value of N will be between 1 and 1427, inclusive.
</p>

<h3>Output</h3>
<p>Your output is one line per test case, containing only the nine-digit code (note that you must print leading zeros).</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
1
3
6
21

<strong>Output:</strong>
000000001
000000001
000000004
000036900</pre>