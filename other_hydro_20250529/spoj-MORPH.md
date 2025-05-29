<p>Morphic is a tree that grows very rapidly, bringing happiness to its owner. It has a single trunk
consisting of a number of cells stacked one on top of another. Each cell has one of n possible colors
which determine the way it mutates during the night, while nobody can see it. Florists denote these
colors by the first <b>n</b> small letters of the English alphabet and know exactly into how many cells, and of
what colors, a cell of each color divides. In fact, they have wrote their knowledge down simply with <b>n</b>
nonempty words, each word representing the resulting sequence of colors.
</p><p>A seed of a Morphic has a single cell of color a and is rooted firmly in the ground. As long as the
Morphic is still alive, each night all its cells simultaniously morph according to the aforementioned rules,
possibly causing an exponential growth because each new cell is of the same size as the original one. For
example, if rules say that a becomes ab, and b becomes ca, then after two nights a seed will evolve to
a trunk consisting of 4 cells: abca.
</p><p>Therefore the top of a Morphic is usually hidden in clouds. The only way to tell if it is still alive is
to check if visible part of the trunk is changing colors. In order to do so, one can build enormously high
(yet still of constant height) tower, and watch from its top a fixed fragment of the trunk.
</p><p>As you can easily see, it is either sufficient to observe first <b>k</b> cells from the bottom for some fixed <b>k</b>,
or no matter how high the tower is, you will not be able to tell for sure if a Morphic died. The latter
happens when for every <b>k</b>, rules cause the <b>k</b>-th cell to eventually stop changing colors, even though the
tree is still alive and mutating.
</p><p>To prevent waste of money on building such enormous towers, you are to write a program that
determines if it is possible to monitor health of a Morphic.</p>
<h3>Input</h3>
<p>The input contains several Morphics descriptions. The first line contains the number of descriptions <b>t</b>
(<b>t</b> &lt;= 10000) that follow. Each of them begins with the number of colors <b>n</b> (1 &lt;= <b>n</b> &lt;= 26). Next <b>n</b> lines
contain the rules by which the Morphic grows. The i-th one describes the sequence of colors in bottom-up
order obtained from a single cell of i-th color. Each line contains at most 100 lowercase English letters.</p>
<h3>Output</h3>
<p>For each test case output one line containing YES if building of a tower is pointless (as in: YES, we can
save money!). Otherwise output NO.</p>
<h3>Example</h3>
<pre><b>Input:</b>
4
2
ab
a
3
ba
c
c
3
ba
c
b
3
bbbbbbbbbbbbbbb
ccccccccccccccc
c

<b>Output:</b>
YES
YES
NO
YES
</pre>
<b>Warning: enormous input/output data, be careful with certain languages</b>