<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For example, the following tree is nice,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><nice-tree.jpg></nice-tree.jpg></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">but the following tree is not.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><not-nice-tree.jpg></not-nice-tree.jpg></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The leaves of a nice binary tree are labeled by the letter ¡®l¡¯, and other nodes are labeled by the letter ¡®n¡¯.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Given the pre-order traversal of a nice binary tree, you are required to find the depth of the tree.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Notes :&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1. The depth of a tree is defined as the length of the longest path with one end at the root.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2. The pre-order traversal of the tree in the first image above produces the string ¡°nlnnlll¡±.</div>
<p>Binary trees can sometimes be very difficult to work with. Fortunately, there is a class of trees with some really nice properties. A rooted binary tree is called ¡°nice¡±, if every node is either a leaf, or has exactly two children.</p>
<p>For example, the following tree is nice,</p>
<p><img style="vertical-align: middle;" src="./23608/file/2IwCmEnu.png" alt="nice tree" width="77" height="120"></p>
<p>but the following tree is not.</p>
<p><img style="vertical-align: middle;" src="./23608/file/Zx5ZXrwu.png" alt="not a nice binary tree" width="96" height="120"></p>
<p>The leaves of a nice binary tree are labeled by the letter ¡®l¡¯, and other nodes are labeled by the letter ¡®n¡¯.</p>
<p>Given the pre-order traversal of a nice binary tree, you are required to find the depth of the tree.</p>
<p><strong>Notes</strong> :&nbsp;</p>
<p>1. The depth of a tree is defined as the length of the longest path with one end at the root.</p>
<p>2. The pre-order traversal of the tree in the first image above produces the string ¡°nlnnlll¡±.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains the number of test cases T. T lines follow. Each line contains a string, which represents the pre-order traversal of a ¡°nice¡± binary tree. Leaves are represented by the letter ¡®l¡¯ and other nodes by the letter ¡®n¡¯. The input is guaranteed to be the preorder traversal of a nice binary tree.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Output one line for each test case, containing a single integer, the depth of tree.</p>
<p>&nbsp;</p>
<div>
<h3>Constraints</h3>
<p>0 &lt; T &lt; 20</p>
<p>Length of the input string in each test case is at most 10000.</p>
<p>&nbsp;</p>
</div>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
l
nlnll
nlnnlll


<strong>Output:</strong>
0
2
3<span style="white-space: normal;">
</span></pre>