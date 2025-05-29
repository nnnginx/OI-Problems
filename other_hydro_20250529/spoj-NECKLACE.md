<p>
There are <b>N</b> points marked on a surface, pair (<b>x<sub>i</sub></b>, <b>y<sub>i</sub></b>) is coordinates of a point number <b>i</b>.
Let's call a <i>necklace</i> a set of <b>N</b> figures which fulfills the following rules.

</p><p>
</p><ul>
<li>The figure <b>#i</b> consists of all such points (<b>x</b>, <b>y</b>) that (<b>x</b> - <b>x<sub>i</sub></b>)<i><sup>2</sup></i> + (<b>y</b> - <b>y<sub>i</sub></b>)<i><sup>2</sup></i> ¡Ü <b>r<sub>i</sub></b><i><sup>2</sup></i>, where <b>r<sub>i</sub></b> ¡Ý <i>0</i>.
</li><li>Figures <b>#i</b> and <b>#(i+1)</b> intersect (<i>1</i> ¡Ü <b>i</b> &lt; <b>N</b>).
</li><li>Figures <i>#1</i> and <b>#N</b> intersect.
</li><li>All the rest pairs of figures do not intersect.
</li></ul>

<p>
Write a program which takes points and constructs a necklace.

</p><h3>Input</h3>
<p>
First line of input contains an integer <b>t</b> (<i>1</i> ¡Ü <b>t</b> ¡Ü <i>45</i>), equals to the number of testcases. Then descriptions of <b>t</b>
testcases follow.

</p><p>
The first line of the description contains one integer number <b>N</b> (<i>2</i> ¡Ü <b>N</b> ¡Ü <i>100</i>).
Each of the next <b>N</b> lines contains two real numbers <b>x<sub>i</sub></b>, <b>y<sub>i</sub></b>  (<i>-1000</i> ¡Ü <b>x<sub>i</sub></b>, <b>y<sub>i</sub></b> ¡Ü <i>1000</i>), separated by one space. It is guaranteed that at least one necklace exists for each testcase.

</p><h3>Output</h3>
<p>
For each testcase your program should output exactly <b>N</b> lines. A line <b>#i</b> should contain real number <b>r<sub>i</sub></b> (<i>0</i> ¡Ü <b>r<sub>i</sub></b> &lt; <i>10000</i>).
To avoid potential accuracy problems, a checking program uses the following rules.

</p><p>
</p><ul>
<li>Figures <b>#i</b> and <b>#j</b> definitely do not intersect if <b>r<sub>i</sub></b> + <b>r<sub>j</sub></b> ¡Ü <b>d<sub>ij</sub></b> - <i>10<sup>-5</sup></i>. 
</li><li>Figures <b>#i</b> and <b>#j</b> definitely intersect if <b>d<sub>ij</sub></b> + <i>10<sup>-5</sup></i> ¡Ü <b>r<sub>i</sub></b> + <b>r<sub>j</sub></b>.
</li><li>The case when <b>d<sub>ij</sub></b> - <i>10<sup>-5</sup></i> &lt; <b>r<sub>i</sub></b> + <b>r<sub>j</sub></b> &lt; <b>d<sub>ij</sub></b> + <i>10<sup>-5</sup></i> is decided in favour of a contestant.
</li><li><b>d<sub>ij</sub></b> equals <i>sqrt</i>((<b>x<sub>i</sub></b> - <b>x<sub>j</sub></b>)<i><sup>2</sup></i> + (<b>y<sub>i</sub></b> - <b>y<sub>j</sub></b>)<i><sup>2</sup></i>) in the rules above.
</li></ul>

<h3>Example</h3>

<pre><b>Input:</b>
1
4
0 0
10 0
10 10
0 10

<b>Output:</b>
7
7
7
7

</pre>