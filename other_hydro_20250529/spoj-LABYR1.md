<p align="justify">
The northern part of the Pyramid contains a very large and complicated labyrinth. The labyrinth is divided into square blocks, each of them either filled by rock, or free. There is also a little hook on the floor in the center of every free block. The ACM have found that two of the hooks must be connected by a rope that runs through the hooks in every block on the path between the connected ones. When the rope is fastened, a secret door opens. The problem is that we do not know which hooks to connect. That means also that the neccessary length of the rope is unknown. Your task is to determine the maximum length of the rope we could need for a given labyrinth.</p>

<h3>Input</h3>
<p align="justify">The input consists of <var>T</var> test cases. The number of them (<var>T</var>) is given on the first line of the input file.
Each test case begins with a line containing two integers <var>C</var> and <var>R</var> (<var>3 &lt;= C,R &lt;= 1000</var>) indicating the number of columns and rows. Then exactly <var>R</var> lines follow, each containing <var>C</var> characters. These characters specify the labyrinth. Each of them is either a hash mark (<code>#</code>) or a period (<code>.</code>). Hash marks represent rocks, periods are free blocks. It is possible to walk between neighbouring blocks only, where neighbouring blocks are blocks sharing a&nbsp;common side. We cannot walk diagonally and we cannot step out of the labyrinth. 

</p><p align="justify">
The labyrinth is designed in such a way that there is exactly one path between any two free blocks. Consequently, if we find the proper hooks to connect, it is easy to find the right path connecting them.

</p><h3>Output</h3>
<p align="justify">Your program must print exactly one line of output for each test case. The line must contain the sentence "<code>Maximum rope length is <var>X</var>.</code>" where <var>X</var>is the length of the longest path between any two free blocks, measured in blocks.

</p><h3>Example</h3>
<pre><b>Sample Input:</b>
2
3 3
###
#.#
###
7 6
#######
#.#.###
#.#.###
#.#.#.#
#.....#
#######

<b>Sample output:</b>
Maximum rope length is 0.
Maximum rope length is 8.</pre>

<b>Warning: large Input/Output data, be careful with certain languages</b>