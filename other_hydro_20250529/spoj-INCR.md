<p>
A sequence <b>p(1)</b>, <b>p(2)</b>, ..., <b>p(N)</b> consisting of numbers 1, 2, ..., <b>N</b> is called a permutation if all elements in the sequence are different.

</p><p>
It is said that a permutation <b>p</b> contains increasing subsequence of <b>k</b> elements when there are numbers 
1 ¡Ü <b>i<sub>1</sub></b> &lt; <b>i<sub>2</sub></b> &lt; ... &lt; <b>i<sub>k</sub></b> ¡Ü N such that <b>p(i<sub>1</sub>)</b> &lt; <b>p(i<sub>2</sub>)</b> &lt; ... &lt; <b>p(i<sub>k</sub>)</b>.

</p><p>
When a permutation <b>p</b> contains an increasing subsequence consisting of <b>B</b> elements and does not contain an increasing subsequence consisting of <b>B+1</b> elements then the number <b>B</b> is called the degree of increase of this permutation.

</p><p>
You need to write a program which being given a number <b>N</b> calculates the number of permutations whose degree of increase is <b>B</b>.
Since the number of such permutations might be quite big, it is necessary to calculate its remainder of integer division by 1 000 000 000.

</p><h3>Input</h3>
<p>First line of input contains integer <b>T</b> (1 ¡Ü <b>T</b> ¡Ü 60) - the number of testcases. Then descriptions of <b>T</b>
testcases follow.

</p><p>The description of the testcase consists of one line. The line contains two integer numbers <b>N</b> and <b>B</b> (1 ¡Ü <b>N</b> ¡Ü 40, 1 ¡Ü <b>B</b> ¡Ü 5)
separated by one or more spaces.

</p><h3>Output</h3>
<p>For each testcase in the input your program should output one line. This line should contain one integer number which is the remainder of integer division by 1 000 000 000 of the number of permutations whose degree of increase is <b>B</b>.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
3 2

<b>Output:</b>
4
</pre>