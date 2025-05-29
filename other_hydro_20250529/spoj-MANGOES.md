<p>Ranjith is very fond of mangoes. One fine sunny day, he goes to market to get some mangoes. In the market place, he finds <i>N</i> boxes (indexed from 1 to <i>N</i>), filled with mangoes kept infront of him. Each box indexed <i>i</i> is denoted by <i>b<sub>i</sub></i> and contains exactly <i>i</i> mangoes. The number of mangoes in <i>b<sub>i</sub></i> is denoted by <i>m<sub>i</sub></i> and <i>m_i</i> = <i>i</i>. Let <i>t<sub>i</sub></i> denotes the type of mangoes in box <i>b<sub>i</sub></i> (<i>t<sub>i</sub></i> is either "real" or "fake"). He can choose any box <i>b<sub>i</sub></i> (<i>i</i> &lt;= <i>N-2</i>), but he doesn't know if the box contains "real" mangoes or "fake" mangoes i.e. type of box <i>b<sub>i</sub></i>.
</p>

<p>
The type of mangoes in <i>b<sub>i</sub></i> depends on the number of mangoes in boxes <i>b<sub>i</sub></i>, <i>b<sub>i+1</sub></i>, <i>b<sub>i+2</sub></i>&nbsp;i.e. {<i>m<sub>i</sub></i>, <i>m<sub>i+1</sub></i>, <i>m<sub>i+2</sub></i>}. Mangoes in box <i>b<sub>i</sub></i> are "real" if for each pair of numbers taken from set {<i>m<sub>i</sub></i>, <i>m<sub>i+1</sub></i>, <i>m<sub>i+2</sub></i>}, Greatest common divisor(GCD) equals 1. Otherwise, "fake". Note that <i>t<sub>i</sub></i> is not defined for <i>i</i> = <i>N-1</i> and <i>i</i> = <i>N</i> and assumed to be "fake".&nbsp;
</p>

<p>
Given <i>N</i>, Ranjith wants to know the total number of "real" mangoes he will get from all boxes. As Ranjith cannot count beyond <i>N</i>, output the result modulo <i>N</i>.
</p>

<h3>Input</h3>
<p>Test File starts with number of test cases - <i>T</i>;</p>
<p><i>T</i> lines follows, each containing <i>N</i>, number of boxes.</p>

<h3>Output</h3>
<p>Output <i>T</i> lines Number of "real" mangoes Ranjith gets (modulo <i>N</i>) in each one of the <i>T</i> cases.</p>

<h3>Constraints</h3>
<p>
2 &lt; <i>N</i> &lt;= 10^8<br>
<i>T</i> &lt;= 10000
</p>

<h3>Example</h3>
<pre><b>Input:</b>
2
9
5

<b>Output:</b>
7
4</pre>