<p>You are given a sequence of <em>n</em> numbers <em>a</em><sub>0</sub>, …, <em>a</em><sub><em>n</em>−1</sub>. A cyclic shift by <em>k</em> positions (0 ≤ <em>k</em> ≤ <em>n</em>−1) results in the following sequence: <em>a</em><sub><em>k</em></sub>, <em>a</em><sub><em>k</em>+1</sub>, …, <em>a</em><sub><em>n</em>−1</sub>, <em>a</em><sub>0</sub>, <em>a</em><sub>1</sub>, …, <em>a</em><sub><em>k</em>−1</sub>. How many of the <em>n</em> cyclic shifts satisfy the condition that the sum of the first <em>i</em> numbers is greater than or equal to zero for all <em>i</em> with 1 ≤ <em>i</em> ≤ <em>n</em>?</p>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Input</span></span></strong></p>
<p>Each test case consists of two lines. The first contains the number <em>n</em> (1 ≤ <em>n</em> ≤ 10<sup>6</sup>), the number of integers in the sequence. The second contains <em>n</em> integers <em>a</em><sub>0</sub>, …, <em>a</em><sub><em>n</em>−1</sub> (−1000 ≤ <em>a</em><sub><em>i</em></sub> ≤ 1000) representing the sequence of numbers. The input will finish with a line containing 0.</p>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Output</span></span></strong></p>
<p>For each test case, print one line with the number of cyclic shifts of the given sequence which satisfy the condition stated above.</p>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Sample Input</span></span></strong></p>
<pre class="verbatim">3
2 2 1
3
-1 1 1
1
-1
0
</pre>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Sample Output</span></span></strong></p>
<pre class="verbatim">3
2
0
</pre>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Adrian Kuegel</em></blockquote>