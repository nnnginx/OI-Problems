<p>Two groups of cavemen got into a land dispute and decided to settle it the old fashion-way, by throwing sticks at each other. The fight was organized in a cave, high enough that the ceiling is of no concern, but mineral deposits on the ground get in the way of flying sticks.</p>
<p>The cave can be divided into R rows and C columns, so that the entire cave consists of R��C cells. Each cell in the cave is either empty or contains a chunk of mineral. Two chunks of minerals are part of the same cluster if they are adjacent in one of the four main directions (up, down, left, right).</p>
<p>One group of cavemen is on the left side of the cave, the other on the right side. The groups alternate throwing sticks at the other group; first a group chooses the height at which the stick will fly and then (climbing on each others' shoulders as necessary) they throw it and the stick flies horizontally through the cave at the chosen height.</p>
<p>If the stick hits a chunk of mineral on the way, it destroys the chunk, the cell becomes empty and the stick stops its journey.</p>
<p>When a chunk is destroyed, it is possible that a cluster falls apart. If a newly created cluster would float in the air, then it falls down because of gravity. While falling, the cluster does not change shape i.e. all chunks in it fall together. As soon as some chunk in the falling cluster lands on a chunk from a different cluster or the ground, the entire cluster stops falling. Of  ourse, if a cluster lands on another, they merge and become one.</p>
<p>Your program will be given the layout of minerals in the cave and the heights at which sticks were
thrown. Determine the layout of minerals after the sticks are exchanged.</p>
<h3>Input</h3>
<p>The first line contains two integers R and C (1 �� R, C �� 100), the dimensions of the cave.</p>
<p>Each of the following R lines will contain C characters. The character '.' represents an empty cell, while the letter 'x' represents a chunk of mineral. </p>
<p>The next line contains an integer N (1 �� N �� 100), the number of sticks thrown.</p>
<p>The last line contains N integers separated by spaces, the heights at which sticks were thrown. All heights will be between 1 and R (inclusive), with height 1 being the bottom of the matrix and height R the top. The first tick is thrown left to right, the second right to left and so on.</p>
<p>No cluster will initially float in the air. Also, the input data will be such that at no point will two or
more clusters fall simultaneously, so that there will be no ambiguous situations.</p>

<h3>Output</h3>
<p>The output should consist of R lines, each containing C characters, the final layout of the cave, in the
same format as in the input.</p>

<h3>Example</h3>

<pre><b>Input:</b>
8 8
........
........
...x.xx.
...xxx..
..xxx...
..x.xxx.
..x...x.
.xxx..x.
5
6 6 4 3 1

<b>Output:</b>
........
........
........
........
.....x..
..xxxx..
..xxx.x.
..xxxxx.
</pre>