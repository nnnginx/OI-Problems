<p>
In statistics, a histogram is a graphical display of tabulated frequencies, shown as bars.
 It shows what proportion of cases fall into each of several categories. It is a polygon composed of a sequence of rectangles aligned at a common base line. In this problem all rectangles have a width of unit length. But their heights are distinct. Some permutation of the heights will give the maximum perimeter. Your task is to find the maximum perimeter of the histogram and the number of permutations that give the maximum perimeter.
</p>

<center>
<img src="/content/swarnaprakash:hist2.jpg">
</center>
<p>
In the image Figure (a) shows a histogram with heights {1,2,3,4} (1st sample testcase) and has a perimeter of 16 units. Figure (b) shows one of the permutations {3,1,2,4} having the maximum perimeter of 20 units.
</p>

<h3 align="center">Input</h3>
<p>Input consists of multiple test cases. Each test case describes a histogram and starts with an integer <b>N</b>, 2 ¡Ü N ¡Ü 15, denoting the number of rectangles it is composed of. Next line consists of N space separated positive integers representing the heights of the rectangles. All heights are distinct and less than or equal to 100. N=0 indicates the end of tests. There are atmost 50 test cases.
</p>
<h3 align="center">Output</h3>
<p>For each test case output the maximum possible perimeter of the histogram and the number of permutations that give maximum perimeter in a single line, separated by a single space.</p>

<h3 align="center">Example</h3>

<pre><b>Input:</b>
4
1 2 3 4
3
2 6 5
0

<b>Output:</b>
20 8
24 2

</pre>