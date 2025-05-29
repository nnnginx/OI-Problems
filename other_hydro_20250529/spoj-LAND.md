<p>Indigo Real-estate Company is now planning to develop a new housing complex. The entire complex is a square,
all of whose edges are equally <i>a</i> meters. The complex contains <i>n</i> subdivided blocks, each of which is a <i>b</i>-meter
square. Here both <i>a</i> and <i>b</i> are positive integers.

</p><p>However the project is facing a big problem. In this country, a percentage limit applies to the subdivision of a
land, under the pretext of environmental protection. When developing a complex, the total area of the subdivided
blocks must not exceed 50% of the area of the complex; in other words, more than or equal to 50% of the newly
developed housing complex must be kept for green space. As a business, a green space exceeding 50% of the
total area is a <i>dead space</i>. The primary concern of the project is to minimize it.

</p><p>Of course purchasing and developing a land costs in proportion to its area, so the company also wants to minimize
the land area to develop as the secondary concern. You, a member of the project, were assigned this task, but can
no longer stand struggling against the problem with your pencil and paper. So you decided to write a program to
find the pair of minimum <i>a</i> and <i>b</i> among those which produce the minimum dead space for given <i>n</i>.

</p><h3>Input</h3>
<p>The input consists of multiple test cases. Each test case comes in a line, which contains an integer <i>n</i>. You may
assume 1 ¡Ü <i>n</i> ¡Ü 10000.
</p><p>The end of input is indicated by a line containing a single zero. This line is not a part of the input and should not
be processed.

</p><h3>Output</h3>
<p>For each test case, output the case number starting from 1 and the pair of minimum <i>a</i> and <i>b</i> as in the sample
output.
</p><p>You may assume both <i>a</i> and <i>b</i> fit into 64-bit signed integers.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
2
0

<b>Output:</b>
Case 1: 3 2
Case 2: 2 1

</pre>