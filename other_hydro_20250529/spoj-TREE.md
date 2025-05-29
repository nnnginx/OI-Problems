<p style="text-align: justify;">Tree is an important data structure in Computer
Science. Of all trees we work with, Binary Tree is probably the most popular
one. A Binary Tree is called a <b>Strictly Binary Tree</b> if every nonleaf
node in a binary tree has nonempty left and right subtrees. Let us define <b>a
Strictly Binary Tree of depth d</b>, as a Strictly Binary Tree that has at
least one root to leaf path of length <b>d</b>, and no root to leaf path in
that tree is longer than <b>d</b>. So let us use a similar reasoning to
define a generalized structure. <span style=""><o:p></o:p></span></p>

<p style="text-align: justify;">An n-ary Tree is called a <b>Strictly n-ary Tree</b>
if every nonleaf node in an n-ary tree has n children each. A <b>Strictly
n-ary Tree of depth d</b> can now be defined as a Strictly n-ary Tree that
has at least one root to leaf path of length d, and no root to leaf path in
that tree is longer than d. </p>

<p style="text-align: justify;">Given the value of n and depth d, your task is to
find the number of different strictly n-ary trees of depth d. </p>

<p style="text-align: justify;">The figure below shows the 3 different strictly
binary trees of depth 2.</p>
<img src="/content/quanghuy:tree8jt.png">


<h3>Input</h3>
<p style="text-align: justify">
Input consists
of several test cases. Each test case consists of two integers <b>n (0 &lt; n
&lt;= 32), d (0 &lt;= d &lt;= 16)</b>. Input is terminated a test case where
n=0 and d=0, you must not process this test case.</p>

<h3>Output</h3>
<p style="margin: 0in 0in 0.0001pt; text-align: justify;">For each test
case, print three integers, n, d and the number of different strictly n-ary
trees of level d, in a single line. There will be a single space in between two
integers of a line. You can assume that you would not be asked about cases
where you had to consider trees that may have more than 2<sup>10</sup> nodes in
a level of the tree. You may also find it useful to know that the answer for
each test case will always fit in a 200 digit integer.</p>

<h3>Example</h3>

<pre><b>Input:</b>
2 0
2 1
2 2
2 3
3 5
0 0

<b>Output:</b>
2 0 1
2 1 1
2 2 3
2 3 21
3 5 58871587162270592645034001
</pre>