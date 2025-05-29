<p>Jaiganesh and Siddharth were discussing about integer factorization. Suddenly Jai, who always thinks differently, thought, when it is possible to factorize numbers, why not factorize strings? Siddharth argued that it is impossible! So, now Jai wants to prove to Sid that it is possible for all strings. He decides to write a program that when given a string as input will factorize it. He then realised that there are many ways to factorize a string. So he decided to write a program that will maximize the sum of powers of the factors.</p>
<p>&nbsp;</p>
<p>Jai defined the nth power of a string as same string repeated n times. For example, (abc) ^ 2 = abcabc, and (abc) ^ 4 = abcabcabcabc.</p>
<p>&nbsp;</p>
<p>So, now this is what you have to do. Given a string as input, factorize the string such that the sum of powers is maximum and print that value of sum. An additional constraint is that the string should be factorized such that the power of each factor is always even. It is guaranteed that such a solution will always exist.</p>
<h3>Input</h3>
<p>The first line of input consists of C, the number of test cases. Then C lines follow each containing a string s, the length of which is always even.</p>
<p>1 &lt; |s| &lt; 100000</p>
<p>1 &lt; C &lt; 50</p>
<h3>Output</h3>
<p>The output consists of a single line for each test case, denoting the maximum sum of even powers that can be obtained.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1</pre>
<pre>abcabcababababacac

<strong>Output:</strong>
8</pre>
<pre><p><strong>Explanation of test case:</strong>&nbsp;</p><p>The string can be factorized as (abc) ^ 2 * (ab) ^ 4 * (ac) ^ 2.</p><p>The sum of powers is 2 + 4 + 2 = 8.</p></pre>