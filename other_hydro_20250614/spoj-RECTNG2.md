<p>A partition of a rectangle is either a whole rectangle or a subdivision the rectangle into either a upper part and a lower part or a left part and a right part, and each part is a partition of the corresponding rectangle. Figure 1 shows several examples of partitions.</p>
<p><img src="../../../content/john_jones:rectng21.jpg" alt=""></p>
<p>Figure 2 shows three equal sized rectangles, partitioned into sub-rectangles. Partition B is obtained from partition A by partitioning two of the sub-rectangles of A. Generally, if a partition B is obtained from A by partitioning one or more of its sub-rectangles, we say that B is finer than A, or that A is coarser than B. This relation is partial: partition C is neither coarser nor finer than A or B.</p>
<p><img src="../../../content/john_jones:rectng22.jpg" alt=""></p>
<p>Given two partitions D and E of the same rectangle, infinitely many partitions exist that are finer than both D and E. In Figure 3 both F and G are finer than D and E. Among the partitions that are finer than both D and E, a unique one exists that is coarsest. This partition is called the infimum of D and E. In Figure 3, partition F is the infimum of D and E.</p>
<p><img src="../../../content/john_jones:rectng23.jpg" alt=""></p>
<p>In Figure 4, both H and J are coarser than D and E. Here J is the finest partition that is coarser than D and E. Then J is the supremum of D and E.</p>
<p><img src="../../../content/john_jones:rectng24.jpg" alt=""></p>
<p>Write a program that, given two partitions of the same rectangle, finds the infimum and the supremum of these partitions.</p>
<h3>Input</h3>
<p>The input file contains one or more test cases. The first line of each test case gives the width w and height h of the rectangle (0 &lt; w, h &lt;= 20). In the next h+1 lines the two partitions are given, as in the sample. Each of these lines contains 4*w+3 characters. The first 2*w+1 of these belong to the first partition; the last 2*w+1 of these belong to the second partition. A space separates the two partitions. Horizontal lines are created using underscores ��_��, vertical lines using ��|��.</p>
<p>The input is terminated by a pair of zeroes.</p>
<h3>Output</h3>
<p>For every case in the input file the output contains a single line containing the case number (in the format shown in the sample), followed by the infimum and the supremum of the two partitions, using the same format as the input.</p>
<p>Place a blank line after the output of each test case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4 3
 _ _ _ _   _ _ _ _ 
|_ _ _ _| |_|_ _ _|
|   |   | |       |
|_ _|_ _| |_ _ _ _|
3 4
 _ _ _   _ _ _ 
| |   | | |   |
| |   | |_|_ _|
|_|_ _| |   | |
|_ _|_| |_ _|_|
0 0

<strong>Output:</strong>
Case 1:
 _ _ _ _   _ _ _ _ 
|_|_ _ _| |_ _ _ _|
|   |   | |       |
|_ _|_ _| |_ _ _ _|

Case 2:
 _ _ _   _ _ _ 
| |   | |     |
|_|_ _| |     |
|_|_|_| |     |
|_ _|_| |_ _ _|

</pre>
<b>Please read the problem statement carefully. The judge compares your output and the expected output, any extra whitespace will cause Wrong Answer.</b>