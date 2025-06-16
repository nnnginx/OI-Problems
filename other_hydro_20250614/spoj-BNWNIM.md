<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/BNWNIM/en/">English</a></td> 
<td width="50%"><a href="/problems/BNWNIM/vn/">Vietnamese</a></td> 
</tr></tbody></table>




<p>Black-White-Nim is played as follows. There are one or more horizontal rows, each containing several black and white beads. Two players take turns removing beads until there are none left. During each turn, a player must remove one or more consecutive beads from the left end of a single row. The removed beads must contain either no black beads or exactly one black bead. If one black bead is removed, that bead must be the rightmost of the removed beads. The player who takes the last turn wins.</p>
<p>Given the number of black and white beads in each rows. The order of beads in each row is randomly generated at the beginning of the game. Each distinct row ordering is equally likely. Black beads are indistinguishable from one another, and white beads are indistinguishable from one another. Output the probability that the first player will win the game assuming that both players follow an optimal strategy.</p>

<h3>Input</h3>
<p>The first line of input contains a number representing the number of tests.</p> 
<p>Each test cases contains three lines, the first line contains N representing the number of rows.</p> 
<p>The second line contains N numbers, representing the number of black beads in each row. There will be at most 100 black beads in each row. </p>
<p>The third line contains N numbers, representing the number of white beads in each row. There will be at most 100 white beads in each row. There will be at least one beads in each row.</p>

<h3>Output</h3>
<p>For each test case, output a line contains a float-number, representing the answer. It must be printed with exactly six decimal places.</p>

<h3>Example</h3>

<pre><b>Input:</b>
4
1
0
2
1
2
0
1
2
2
2
2 5
2 0

<b>Output:</b>
1.000000
0.000000
0.666667
0.666667
</pre>

<h3>Constraints</h3>
<p>Dataset 1: N �� 50. Time limit: 5s</p>