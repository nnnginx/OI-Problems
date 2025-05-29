<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/CIJEVI/en/">English</a></td>
<td width="50%"><a href="/problems/CIJEVI/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p> </p>
<p>To help design the new gas pipeline which will be used to deliver Russian gas to Croatia, Zagreb and Moscow are using the computer game Pipe Mania. In the game, Europe is divided into R rows and C columns. Each cell can be empty or contain one of the seven basic pipeline building blocks:</p>
<p><img src="./21830/file/eyZujfyU.png" alt="" width="342" height="206"></p>

<p>Gas flows from Moscow to Zagreb. Gas can flow in either direction through the building blocks. Block '+' is special in that gas must flow in two directions (one vertical, one horizontal), as in the following example:</p>
<p><img src="./21830/file/yIiyEiGm.png" alt="" width="384" height="230"></p>

<p>Work on the new pipeline had already started when it was found that malicious hackers got hold of the plan and erased exactly one building block from the plan i.e. replaced it with an empty cell.</p>
<p>Write a program that determines where the block was erased from and what type it was.</p>
<h3>Input</h3>
<p>The first line contains two integers R and C, the dimensions of Europe (1 ¡Ü R, C ¡Ü 25)</p>
<p>The following R lines contain the plan, each consisting of exactly C characters. The characters are:</p>
<ul>
<li>Period ('.'), representing an empty cell;</li>
<li>The characters '|' (ASCII 124), '-', '+', '1', '2', '3', '4', representing the building block types;</li>
<li>The letters 'M' and 'Z', representing Moscow and Zagreb. Each of these will appear exactly once in the plan.</li>
</ul>
<p>The flow of gas will be uniquely determined in the input; exactly one building block will be adjacent to each of Moscow and Zagreb. Additionally, the plan will not have redundant blocks i.e. all blocks in the plan must be used after the missing block is added.</p>
<p>The input will be such that a solution will exist and it will be unique.</p>
<h3>Output</h3>
<p>Output the row and column of the erased block, and the type of the block (one of the seven characters as in the input).</p>
<h3>Example</h3>
<pre>Input
3 7
.......
.M-.-Z.
.......
Output
2 4 -


Input
3 5
..1-M
1-+..
Z.23.

Output
2 4 4


Input
6 10
Z.1----4..
|.|....|..
|..14..M..
2-+++4....
..2323....
..........

Output
3 3 |
</pre>
<p></p>