<p>All the buildings in the east district of Byteburg were built in accordance with the old arbitecture: they stand next to each other with no spacing inbetween. Together they form a very long chain of buildings of diverse height, extending from east to west.</p>
<p>The mayor of Byteburg, Byteasar, has decided to have the north face of the chain covered with posters. Byteasar ponders over the minimum number of posters sufficient to cover the whole north face. The posters have rectangular shape with vertical and horizontal sides. They cannot overlap, but may touch each other, i.e. have common points on the sides. Every poster has to entirely adjoin the walls of certain buildings and the whole surface of the north face has to be covered.</p>
<p> </p>

<h1>Task</h1>
<p>Write a programme that:</p>
<ul>
<li>reads the description of buildings from the standard input,</li>
<li>determines the minimum number of posters needed to entirely cover their north faces,</li>
<li>writes out the outcome to the standard output.</li>
</ul>
<p>&nbsp;</p>

<h1>Input</h1>
<p>The first line of the standard input contains one integer N&nbsp;(1 &lt;= N &lt;= 250000), denoting the number of buildings the chain comprises of. Each of the following N&nbsp;lines contains two integers D<sub>i</sub>&nbsp;and W<sub>i</sub>&nbsp;(1 &lt;= D<sub>i</sub>, W<sub>i </sub>&lt;=10<sup>9</sup>), separated by a single space, denoting respectively the length and height of the i-th&nbsp;building in the row.</p>
<p>&nbsp;</p>

<h1>Output</h1>
<p>The first and only line of the standard output should contain one integer, the minimum number of rectangular posters that suffice to cover the north faces of the buildings.</p>
<p>&nbsp;</p>

<h1>Example</h1>
<pre><b><u>Input</u></b>
5
1 2
1 3
2 2
2 5
1 4

<b><u>Output</u></b>
4
</pre>