<p>Consider the following code:</p>
<pre>if (a) <br>if (b) <br>if (c)<br>foo();</pre>
<p>where <em>a,b </em>and <em>c</em>&nbsp;are boolean variables. If we run this code in C++, the function <em>foo()</em> is called if and only if all three variables are true. However, recently a new language - C-- - is being developed. In this language, when an <em>if()</em> evaluates to false, only the statement directly following it is not executed; for example, if <em>a</em> was false, the program would jump from <em>if(a)</em> to <em>if(c)</em>.</p>
<p>Using this convention, there are 5 different possible assignments of truth values to the variables <em>a</em>,<em>b</em>,<em>c</em>&nbsp;which end up calling <em>foo()</em>. Considering <em>a</em>,<em>b</em>,<em>c</em>&nbsp;as three bits in that order, they are 111, 101, 100, 011 and 001.</p>
<p>Given <strong>n</strong> boolean variables within a chain of <strong>m</strong>&nbsp;<em>if()</em>'s, where the variables within one <em>if()</em> are separated using <strong>logical or</strong>, count the number of ways to assign truth values to them which end up calling the function <em>foo()</em> (the call to <em>foo()</em>&nbsp;is after the last <em>if()</em>).</p>
<h3>Input</h3>
<p>The first line of the input is the number of test cases <strong>1 ¡Ü&nbsp;</strong><strong>T ¡Ü 30</strong>. <strong>T </strong>test cases follow.</p>
<p>The first line of each test case contains two nonnegative integers <strong>n ¡Ü 10<sup>5</sup></strong>&nbsp;- the number of boolean variables (they are numbered <strong>1</strong> through <strong>n</strong>) - and <strong>m ¡Ü 10<sup>5</sup></strong>&nbsp;- the number of <em>if()</em>'s. <strong>m</strong> lines follow, the <strong>i</strong>-th line describing the <strong>i</strong>-th <em>if()</em>. The first integer in each line is a positive integer <strong>k<sub>i</sub></strong>&nbsp;- the number of variables in the <strong>i</strong>-th <em>if()</em>&nbsp;(implicitly separated by the <strong>logical or</strong>&nbsp;operator) - followed by&nbsp;<strong>k<sub>i</sub></strong> positive integers in the range <strong>[1,n]</strong>: the variables in the <strong>i</strong>-th <em>if()</em>. Not all variables need necessarily appear within the <em>if() </em>chain, and the variables within one <em>if()</em>&nbsp;need not be distinct.</p>
<p>The sum of <strong>k<sub>i</sub></strong> within a test case will not exceed&nbsp;<strong>5*10<sup>5</sup></strong>. Additionally, the sum of <strong>n</strong>,<strong>m </strong>and <strong>k<sub>i</sub><sub>&nbsp;</sub></strong>within a single input file will not exceed <strong>2*10<sup>6</sup>.</strong></p>
<p><strong>The input is quite large - make sure to read it efficiently.</strong></p>
<h3>Output</h3>
<p>For each case, output the string "Case <strong>x</strong>:<strong> y</strong>" in a single line, where <strong>x</strong>&nbsp;is the number of the test case, starting from 1, and <strong>y </strong>is the number of ways of assigning truth values to the <strong>n</strong> boolean variables (out of <strong>2<sup>n</sup></strong>), which when run in C-- end up calling <em>foo()</em>, modulo <strong>10<sup>9</sup>+9</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3 3
1 1
1 2
1 3
5 3
2 1 2
3 1 3 5
2 2 4
<strong>Output:</strong>
Case 1: 5
Case 2: 24
</pre>
<p>&nbsp;</p>