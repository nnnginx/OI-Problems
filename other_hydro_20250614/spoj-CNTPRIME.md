<p><span style="font-family: 'trebuchet ms', geneva;">Tortoise and Achilles are playing the Counting the Primes game. Achilles will give Tortoise some numbers, and some intervals, and then Tortoise needs to count the primes on those intervals. It is an easy game, but Tortoise is doing the counting slowly. Achilles is pissed off, so he has given you the task as you are a good programmer. For a twist, he has changed the game a little bit, that is he will give some intervals for counting the prime as well as he will give some intervals to change the numbers in that interval.</span></p>
<p><span style="font-family: 'trebuchet ms', geneva;">You are given an array of <strong>n</strong> elements. After that you will be given <strong>M</strong> commands. They are -</span></p>
<ul>
<li><span style="font-family: 'trebuchet ms', geneva;"><strong>0 x y v</strong> - you have to change all numbers in the range of <strong>x</strong> to <strong>y</strong> (inclusive) to <strong>v</strong>, where <strong>x</strong> and <strong>y</strong> are two indexes of the array.</span></li>
<li><span style="font-family: 'trebuchet ms', geneva;"><strong>1 x y</strong> - output a line containing a single integer which is the number of primes between <strong>x</strong> and <strong>y</strong> (inclusive). </span></li>
</ul>
<p><span style="font-family: 'trebuchet ms', geneva;">The array is indexed from <strong>1</strong> to <strong>n</strong>.</span></p>
<p><strong><span style="font-family: 'trebuchet ms', geneva;">Input:</span></strong></p>
<p><span style="font-family: 'trebuchet ms', geneva;">Input starts with an integer <strong>T (�� 10)</strong>, denoting the number of test cases.</span></p>
<p><span style="font-family: 'trebuchet ms', geneva;">Each case contains two integers <strong>n (1 �� n �� 10<sup>4</sup>)</strong> and <strong>q (1 �� q �� </strong><strong>2*10<sup>4</sup></strong><strong>)</strong>. Then next line, you will be given <strong>N</strong> integers. After that each of the next <strong>q</strong> lines will contain a task in one of the following form:</span></p>
<ul>
<li><strong><span style="font-family: 'trebuchet ms', geneva;">0 x y v (1 �� x �� y �� n, 2 �� v �� 10<sup>6</sup>)</span></strong></li>
<li><strong><span style="font-family: 'trebuchet ms', geneva;">1 x y (1 �� x �� y �� n)</span></strong></li>
</ul>
<p><span style="font-family: 'trebuchet ms', geneva;">And the numbers will be in range of <strong>[2, 10<sup>6</sup>]</strong>.</span></p>
<p><strong><span style="font-family: 'trebuchet ms', geneva;">Output:</span></strong></p>
<p><span style="font-family: 'trebuchet ms', geneva;">For each case, print the case number first. Then for each query <strong>'1 x y'</strong>, print the number of primes between <strong>x</strong> and <strong>y [inclusively]</strong>.</span></p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="319" valign="top">
<p><strong><span style="font-family: 'trebuchet ms', geneva;">Sample Input</span></strong></p>
</td>
<td width="319" valign="top">
<p><strong><span style="font-family: 'trebuchet ms', geneva;">Output for   Sample Input</span></strong></p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p><span style="font-family: 'trebuchet ms', geneva;">1</span></p>
<p><span style="font-family: 'trebuchet ms', geneva;">5   3</span></p>
<p><span style="font-family: 'trebuchet ms', geneva;">78   2 13 12 3</span></p>
<p><span style="font-family: 'trebuchet ms', geneva;">1   1 2</span></p>
<p><span style="font-family: 'trebuchet ms', geneva;">0   4 4 5</span></p>
<p><span style="font-family: 'trebuchet ms', geneva;">1   1 5</span></p>
</td>
<td width="319" valign="top">
<p><span style="font-family: 'trebuchet ms', geneva;">Case   1:</span></p>
<p><span style="font-family: 'trebuchet ms', geneva;">1</span></p>
<p><span style="font-family: 'trebuchet ms', geneva;">4</span></p>
</td>
</tr>
</tbody>
</table>
<p><span style="font-family: 'trebuchet ms', geneva;"><br></span></p>
<p><span style="font-family: 'trebuchet ms', geneva;"><br></span></p>
<p><strong><span style="font-family: 'trebuchet ms', geneva;">Note: </span></strong></p>
<ul>
<li><strong><span style="font-family: 'trebuchet ms', geneva;">Use Faster IO like scanf,printf</span></strong></li>
<li><span style="font-family: 'trebuchet ms', geneva;"><strong>A prime number is a natural number greater than 1 that has no positive divisors other than 1 and itself. The first prime numbers are </strong><span id="MathJax-Element-21-Frame"><span id="MathJax-Span-121">2,3,5,7,11....<span style="display: inline-block; position: relative; width: 127px; height: 0px; font-size: 124%;"><span style="position: absolute; clip: rect(1.995em, 1000em, 3.168em, -0.404em); top: -2.823em; left: 0em;"><span id="MathJax-Span-122"><span id="MathJax-Span-123">2</span><span id="MathJax-Span-124">,</span><span id="MathJax-Span-125" style="padding-left: 0.167em;">3</span><span id="MathJax-Span-126">,</span><span id="MathJax-Span-127" style="padding-left: 0.167em;">5</span><span id="MathJax-Span-128">,</span><span id="MathJax-Span-129" style="padding-left: 0.167em;">7</span><span id="MathJax-Span-130">,</span><span id="MathJax-Span-131" style="padding-left: 0.167em;">11</span><span id="MathJax-Span-132">,</span><span id="MathJax-Span-133" style="padding-left: 0.167em;">��</span></span></span></span></span></span></span></li>
</ul>
<p>&nbsp;</p>