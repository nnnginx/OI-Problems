<p>Ohani has recently learned about complete binary tree and binary search tree. Now she wants to create a complete binary tree and insert some value in the nodes such that it maintains the property of a binary search tree. She calls this tree Complete Binary Search Tree. So she takes a sorted array and one by one she inserts the values in a complete binary tree to create Complete Binary Search Tree (CBST).</p>
<p>A binary tree is called a Binary Search Tree if for each node u, the value of u is greater than every value in the left subtree of u and is less than every value in right subtree of u.</p>
<p>A binary tree is said to be complete if all its levels, expect possibly the last, have the maximum number of possible nodes, and if all the nodes at the last level appears as far left as possible. So, there is a unique complete tree for n nodes. Here is a complete tree of 10 nodes.</p>
<p><img src="file://WfTewylT.png" alt="binary tree" width="413" height="291"></p>
<h3><span style="font-weight: normal;">Let a sorted array of five element is: 1 3 4 6 9. So, the CBST of this array is:</span></h3>
<p><span style="font-weight: normal;"><img src="file://MvSTZ1Kq.png" alt="CBST" width="313" height="211">&nbsp;</span></p>
<h3><span style="font-weight: normal;">But suddenly she comes through a problem. Her teacher gave her an array which is unsorted. So, she first sort the array and then use the sorted array to create CBST. To sort the array, she takes any elements and place it at any place in the array in one step. For example: if an array is: 1 4 2 3, she can take 2 and place it after 1, she can then take 4 and place it after 3, so, total 2 steps sorts the array. But this is not the minimum. Now your task is to find the minimum number of steps needed to sort an unsorted array using Ohani's procedure and then build a CBST.</span></h3>
<h3>Input</h3>
<p>The first line of the input contains an integer T (1&lt;=5) denoting the number of test cases.</p>
<p>Each test case contains of two lines. First line contains an integer N(1&lt;=N&lt;=100000), &nbsp;the number of elements in the array.<br>Next line contains N distinct numbers where each numbers will be between 1 to N&nbsp;</p>
<h3>Output</h3>
<p>For each test case, you need to output the case number on &nbsp;the first line.<br>In the second line you have to output the minimum numbers of steps required to sort the array.<br>In the third line, for each &nbsp;value from 1 to N, the parent of these values in the built CBST. The parent of the root is -1.</p>
<p>For example, for if the given array is: 1 4 2 3, then the output for the CBST is,</p>
<p>2 3 -1 3</p>
<p>Because, the parent of value 1 is 2, the parent of value 2 is 3, 3 is the root, so, it's parent is -1, the parent of 4 is 3.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1<br>4<br>1 4 2 3

<strong>Output:</strong>
Case 1:<br>Minimum Move:&nbsp;1<br>2 3 -1 3&nbsp;</pre>