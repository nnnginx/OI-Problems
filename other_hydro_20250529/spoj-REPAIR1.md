<p>Once upon a time, there was a famous university called Famous University. As thousands of students studied and lived in FU, a gigantic residential building was built, which is called 'B37'. All students lived in B37 happily.</p>
<p>After decades, FU is still as famous as it had been in the past; however, the students living in it are now unhappy, because B37 is too old. Although the door of the building looks fine, it can be easily broken when being opened by some careless student too forcefully.</p>
<p>So, Blue Mary, the accommodation officer of B37, is facing an extremely serious problem.</p>
<p>With some mysterious methods, Blue Mary has predicted that exactly <em>N</em> students will enter or exit B37 during the next term. Unfortunately she doesn't know who the careless ones are, so she assumes that every student opening the door has a probability of <em>P</em> percent to be a careless one. When the door is broken by some careless guy, Blue Mary may repair it immediately or after some time, with a cost of <em>A</em> yuan. Unfortunately when a student goes through the door and finds it already broken and not repaired, she will report it to the headmaster, and Blue Mary will be subject to a fine of <em>B</em> yuan. The door is in good condition before the term begins, and will be repaired by the university after the term ends, so Blue Mary can leave the door unrepaired at the end of the term.</p>
<p>Being good at mathematics, Blue Mary has made a strategy, to decide when to and when not to repair the door, in order to minimize her expense.</p>
<p>Please write a program to calculate the expectation of her expense.</p>
<h3>Input</h3>
<p>The input consists of multiple test cases, the number of them is about 200000.</p>
<p>For each test case, there is one line containing four non-negative integers <em>N</em>, <em>P</em>, <em>A</em>, <em>B</em> described as above, with 0&lt;=<em>N</em>&lt;=100000, 0&lt;=<em>P</em>&lt;=100, 0&lt;=<em>A</em>&lt;=100, 0&lt;=<em>B</em>&lt;=100.</p>
<p>End of input is indicated by a line consisting of four zeros.</p>
<h3>Output</h3>
<p>For each test case, output one line containing the expectation of Blue Mary's minimal expense. We accept solutions with absolute error less than 10<sup>-4</sup>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10 100 0 1
10 100 1 0
2 50 2 1
0 0 0 0

<strong>Output:</strong>
0.0000
0.0000
0.5000
</pre>
<h3>Hint</h3>
<p>In the first sample, the door will be broken every time it is opened, but repairing is free, so just repair it every time.</p>
<p>In the second sample, nothing will be fined, so just leave the door unrepaired.</p>
<p>In the last sample, if the door is broken by the first student, Blue Mary will be fined 1 yuan, otherwise she doesn��t need to pay anything.</p>