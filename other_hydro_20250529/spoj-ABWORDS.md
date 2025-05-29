<p align="justify">Every sequence of small letters a and b (also the empty sequence) is called an ab-word. If <i>X</i> = [<i>x</i><sub>1</sub>, ..., <i>x</i><i><sub>n</sub></i>] is an ab-word and <i>i</i>, <i>j</i> are integers such that 1 &lt;= <i>i</i> &lt;= <i>j</i> &lt;= <i>n</i> then <i>X</i>[<i>i</i>..<i>j</i>] denotes the subword of <i>X</i> consisting of the letters <i>x</i><i><sub>i</sub></i>, ..., <i>x</i><i><sub>j</sub></i>. We say that an ab-word <i>X</i> = [<i>x</i><sub>1</sub>..<i>x</i><i><sub>n</sub></i>] is nice if it has as many letters a as b and for all <i>i</i> = 1, ..., <i>n</i> the subword <i>X</i>[1..<i>i</i>] has at least as many letters a as b.</p>
<p align="justify">Now, we give the inductive definition of the similarity between nice ab-words.</p>
<div align="justify">
<ul>
        <li align="justify">Every two empty ab-words (i.e. words with no letters) are similar</li>
        <li align="justify">Two non-empty nice ab-words <i>X</i> = [<i>x</i><sub>1</sub>, ..., <i>x</i><i><sub>n</sub></i>] and <i>Y</i> = [<i>y</i><sub>1</sub>, ..., <i>y</i><i><sub>m</sub></i>] are similar if they have the same length (<i>n</i> = <i>m</i>) and one of the following conditions if fulfilled: </li>
        <ol>
                <li align="justify"><i>x</i><sub>1</sub> = <i>y</i><sub>1</sub>, <i>x</i><i><sub>n</sub></i> = <i>y</i><i><sub>n</sub></i> and <i>X</i>[2..<i>n</i>-1] and <i>Y</i>[2..<i>n</i>-1] are similar ab-words and they are both nice;</li>
                <li align="justify">there exists <i>i</i>, 1 &lt;= <i>i</i> &lt;= <i>n</i>, such that <i>X</i>[1..<i>i</i>], <i>X</i>[<i>i</i>+1..<i>n</i>] are nice ab-words and</li>
                <ol type="a">
                        <li align="justify"><i>Y</i>[1..<i>i</i>], <i>Y</i>[<i>i</i>+1..<i>n</i>] are nice ab-words and <i>X</i>[1..<i>i</i>] is similar to <i>Y</i>[1..<i>i</i>] and <i>X</i>[<i>i</i>+1..<i>n</i>] is similar to <i>Y</i>[<i>i</i>+1..<i>n</i>], or</li>
                        <li align="justify"><i>Y</i>[1..<i>n</i>-i], <i>Y</i>[<i>n</i>-<i>i</i>+1..<i>n</i>] are nice ab-words and <i>X</i>[1..<i>i</i>] is similar to <i>Y</i>[<i>n</i>-<i>i</i>+1..<i>n</i>] and <i>X</i>[<i>i</i>+1..<i>n</i>] is similar to <i>Y</i>[1..<i>n</i>-<i>i</i>].</li>
                </ol>
        </ol>
</ul>
</div>
<p align="justify">A <b>level of diversity</b> of a non-empty set <i>S</i> of nice ab-words is the maximal number of ab-words that can be chosen from <i>S</i> in such a way that for each pair <i>w</i><sub>1</sub>,<i>w</i><sub>2</sub> of chosen words, <i>w</i><sub>1</sub> is not similar to <i>w</i><sub>2</sub>.</p>


<h3>Task</h3>
<p align="justify">Write a program that for each test case:</p>
<div align="justify">
<ul align="justify">
        <li align="justify">reads elements of <i>S</i> from standard input;</li>
        <li align="justify">computes the level of diversity of the set <i>S</i>;</li>
        <li align="justify">writes the result to standard output.</li>
</ul></div>

<h3>Input</h3>
<p align="justify">The number of test cases <i>t</i> is in the first line of input, then <i>t</i> test cases follow separated by an empty line.</p>
<p align="justify">In the first line of a test case there is a number <i>n</i> of elements of the set <i>S</i>, 1 &lt;= <i>n</i> &lt;= 1000; in the following <i>n</i> lines there are elements of the set <i>S</i>, i.e. nice ab-words (one word in each line); the first letter of every ab-word is the first symbol in line and there are no spaces between two consecutive letters in the word; the length of every ab-word is an integer from the range [1..200]. </p>

<h3>Output</h3>
<p align="justify">For each test case your program should output one line with one integer - the level of diversity of <i>S</i>. </p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
3
aabaabbbab
abababaabb
abaaabbabb

<b><tt>Sample output:</tt></b>
2
</pre>