<p>Atul loves gifting choclates and Aastha loves eating them but excess of anything is bad and same goes for choclates. Eating all those chocolates has made Aastha overweight and she needs to watch her weight now. So she has to classify the chocolates based on their sugar content. She gave this task to Jaya. After completing the task Jaya is still not confident. She wants you to check whether her classification is correct or not. Basically if two chocolates have the same sugar level they are represented as a=b else they are represented as a!=b. You are given a list of binary relations, equalities and inequalities, like a = b, a != d, b = c etc. Your task is to output YES if the classification is correct , that you can satisfy all equalities and inequalities. Otherwise you should output NO.</p>
<h3>Input</h3>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In the first line there is one integer T denoting the number of test cases. Description of T test cases follow. Each one have two integers N and K given in the first line denoting the number of variables and the number of relations between them for this test case. All variables are represented by integers in range [1, N]. K lines follow. Each of them is of the form "x1 R x2" where x1 and x2 are integers representing variables&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="white-space: pre;"> </span>and R is either "=" or "!=" and denotes the kind of relation between these variables.</div>
<p>In the first line there is one integer T denoting the number of test cases. Description of T test cases follow. Each one have two integers N and K given in the first line denoting the number of variables and the number of relations between them for this test case. All variables are represented by integers in range [1, N]. K lines follow. Each of them is of the form "x1 R x2" where x1 and x2 are integers representing variables and R is either "=" or "!=" and denotes the kind of relation between these variables.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p><span style="color: #252c33; font-family: 'Open Sans', sans-serif; font-size: 14px; line-height: 21px; word-spacing: 1px;">Output exactly&nbsp;</span><span style="font-weight: 600; color: #252c33; font-family: 'Open Sans', sans-serif; font-size: 14px; line-height: 21px; word-spacing: 1px;">T</span><span style="color: #252c33; font-family: 'Open Sans', sans-serif; font-size: 14px; line-height: 21px; word-spacing: 1px;">&nbsp;lines. In i-th of them, output the answer to the i-th test case.</span></p>
<p>&nbsp;</p>
<p><span style="font-family: 'Open Sans', sans-serif; color: #252c33;"><span style="font-size: 14px; line-height: 21px; word-spacing: 1px;">1&lt;=N,K&lt;=10^6</span></span></p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><pre style="overflow-x: auto; padding: 10px; margin: 0px; color: #46535e; font-size: 14px; line-height: 21px; word-spacing: 1px;">2
2 2
1 = 2
1 != 2
3 2
1 = 2
2 != 3</pre>
<strong>Output:</strong>
<pre style="overflow-x: auto; padding: 10px; margin: 0px; color: #46535e; font-size: 14px; line-height: 21px; word-spacing: 1px;">NO
YES</pre>
</pre>