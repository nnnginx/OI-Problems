<p>A group of n children are playing with a set of n<sup>2</sup> flat square blocks. Each block is painted from above with one colour, and 
there are no more than 2 blocks of each colour. The blocks are initially arranged in an n x n square forming some sort of picture.
</p><p>
The children have been provided with some other n x n picture and asked to rearrange the blocks to that form. Since this is not really what they enjoy doing most, they intend to solve the task together and spend as little time on it as possible. Thus, every minute each child chooses a single 1 x n row or n x 1 column of blocks to rearrange. This row/column may never intersect with rows/columns chosen by other children in the same minute. A child takes one minute to perform any rearrangement (permutation) of the blocks within its row/column it likes.
</p><p>
Determine whether the children can perform their task of converting one block image into the other, and if so -- find the minimum possible time in minutes required to achieve this.

</p><h3>Input</h3>
<p>
The input starts with a line containing a single integer t&lt;=200, the number of test cases. t test cases follow. 

Each test case begins with a line containing integer n (1&lt;=n&lt;=500). The next n lines contain n integers P<sub>i,j</sub> each, forming a bitmap matrix representing the colours of the blocks in their initial configuration (1&lt;=P<sub>i,j</sub>&lt;=n<sup>2</sup>). The following n lines contain n integers Q<sub>i,j</sub> each, corresponding to the matrix for the final configuration (1&lt;=Q<sub>i,j</sub>&lt;=n<sup>2</sup>). 

</p><h3>Output</h3>
<p>For each test case output a line with a single non-negative integer corresponding to the number of minutes required to transform matrix P into matrix Q, or the word <tt>no</tt> if no such transformation is possible.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
3
1 3 4
2 1 3
2 5 5
3 1 3
2 1 2
4 5 5
3
1 2 3
4 5 6
7 8 9
1 5 6
4 2 9
7 8 3
2
1 2
1 2
1 3
1 2

<b>Output:</b>
2
1
no
</pre>

<p>
The actions taken in the first test case are illustrated below.
</p><p>
<img src="/content/adrian:blocks.png" alt="2 step transformation: 134 213 255 -> 413 312 255 -> 313 212 455">
</p>
<b>Warning: enormous Input/Output data, be careful with certain languages</b>