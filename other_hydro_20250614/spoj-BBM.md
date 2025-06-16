<h3>Warning:</h3>
<p> Source code size limit is 2048B (half is enough) and time limit could not allow all language to get AC ; I got AC in 0.41s with language C. (Timing edited, 2017-02-11, after compiler changes).
The <b>main</b> difficulty of the problem is to manage efficiently the given precomputed
values <b>and</b> the memory available, in the given time. Have fun ;-)
</p>


<h3>The March</h3>
<p>Leo invited all his friends to a giant meeting for peace in byteland.
All people came in bus which were all full.<br>
Last year, they were <a href="http://www.spoj.com/problems/TMB/">thousands of people</a>.
As Leo like structured things, he thought to form groups.
<br>
Two years ago, all the ways to form homogeneous team with the 4 people (A,B,C,D) were : </p>
<pre>{{A,B,C,D}} : one team of 4 (one way),
{{A}, {B}, {C}, {D}} : four 'teams' of 1 (one way more),
{{A,B}, {C,D}} or {{A,C}, {B,D}} or {{A,D}, {B,C}} : two teams of 2 (3 ways more).
</pre>
<p>
for a total of 5 ways. But this year many more people are awaited.<br>
As the answer should not fit in a 64-bit container, you should give your answer modulo M7=1000000007.</p>

<h3>Input</h3>
<p>
The input starts with 2^12 useful precomputed values:
 factorial(i) MOD M7 for i in [0 ; 2^30[ with a step of 2^18, each one on one line.<br>
The input continues with the number T of test cases in a single line.<br>
In each of the next T lines there are two integers : N, K.<br>
N is the quantity of bus that came to the meeting.<br>
K is the common capacity of each bus.</p>

<h3>Output</h3>
<p>
For each test case, your task is to calculate the number of ways people
can form homogeneous teams.<br>
</p>

<h3>Example</h3>
<pre><b>Input:</b>
1            &lt;--- 0! mod M7
639926614    &lt;--- (2^18)! mod M7
[...]        ( 4093 lines more)
0            &lt;--- (2^30 - 2^18)! mod M7
3
2 2
1 6
2 3

<b>Output:</b>
5
27
27
</pre>


<h3>Constraints</h3>
<pre>0 &lt; T ¡Ü 300
0 &lt; K ¡Ü 30000
0 &lt; N ¡Ü 30000
</pre>
<p>Uniform-random input in the range.</p>