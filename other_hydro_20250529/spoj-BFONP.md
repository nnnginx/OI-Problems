<p>Have you solved <a title="Transform the Expression" href="../ONP/" target="_blank">ONP</a> problem? Especially using&nbsp;<a title="Brainf**k" href="../../../ranks/ONP/lang=BF" target="_blank">brainf**k</a>? This problem will give you extra points if you can solve <a title="Transform the Expression" href="../ONP/" target="_blank">ONP</a>&nbsp;using <a title="Brainf**k" href="../../../ranks/ONP/lang=BF" target="_blank">brainf**k</a>. Note that this problem has larger constraints.</p>
<p>The task is: "Transform the algebraic expression with brackets into RPN form (Reverse Polish Notation). Two-argument operators: +, -, *, /, ^ (priority from the lowest to the highest), brackets ( ). Operands: only letters: a,b,...,z. Assume that there is only one RPN form (no expressions like a*b*c)."</p>
<h3>Input</h3>
<p>t [the number of expressions �� 1000]</p>
<p><em>expression</em>&nbsp;[length = See: "Other Info" part]</p>
<p>[other expressions]</p>
<h3>Output</h3>
<p>The <em>expressions</em>&nbsp;in RPN form, one per line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>3</pre>
<pre>(a+(b*c))</pre>
<pre>((a+b)*(z+x))</pre>
<pre>((a+t)*((b+(a+c))^(c+d)))

<strong>Output:</strong></pre>
<pre>abc*+
</pre>
<pre>ab+zx+*</pre>
<pre>at+bac++cd+^*</pre>
<h3>Other Info</h3>
<p>Input: I deliberately not tell the input length, constraints, distribution, etc. You can guess it from judge output for my BF program (BF Cell Used) ;-) And of course I gernerate it randomly (But I can't tell the distribution).<br>This problem is using custom judge, so you can see the detail after you get AC/WA.<br>Judge output format is like this: ("<span style="text-decoration: underline;">Code Length (Valid Command only)</span>")"<span style="text-decoration: underline;">Cell Used</span>"("<span style="text-decoration: underline;">BF Command executed</span>").<br><a title="My Submission" href="http://4.bp.blogspot.com/-Ldc9bnElF4E/UeO3ZEfJJTI/AAAAAAAAAXQ/KqTYittMt_E/s1600/Transform+the+Expression+(Again!).png" target="_blank">Click here to see my submission result for this problem.</a><br>I have two solutions for this problem:<br>1) ID 9658441 (otimized):&nbsp;Judge output for my BF code is: (471)4320(606116310) meaning that my Valid BF commands = 471 commands and My code using 4320 BF cell and 606116310 commands executed.<br>2) ID 9658572 (golfed): Judge output for my BF code is: (295)4320(888371635) meaning that my Valid BF commands = 295 commands and My code using 4320 BF cell and 888371635 commands executed.<br>You can click (AC/WA) status for more detail.<br>My code running time is 0.68s (optimized solution) and 1.47s (golfed solution) and both using 1.6M of memory.<br>Time limit is ~14�� my BF program top speed.</p>
<hr>
<p><strong>See also:</strong> <a title="TJANDRA" href="../TJANDRA/" target="_blank">Another problem added by Tjandra Satria Gunawan</a></p>