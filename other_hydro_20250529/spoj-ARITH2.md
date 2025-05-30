<p>While browsing aimlessly, Peter stumbled upon an old riddle he used to solve on his calculator when he was still young. It was the kind of a riddle where you punch in a bunch of numbers and operators into a simple pocket calculator and then turn it upside down to get the answer:</p>
<p><em>These come in many different sizes but they are always exactly one foot long. Answer: 103 * 103 * 5.</em></p>
<p><em>What are made of ice to keep people warm? Answer: 50 * 40 * 250 + 791. </em></p>
<p>After a few minutes he found a large amount of such riddles and full of excitement he went to solve them. He turned his computer screen upside down...</p>
<p>... only to find out that he does not have a reasonable calculator program installed on his computer.</p>
<h3>Problem specification</h3>
<p>You are given multiple sequences of button presses of a simple pocket calculator that consist of digits and arithmetic operators. For each such sequence find the number it would produce on a pocket calculator's display.</p>
<p>Note that the pocket calculator evaluates the operators in the order in which they are given. (i.e., there is no operator precedence.) Assume that the display of the calculator is large enough to show the result, and that its memory is sufficient to store all intermediate results.</p>
<h3>Input specification</h3>
<p>The first line of the input file contains an integer T specifying the number of test cases. Each test case is preceded by a blank line.</p>
<p>Each test case represents one sequence of button presses for a pocket calculator. The sequence consists of non-negative integers and arithmetic operators and ends with an equal sign. It may also contain spaces to improve readability.</p>
<p>The operator / represents integer division, rounded down. You may assume that no test case contains division by zero and that in all test cases all intermediate results are non-negative.</p>
<p><em>Tip:</em> <strong>long long int</strong> in C/C++, <strong>long</strong> in Java or <strong>int64</strong> in Pascal is enough for this problem.</p>
<h3>Output specification</h3>
<p>For each sequence from the input file output the number that would be displayed on the calculator.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4

1 + 1 * 2 =

29 / 5 =

103 * 103 * 5 =

50 * 40 * 250 + 791 =

<strong>Output:</strong>
4
5
53045
500791
</pre>
<h3>Hint</h3>
<p>The first test case shows that there is no operator precedence.</p>
<p>The second one shows that integer division always rounds down.</p>
<p>The last two outputs are the answers to the two riddles in the problem statement: "shoes" (53045 upside down), and "igloos"(500791 upside down).</p>