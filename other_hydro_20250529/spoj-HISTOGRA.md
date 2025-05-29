<p>

A histogram is a polygon composed of a sequence of rectangles aligned at a common base line.
The rectangles have equal widths but may have different heights.
For example, the figure on the left shows the histogram that consists of rectangles with the heights 2, 1, 4, 5, 1, 3, 3, measured in units where 1 is the width of the rectangles:

</p><center>
<img src="./22777/file/EAWr4qrS.png">
</center>

<p>
Usually, histograms are used to represent discrete distributions, e.g., the frequencies of characters in texts.
Note that the order of the rectangles, i.e., their heights, is important.
Calculate the area of the largest rectangle in a histogram that is aligned at the common base line, too.
The figure on the right shows the largest aligned rectangle for the depicted histogram.

</p><h3>Input Specification</h3><p>

The input contains several test cases.
Each test case describes a histogram and starts with an integer <code>n</code>, denoting the number of rectangles it is composed of.
You may assume that <code>1 &lt;= n &lt;= 100000</code>.
Then follow <code>n</code> integers <code>h<sub>1</sub>, ..., h<sub>n</sub></code>, where <code>0 &lt;= h<sub>i</sub> &lt;= 1000000000</code>.
These numbers denote the heights of the rectangles of the histogram in left-to-right order.
The width of each rectangle is <code>1</code>.
A zero follows the input for the last test case.


</p><h3>Output Specification</h3><p>

For each test case output on a single line the area of the largest rectangle in the specified histogram.
Remember that this rectangle must be aligned at the common base line.

</p><h3>Sample Input</h3><p>

</p><pre>7 2 1 4 5 1 3 3
4 1000 1000 1000 1000
0
</pre>

<h3>Sample Output</h3><p>

</p><pre>8
4000
</pre>