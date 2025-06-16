<p>
A set <b>S</b> of positive integers is called <i>strongly triple-free</i> if, for any integer <b>x</b>, the sets {<b>x</b>, 2<b>x</b>}
and {<b>x</b>, 3<b>x</b>} are not subsets of <b>S</b>. Let's define <b>F(n)</b> as a number of strongly triple-free subsets of {1, 2, ..., <b>n</b>},
where <b>n</b> is a natural number.

</p><p>
You need to write a program which being given a number <b>n</b> calculates the number <b>F(n)</b> modulo 1 000 000 001.

</p><h3>Input</h3>
<p>
The first line of input contains integer <b>T</b> (1 ¡Ü <b>T</b> ¡Ü 500) - the number of testcases. Then descriptions of <b>T</b> testcases follow.

</p><p>
The description of the testcase consists of one line. The line contains an integer number <b>n</b> (1 ¡Ü <b>n</b> ¡Ü 100 000).

</p><h3>Output</h3>
<p>
For each testcase in the input your program should output one line. This line should contain one integer number which
is the number <b>F(n)</b> modulo 1 000 000 001.

</p><h3>Example</h3>

<pre><b>Input:</b>
5
3
1
10
20
39

<b>Output:</b>
5
2
198
43776
971827200
</pre>