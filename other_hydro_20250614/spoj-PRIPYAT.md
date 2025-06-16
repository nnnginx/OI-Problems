<p>Pripyat is an abandoned city in Ukraine. On April 27, 1986, the whole population of Pripyat was evacuated because of the Chernobyl nuclear power plant accident.</p>
<p>Today (April 26) is the 32nd anniversary of the Chernobyl nuclear disaster, and Duck plans to visit Chernobyl to know more about this disaster. He has a list of <strong>N</strong> must-visit places in Pripyat, with its excitation level <strong>EXC</strong>, time required to visit&nbsp;<strong>VT</strong> and radiation level <strong>RL</strong>. Of course, sometimes it is impossible to visit all places because of limited visiting time and the danger of radiation. Given his maximum of available time to visit&nbsp;<strong>MVT</strong> and tolerance to radiation level <strong>TRL</strong>, can you help him to select some places to visit so that the total EXC is maximized and the VT and RL are less than or equal to the given limit.&nbsp;</p>
<p>Based on your finding, given a matrix <strong>MX</strong> showing some barriers that are not allowed to pass through, Duck's hotel location and all must-visited places' location, determine the minimum distance to be moved to visit all the selected places starting from his hotel location. Duck can only move to adjacent cells that share one edge horizontally or vertically, and he can only visit the selected place once. That is, he cannot pass through the selected place twice or more. Also, he cannot pass through the unselected places.</p>
<h3>Input</h3>
<p>The first line is the number of test cases <strong>T</strong>. (1 &lt;= T &lt;= 25)</p>
<p>For each test case, it starts with two integers: number of must-visit places <strong>N</strong> (1 &lt;= N &lt;= 20) and his maximum of available time to visit <strong>MVT</strong> (1 &lt;= MVT &lt;= 100) , and one real number: tolerance to radiation level <strong>TRL</strong>. (0.01 &lt;= TRL &lt;= 10)</p>
<p>Following N lines, each showing ith place's information, consisting of two integers: excitation level <strong>EXC</strong> (1 &lt;= EXC &lt;= 100) and time required to vistit <strong>VT</strong> (1 &lt;= VT &lt;= 100), and one real number: radiation level <strong>RL</strong>. (0.01 &lt;= RL &lt;= 10)</p>
<p>After that, a line consists of two integers: number of rows of the matrix <strong>R</strong>, and number of colunms of the matrix <strong>C</strong>. (1 &lt;= R, C &lt;= 50)</p>
<p>Next R lines, each has C characters, representing the map of Pripyat <strong>MX</strong>. '+' means hotel location, '.' means available cells Duck can walk, '#' means barriers Duck cannot pass through, and N consecutive upper letters counting from A corresponding to ith place, eg. A = 1 (N<sub>1</sub>), B = 2 (N<sub>2</sub>) and so on up to T = 20 (N<sub>20</sub>).</p>
<p>It is guranteed that R * C &gt;= N + 1, and all real numbers are with at most two digits after the decimal point.</p>
<h3>Output</h3>
<p>One integer indicating the minimum distance to be moved to visit all the selected places starting from his hotel location. If there are multiple combinations, choose the first in alphabetical order.</p>
<p>If no places are selected, output '0'; if it is impossible to visit all selected places, output '-1' (without quotes).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2

5 8 0.8
3 1 0.04
9 9 0.1
4 2 0.12
10 5 0.2
7 2 0.02
8 10
.B...#....
...#.+.#.C
..A.....#.
..##.##.##
....#..E..
#.........
#.....##..
#..#..D...

5 18 1.6
8 6 0.04
9 9 0.1
4 5 0.12
10 5 0.2
3 1 0.02
8 10
.B...#....
...#.+.#..
........#.
..########
....#...DE
#.......##
#.##..###A
...#..C...

<strong>Output:</strong>
17
-1
</pre>
<h3>Explanation</h3>
<p>In test case 1, A, D, E are selected and the minimum distance to visit all of them from '+' is 17.</p>
<p>In test case 2, A, C, D, E are selected. But D blocks E and C blocks A, it is impossible to visit all selected places once only. Duck has to visit C twice or D twice.</p>