<p>After giving a heartwarming, inspirational speech to the sorority sisters of Delta Gamma at the University of Maryland, Michael Shannon was assaulted on the street by an armed mathematician, who defined a function <strong>f</strong> as follows:</p>

<img style="display: block; margin-left: auto; margin-right: auto;" src="./24397/file/DqnwcWAZ.png" width="370" height="118" alt="f(0,n,k)=n^k \\ f(m,n,k)=\sum_{i=0}^n f(m-1,i,k), m>0" title="f(0,n,k)=n^k \\ f(m,n,k)=\sum_{i=0}^n f(m-1,i,k), m>0">

<p>The mathematician presented Shannon with an ultimatum: You will write a program to calculate this function modulo 10^9+7 for various values of <strong>m</strong>, <strong>n</strong>, and <strong>k</strong> within the given constraints XOR I will shoot you with this gun!</p>

<p>As the mathematician lay recovering in his hospital bed, a Sigma Nu brother who had witnessed the event gingerly approached him and said, "Professor Martinson, I've written a program to solve your problem, but the online judge on your website keeps telling me the answer is wrong. Please tell me what the problem is. Submission ID 571972597."</p>

<p>Wearily, Martinson replied, "Have you written a brute force program to verify your program's output for smaller cases?"</p>

<p>The Sigma Nu brother replied, "Sorry, what did you say? I wasn't listening. Hey, are you going to eat that?" He then took the professor's chocolate pudding and went home to his lovely girlfriend from Zeta to enjoy the rest of the evening.</p>

<h3>Input</h3>

<p>In the first line, an integer <strong>T</strong>, the number of test cases. Then <strong>T</strong> lines containing integers <strong>m</strong>, <strong>n</strong>, and <strong>k</strong> separated by spaces.</p>

<h3>Output</h3>

<p><strong>T</strong> lines containing the value of <strong>f</strong>(<strong>m</strong>,<strong>n</strong>,<strong>k</strong>) modulo 10^9+7 for each test case.</p>

<h3>Constraints</h3>

<p>
1 ¡Ü <strong>T</strong> ¡Ü 20000 <br>
0 ¡Ü <strong>m</strong> ¡Ü 1000 <br>
0 ¡Ü <strong>n</strong> ¡Ü 10^9 <br>
0 ¡Ü <strong>k</strong> ¡Ü 1000
</p>

<h3>Example</h3>

<p><strong>Input:</strong></p>
<pre>5
0 0 0
1 100 1
2 100 0
2 100 1
100 100 100</pre>

<p><strong>Output:</strong></p>
<pre>1
5050
5151
171700
143422859</pre>

<h3>Additional Info</h3>

<p>There are two randomly generated data sets, one with <strong>T</strong>=10000 and the other with <strong>T</strong>=20000. The distributions are close to uniform random.</p>

<p>At the time of publication, my C code runs in 0.69s and my Python 2.7 code runs in 24.70s. The Python code is about 1KB, not golfed.</p>