<p>Little Ben had just learned different bases in math. He learned very quickly how to add and subtract in multiple bases, so his teacher provided him with a worksheet to work on. Each section provided a different base and gave an example.</p>
<p>Unfortunately, Little Ben's teacher forgot to write what base each question was in! Please help Little Ben do his homework; he'll be very grateful!</p>
<p style="text-align: center;"><strong>Input</strong></p>
<p>The first line of input contains an integer <code>n</code> (1 ¡Ü n &lt; 36) that indicates the amount of sections (test cases). Each test case is as follows:</p>
<pre><span style="font-family: 'courier new', courier;">A - B = C
I
X1 op Y1 =
X2 op Y2 =
...
XI op YI =</span></pre>
<p>where <code>A - B = C</code> is the correct example, <code>I</code> (1 ¡Ü I ¡Ü 1000) is the number of questions in that section, <code>Xi</code> and <code>Yi</code> are the operands of each problem (<code>Xi</code> = |<code>Xi</code>|, <code>Yi</code> = |<code>Yi</code>|), and <code>op</code> is either + or -, denoting addition or subtraction.</p>
<p style="text-align: center;"><br> <strong>Output</strong></p>
<p>Your program should output in the following format:</p>
<pre><span style="font-family: 'courier new', courier;">SECTION 1 (BASE b)<br>  X1 op Y1 = Z1<br>  X2 op Y2 = Z2<br>  ...<br>  Xi op Yi = Zi<br>SECTION 2 (BASE b)<br>  X1 op Y1 = Z1<br>  X2 op Y2 = Z2<br>  ...<br>  Xi op Yi = Zi<br>...<br>SECTION N (BASE b)<br>  X1 op Y1 = Z1<br>  X2 op Y2 = Z2<br>  ...<br>  Xi op Yi = Zi</span></pre>
<p>where <code>Zi</code> is the solution to <code>Xi op Yi</code>, and <code>b</code> is the base used. (2 ¡Ü b ¡Ü 36). <em>If the base is ambiguous, use the smallest base for which the example is correct and the questions are valid.</em>&nbsp;You may assume all solutions fit inside a 64-bit integer and that each base will appear at most once.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><strong>Example</strong></p>
<p><strong>Input:</strong></p>
<pre><span style="font-family: 'courier new', courier;">4
110 - 101 = 1
2
1111111 + 1 =
100 - 1 =
177 + 1 = 200
2
7712347 + 7 =
11111 + 7777 =
ZAP + DZ = ZOO
1
E + PI =
10 + 1 = 11
1
5 + 5 =</span></pre>
<p><strong>Output:</strong></p>
<pre><span style="font-family: 'courier new', courier;">SECTION 1 (BASE 2)
  1111111 + 1 = 10000000
  100 - 1 = 11
SECTION 2 (BASE 8)
  7712347 + 7 = 7712356
  11111 + 7777 = 21110
SECTION 3 (BASE 36)
  E + PI = PW
SECTION 4 (BASE 6)
  5 + 5 = 14</span></pre>
<p style="text-align: center;"><strong>Notes: </strong></p>
<ul>
<li>large input/output data, be careful with certain languages</li>
<li>Tricky input/output; please read problem statement carefully</li>
</ul>