<p>
Many problems arising in practical applications may be stated as <i>optimization problems</i>. Usually it is necessary to maximize or minimize so called <i>criterion function</i> taking into account some <i>constraints</i>.

</p><p>
Let¡¯s consider a trigonometric optimization problem. It is necessary to maximize or to minimize criterion function <b>F<sub>1</sub>(x) + F<sub>2</sub>(y) + F<sub>3</sub>(z)</b> with constraint <b>x + y + z = S</b>, where <b>x</b>, <b>y</b>, <b>z</b> ¨C variables, <b>S</b> ¨C parameter, <b>x</b>, <b>y</b>, <b>z</b>, <b>S</b> - natural numbers.  Each of the functions <b>F<sub>1</sub></b>, <b>F<sub>2</sub></b> and <b>F<sub>3</sub></b> is a trigonometric function <b><i>sin</i></b> or <b><i>cos</i></b>.

</p><p>
You need to write a program which solves the <i>trigonometric optimization</i> problem.

</p><h3>Input</h3>
<p>
The first line of the input data contains integer <b>T</b> (1 ¡Ü <b>T</b> ¡Ü 65) - the number of testcases. Then the descriptions of <b>T</b> testcases follow.
</p><p>
The description of each testcase consists of <i>5</i> lines. The first line describes function <b>F<sub>1</sub></b> and contains either <b>sin</b> or <b>cos</b>. The second and the third lines describe functions <b>F<sub>2</sub></b> and <b>F<sub>3</sub></b> respectively and have the same format as the first line. Next, the fourth line contains either <b>min</b> or <b>max</b>. If the line contains <b>min</b> than it is necessary to minimize <i>criterion function</i>, otherwise it is necessary to maximize <i>criterion function</i>. Finally, the fifth line contains parameter <b>S</b> value (3 ¡Ü <b>S</b> ¡Ü 1 000 000).

</p><h3>Output</h3>
<p>For each testcase you should output one line into the output data. This line should contain one real number ¨C the found value of the <i>criterion function</i>. Absolute error of your answer must not exceed <b>10<sup>-10</sup></b>.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
sin
cos
sin
max
10

<b>Output:</b>
2.7787651403
</pre>