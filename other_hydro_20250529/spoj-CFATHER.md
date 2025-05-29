<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>The computer science mafia, headed of course by the Codefather, have control of the computer science course points spreadsheet. The Codefather has the power to transfer points from one person to another.</p>
<p>The Codefather¡¯s daughter is getting married, and he wants to give a gift to his future son-in-law, who happens to be taking this computer science course. Since only the person with the most points can get a mark of 100% in this course, the Codefather wants to insure that his future son-in-law will have strictly more points than anyone else by performing a number of point transfers. However, he¡¯s a cautious man (in his business, you have to be), so he follows the following rules:</p>
<p>&nbsp; &nbsp;1. None of the transfers will involve his future son-in-law.</p>
<p>&nbsp; &nbsp;2. For each pair of people, he will only perform up to one point transfer, though this transfer can involve any number of points.</p>
<p>&nbsp; &nbsp;3. No person can be involved in both transfers in which they lose and gain points - only one or the other (or neither).</p>
<p>&nbsp; &nbsp;4. After all the transfers are completed, no student can have a negative amount of points.</p>
<p>There are $N$&nbsp;($1 \leq N \leq 5000$) students in this course, each with a unique student number from $1$ to $N$, inclusive. Student $i$&nbsp;starts off with $P_i$&nbsp;($1 \leq P_i \leq&nbsp;10^6$) points. The Codefather¡¯s future son-in-law is student $1$.</p>
<p>Though the Codefather is a powerful man, he¡¯s still wary of the authorities, and wants to remain as inconspicuous as possible. Therefore, he wants to minimize the number of points in the largest transfer he makes, while still insuring that his future son-in-law will get 100%.</p>
<h3>Input</h3>
<p>Line $1$: 1 integer<strong>, </strong>$N$</p>
<p>Next $N$&nbsp;lines: 1&nbsp;integer, $P_i$, for $i=1..N$</p>
<h3>Output</h3>
<p>If it¡¯s possible for the Codefather to observe the rules and give his future son-in-law more points than anyone else, minimize the number of points in the largest transfer he must make and output this value.</p>
<p>Otherwise, output ¡°impossible¡±.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">4</span>
<span style="font-family: 'courier new', courier;">500</span>
<span style="font-family: 'courier new', courier;">300</span>
<span style="font-family: 'courier new', courier;">900</span>
<span style="font-family: 'courier new', courier;">100</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">202</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The future son-in-law only has 500 points, so the Codefather must make student 3 lose at least 401. However, the other students must also stay strictly below 500. His best strategy is to transfer 199 points from student 3 to student 2, and 202 points from student 3 to student 4. This will result in the following point distribution:</p>
<p>Student 1: 500</p>
<p>Student 2: 499</p>
<p>Student 3: 499</p>
<p>Student 4: 302</p>