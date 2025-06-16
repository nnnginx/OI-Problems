<p>Do you remember the box of Matryoshka dolls last week? Adam just got another box of dolls from Matryona. This time, the dolls have different shapes and sizes: some are skinny, some are fat, and some look as though they were attened. Specifically, doll i can be represented by three numbers wi, li, and hi, denoting its width, length, and height. Doll i can fit inside another doll j if and only if wi &lt; wj , li &lt; lj , and hi &lt; hj . That is, the dolls cannot be rotated when fitting one inside another. Of course, each doll may contain at most one doll right inside it. Your goal is to fit dolls inside each other so that you minimize the number of outermost dolls.</p>
<h3>Input</h3>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 54px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The input consists of multiple test cases. Each test case begins with a line with a single integer N, 1 ¡Ü N ¡Ü 500, denoting the number of Matryoshka dolls. Then follow N lines, each with three space-separated integers wi, li, and hi (1 ¡Ü wi; li; hi ¡Ü 10,000) denoting the size of the ith doll. Input is followed by a single line with N = 0, which should not be processed.</div>
<p>&nbsp;</p>
<p>The input consists of multiple test cases. Each test case begins with a line with a single integer N, 1 ¡Ü N ¡Ü 500, denoting the number of Matryoshka dolls. Then follow N lines, each with three space-separated integers wi, li, and hi (1 ¡Ü wi; li; hi ¡Ü 10,000) denoting the size of the ith doll. Input is followed by a single line with N = 0, which should not be processed.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>For each test case, print out a single line with an integer denoting the minimum number of outermost dolls that can be obtained by optimally nesting the given dolls.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
5 4 8
27 10 10
100 32 523
3
1 2 1
2 1 1
1 1 2
4
1 1 1
2 3 2
3 2 2
4 4 4
0


<strong>Output:</strong>
1
3
2<span style="white-space: normal;">
</span></pre>