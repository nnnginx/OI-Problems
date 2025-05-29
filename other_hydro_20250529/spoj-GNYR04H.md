<p style="font-family: 'Times New Roman'; font-size: medium;">Mr. Young wishes to take a picture of his class. The students will stand in rows, with each row no longer than the row behind it and the left ends of the rows aligned. For instance, 12 students could be arranged in rows (from back to front) of 5, 3, 3 and 1 students.</p>
<pre>X X X X X
X X X
X X X
X
</pre>
<p>&nbsp;</p>

<p style="font-family: 'Times New Roman'; font-size: medium;">In addition, Mr. Young wants the students in each row arranged so that heights decrease from left to right. Also, student heights should decrease from the back to the front. Thinking about it, Mr. Young sees that for the 12-student example, there are at least two ways to arrange the students (numbers represent heights, with 1 meaning the tallest):</p>

<pre> 1  2  3  4  5     1  5  8 11 12
 6  7  8           2  6  9
 9 10 11           3  7 10
12                 4
</pre>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>

<p style="font-family: 'Times New Roman'; font-size: medium;">Mr. Young wonders how many different arrangements of the students there might be for a given arrangement of rows. He tries counting by hand starting with rows of lengths 3, 2 and 1 and counts 16 arrangements:</p>
<pre>123 123 124 124 125 125 126 126 134 134 135 135 136 136 145 146
45  46  35  36  34  36  34  35  25  26  24  26  24  25  26  25
6   5   6   5   6   4   5   4   6   5   6   4   5   4   3   3
</pre>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>

<p style="font-family: 'Times New Roman'; font-size: medium;">Mr. Young sees that counting by hand is not going to be very effective for any reasonable number of students. He asks you to help out by writing a computer program to determine the number of different arrangements of students for a given set of rows.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>
<h1><span style="color: #ff0000; font-size: medium;">Input</span></h1>
<p style="font-family: 'Times New Roman'; font-size: medium;">The input describes a series of test, each described in two lines. The first line gives the number of rows,&nbsp;<span><em>k</em></span>, as a decimal integer. The second line contains the lengths of the rows from back to front&nbsp;<span>(<em>n</em><sub>1</sub>,<em>n</em><sub>2</sub>,...,&nbsp;<em>n</em><sub>k</sub>)</span>&nbsp;as decimal integers separated by single spaces. The problem set ends with a line with a row count of&nbsp;<tt>0</tt>. There will never be more than 5 rows and the total number of students,&nbsp;<span><em>N</em></span>, (sum of the row lengths) will be at most 30.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>

<h1><span style="color: #ff0000; font-size: medium;">Output</span></h1>
<p style="font-family: 'Times New Roman'; font-size: medium;">For each test case output a single integer: The number of arrangements of <span><em>N</em></span>&nbsp;students into the given rows, so that the heights decrease along each row from left to right and along each column from back to front (assume that all heights are distinct). The results should be in separate lines. The input data will be chosen so that the result will always fit in an unsigned 32-bit integer.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>

<h1><span style="color: #ff0000; font-size: medium;">Sample</span></h1>
<p><span style="color: #ff0000; font-size: medium;">Input&nbsp;</span><span style="font-size: medium;">&nbsp;</span></p>
<pre>1
30
5
1 1 1 1 1
3
3 2 1
4
5 3 3 1
5
6 5 4 3 2
2
15 15
0</pre>
<p><span style="color: #ff0000; font-size: medium;">Output&nbsp;</span><span style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</span></p>
<pre>1
1
16
4158
141892608
9694845</pre>