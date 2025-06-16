<p>Given an image <i>I</i> with <i>N</i> columns and <i>M</i> rows, a diagonal projection is the vector (<i>d<sub>1</sub></i>, <i>d<sub>2</sub></i>, ..., <i>d<sub>M+N-1</sub></i>) where <i>d<sub>i</sub></i> = ¦²<i><sub>x+y-1=i</sub> I(x,y)</i>.
Here <i>I(x,y)</i>, <i>1</i> ¡Ü <i>x</i> ¡Ü <i>N</i>, <i>1</i> ¡Ü <i>y</i> ¡Ü <i>M</i>, is the image intensity (a non-negative integer less than 256) at column <i>x</i> and row <i>y</i>.

</p><p>You are given a set of images and you are asked to find the diagonal projection for each of them.

</p><h3>Input</h3>
<p>The first line of input contains a positive number, the number of images that follow. For each image there is a line with <i>N</i> and <i>M</i>. The following <i>M</i> lines describe one row each starting from row 1. A row is described in run-length encoding by pairs of numbers separated by spaces. The first number in each pair is the length of the run and the second number is the image intensity. Obviously, for each row, the run lengths add up to <i>N</i>.  As in the example input, there is a blank line between each two consecutive images and before the first one.

</p><p>The number of test cases is at most 10.
The width of each image is less than <i>10<sup>9</sup></i> and the height is less than <i>10<sup>3</sup></i>.
Additionally, the total size of the input does not exceed 4 MB.

</p><h3>Output</h3>
<p>For each image you should output one line, the diagonal projection for the image in run length encoding. The number of output lines should be the same as the number of images in the input. All the numbers on a line should be separated by exactly one space.

</p><p>When encoding the output in run-length encoding, the runs should be as long as possible, i.e. no two consecutive runs should have the same intensity value.

</p><h3>Example</h3>

<pre><b>Input:</b>
2

3 3
1 1 1 2 1 3
1 1 1 2 1 3
1 3 1 2 1 1

3 2
3 1
3 1

<b>Output:</b>
1 1 1 3 1 8 1 5 1 1
1 1 2 2 1 1
</pre>