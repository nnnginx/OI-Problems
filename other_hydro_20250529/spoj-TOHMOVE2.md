<p>The easier version of this problem can be found <a href="http://www.spoj.com/problems/TOHMOVE1/">here</a>

</p><p>The Tower of Hanoi (also called the Tower of Brahma or Lucas' Tower and sometimes pluralized) is a mathematical game or puzzle. It consists of three rods and a number of disks of different sizes, which can slide onto any rod. The puzzle starts with the disks in a neat stack in ascending order of size on one rod, the smallest at the top, thus making a conical shape.</p>
<p>The objective of the puzzle is to move the entire stack to another rod, obeying the following simple rules:
</p><ol>
<li>Only one disk can be moved at a time.</li>
<li>Each move consists of taking the upper disk from one of the stacks and placing it on top of another stack.</li>
<li>No disk may be placed on top of a smaller disk.</li>
</ol><p></p>
<p>With 3 disks, the puzzle can be solved in 7 moves. The minimal number of moves required to solve a Tower of Hanoi puzzle is 2<sup>N</sup> − 1, where n is the number of disks.</p>

<p><i>The description is retrieved from Wikipedia</i></p><br>

<p>From the description above, AVM wants to know the <i>a</i><sup>th</sup> step of optimal solution. The set of Tower of Hanoi consists of <i>N</i> disks and 3 rods (A as the source rod, B as the spare rod, and C as the target rod).</p>

<h3>Input</h3>
<p>
The input file consists of several lines.
The first line contains a single number <i>T</i> representing the number of test cases.
The next <i>T</i> lines contains <i>N</i> and <i>a</i> representing the number of disk and the <i>a</i><sup>th</sup> move.
</p>

<h3>Output</h3>
<p>
The output file should contains <i>T</i> lines.
The <i>i</i>-th line should contain <i>P : A =&gt; C</i> , the <i>P</i><sup>th</sup> disk, the rod of <i>P</i><sup>th</sup> disk before the movement, and the rod of <i>P</i><sup>th</sup> disk after the movement.
</p>

<h3>Constraint</h3>
<p>1 &lt;= <i>T</i> &lt;= 1000<br>
1 &lt;= <i>N</i> &lt;= 50<br>
1 &lt;= <i>a</i> &lt;= 2<sup><i>N</i></sup> - 1</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
2 3
3 5
3 7

<b>Output:</b>
1 : B =&gt; C
1 : B =&gt; A
1 : A =&gt; C

</pre>

<h3>Explanation</h3>

The 2-disks Tower of Hanoi optimal solution is:
<pre>1 : A =&gt; B
2 : A =&gt; C
1 : B =&gt; C
</pre>
Therefore, the first test case answer is <pre>1 : B =&gt; C</pre>

The 3-disks Tower of Hanoi optimal solution is:
<pre>1 : A =&gt; C
2 : A =&gt; B
1 : C =&gt; B
3 : A =&gt; C
1 : B =&gt; A
2 : B =&gt; C
1 : A =&gt; C
</pre>
Therefore, the second test case answer is <pre>1 : B =&gt; A</pre> and the last test case answer is <pre>1 : A =&gt; C</pre>