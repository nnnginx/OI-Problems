<p>The Industrial Computer Processor Company offers very fast, special purpose processing units tailored to customer needs. Processors of the a-C-m family (such as the 1-C-2 and the 5-C-3) have an instruction set with only two different operations:</p>
<p style="padding-left: 30px;"><em>A add a</em></p>
<p style="padding-left: 30px;"><em>M multiply by m</em></p>
<p>The processor receives an integer, executes a sequence of A and M operations (the program) that modiﬁes the input, and outputs the result. For example, the 1-C-2 processor executing the program <span style="font-family: andale mono,times;">AAAM</span> with the input 2 yields the output 10 (the computation is 2 → 3 → 4 → 5 → 10), while the 5-C-3 processor yields 51 with the same program and input (2→ 7 → 12 → 17 → 51).</p>
<p>You are an <span style="font-family: symbol;">a-<strong>C</strong>-m</span> programmer assigned to a top secret project. This means that you have not been told the precise computation your program should perform. But you are given particular values <em>p</em>, <em>q</em>, <em>r</em>, and <em>s</em> and the following conditions:</p>
<p style="padding-left: 30px;">1. The input is guaranteed to be a number between <em>p</em> and <em>q</em>.</p>
<p style="padding-left: 30px;">2. The output must be some number between <em>r</em> and <em>s</em>.</p>
<p>Given an <span style="font-family: symbol;">a-<strong>C</strong>-m</span> processor and the numbers <em>p</em>, <em>q</em>, <em>r</em>, and <em>s</em>, your job is to construct the shortest <span style="font-family: symbol;">a-<strong>C</strong>-m</span> program which, for every input <em>x</em> such that <em>p</em> ≤ <em>x</em> ≤ <em>q</em>, yields some output <em>y</em> such that <em>r</em> ≤ <em>y</em> ≤ <em>s</em>. If there is more than one program of minimum length, choose the one that come ﬁrst lexicographically, treating each program as a string of <span style="font-family: andale mono,times;">As</span> and <span style="font-family: andale mono,times;">Ms</span>.</p>
<h3>Input</h3>
<p>The input contains several test cases. Each test case is given by a line with the six integers <em>a</em>, <em>m</em>, <em>p</em>, <em>q</em>, <em>r</em>, and <em>s</em> as described above (1 ≤<em> a, m, p, q, r, s</em> ≤ 10<sup>9</sup>, <em>p</em> ≤ <em>q</em> and <em>r</em> ≤ <em>s</em>).</p>
<p>The last test case is followed by a line with six zeros.</p>
<h3>Output</h3>
<p>For each test case, display its case number followed by the best program as described above. Display the word “<span style="font-family: andale mono,times;">empty</span>” if the best program uses no operations. Display the word “<span style="font-family: andale mono,times;">impossible</span>” if there is no program meeting the speciﬁcations.</p>
<p>Display the program as a sequence of space-separated strings, alternating between strings of the form “<span style="font-family: andale mono,times;">nA</span>” and strings of the form “<span style="font-family: andale mono,times;">nM</span>”, where <em>n</em> &gt; 0. Strings of the former type indicate <em>n</em> consecutive <span style="font-family: andale mono,times;">A</span> operations, and strings of the latter type indicate <em>n</em> consecutive <span style="font-family: andale mono,times;">M</span> operations.</p>
<p>Follow the format of the sample output.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1 2 2 3 10 20<br>1 3 2 3 22 33<br>3 2 2 3 4 5<br>5 3 2 3 2 3<br>0 0 0 0 0 0 <br>
<strong>Output:</strong>
<pre>Case 1: 1A 2M<br>Case 2: 1M 2A 1M<br>Case 3: impossible<br>Case 4: empty</pre>
</pre>