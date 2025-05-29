<p align="left">Professor Z. always gives his students lots of boring homework. Last week, after explaining binary search trees (BSTs), he asked his students to draw a picture of BST according to the list of numbers inserted into the tree sequentially. Maryanna spent so much time playing the game "Starcraft II" that she can't finish her homework in time. She needs your help.</p>
<p align="left">&nbsp;<em>A binary search tree, which may sometimes also be called ordered or sorted binary tree, is a node-based binary tree data structure which has the following properties:</em></p>
<p align="left"><em>The left subtree of a node contains only nodes with keys less than the node's key.</em></p>
<p align="left"><em>The right subtree of a node contains only nodes with keys greater than the node's key.</em></p>
<p align="left"><em>Both the left and right subtrees must also be binary search trees.</em></p>
<p align="right"><em>--from Wikipedia</em>&nbsp;</p>
<p align="left">To draw a picture of BST, you may follow the rules listed below:&nbsp;</p>
<ol>
<li>The picture of a 1-node BST, whose size is 1*1, is a single 'o' (15th small Latin letter).</li>
<li>If a BST has a non-empty subtree, draw a single '|' just above the subtree's root, and a single '+' just above previous drawn '|'. Finally, in the row of '+', use the least number (including 0) of '-'s to connect '+' (denoting the left subtree and right subtree) and 'o' (denoting the parent node of the subtree)</li>
<li>The left subtree (if exists) must be drawn on the left side of its parent. Similarly, the right subtree (if exists) must be drawn on the right side of its parent. </li>
<li>The column of the BST's root must not contain any character from left subtree or right subtree.</li>
<li>Any column containing any characters from BST's left subtree must not contain any characters from BST's right subtree, and vice versa. That is, for a node of the BST, the picture of its left subtree and the picture of its right subtree do not share common columns in the picture of the whole tree.</li>
</ol>
<p align="left">&nbsp;The sample output may give a clear clarification about the format of the picture.</p>
<h3>Input</h3>
<p align="left">The first line contains <strong>T</strong> (<strong>T</strong> &lt;= 2500), the number of test cases. T lines follow. Each line contains a positive integer <strong>N</strong> (<strong>N</strong> &lt; 80), followed by <strong>N</strong> integers - a permutation of 1 to <strong>N</strong>. The permutation indicates the insert order for the BST.</p>
<h3>Output</h3>
<p align="left">For each test case:</p>
<p align="left">Output the case number counting from 1 in the first line. The next lines should be the image described above without any trailing spaces. See the sample for more format details.</p>
<p align="left"><em>Notice that no trailing whitespaces after the last visible characters of each line are allowed.</em></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
3 3 1 2
6 4 5 6 1 3 2
5 3 4 5 2 1

<strong>Output:</strong>
Case #1:
+-o
|
o+
 |
 o
Case #2:
+--o+
|   |
o-+ o+
  |  |
 +o  o
 |
 o
Case #3:
 +o+
 | |
+o o+
|   |
o   o
</pre>