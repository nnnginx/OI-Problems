<p>Years ago, there was a really bad craft/hobby called <i>paint-by-numbers</i>: you were given a line drawing, with numbers in each enclosed region, and the number corresponded to a particular colour. An example is shown below (unsolved on the left; solved on the right):</p><p>
<img src="/content/nneonneo:PNTBYNUM_squnsolved.jpg" height="220"><img src="/content/nneonneo:PNTBYNUM_sqsolved.jpg" height="220"><br>(images from <a href="http://thislife.org/paintings/">ThisLife.org</a>)
</p><p>The problem you have to solve is much more linear, in a way.
</p><p>You will be given an <i>n</i>-by-<i>m</i> grid (1 ¡Ü <i>n, m</i> ¡Ü 32) which you will "colour" in with either a dot ('.') or a star ('*').
</p><p>Of course, the grid will not be specified in the usual paint-by-numbers way, since this would be too easy.
</p><p>Instead, you will you have to infer which cells are blank and which contain a star. The only information you will be given are a collection of <i>n + m</i> sequences of numbers, one sequence for each row and column. The sequence will indicate the size of each continuous block of stars. There must be at least one dot between two consecutive blocks of stars.
</p><p>An example is shown below (which is supposed to look fish-like):</p><p><img src="/content/nneonneo:PNTBYNUM_example.png" height="180">
</p><p>You may notice that some paint-by-number patterns are not uniquely solvable. For this problem, you may assume that <i>any</i> solution which satisfies the specification is correct.
</p><h3>Input</h3> <p>Input begins with a line with the number of test cases. Each test case consists of a total of <i>n + m</i> + 2 lines. The first line of the test case consists of an integer <i>n</i> (1 ¡Ü <i>n</i> ¡Ü 32), the number of rows. The second line consists of an integer <i>m</i> (1 ¡Ü <i>m</i> ¡Ü 32), the number of columns. On the next <i>n</i> lines, there will be sequences which describe each of the <i>n</i> rows (from top to bottom). Each line will contain some positive integers, with a space between adjacent integers, and the sequence will terminate with the integer 0. On the next <i>m</i> lines describe the <i>m</i> columns (from left to right), the same format as the rows are specified.
</p><h3>Output</h3> <p>Output consists of <i>n</i> lines for each corresponding test case, each line composed of <i>m</i> characters, where each character is either a dot ('.') or a star ('*'). Separate test cases with a blank line.
</p><h3>Example</h3>
<pre><b>Input:</b>
2
4
7
2 2 0
5 0
5 0
2 2 0
1 1 0
1 1 0
2 0
2 0
4 0
4 0
2 0
4
4
2 1 0
3 0
3 0
1 1 0
4 0
3 0
3 0
1 0

<b>Output:</b>
**..**.
..*****
..*****
**..**.

**.*
***.
***.
*.*.
</pre>