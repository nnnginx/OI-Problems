<p>For a given  number <em>n</em> give all almost square factorisations of <em>n</em>,</p>
<p>so where <em>n=(a^2-1)*(b^2-1) </em>and <em>1&lt;a&lt;=b</em>.</p>
<h3>Input</h3>
<p>The first line contains the number of test cases <em>T</em>, where <em>T&lt;=1000</em>. Each of the following <em>T</em> lines contains one integer <em>0&lt;n&lt;2^62</em>.</p>
<h3>Output</h3>
<p>For each test case print the case number then on a new line the factorisations in increasing order of <em>a</em> value. If there is no such factorisation then print an error message, see the sample input/output for the correct format!</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>4<br>546939993600<br>100<br>172569415200<br>3467754019458593280<br><br><strong>Output:</strong><br>Case #1:<br>546939993600=(31^2-1)*(23869^2-1)=(34^2-1)*(21761^2-1)[do not break the line here]<br>=(271^2-1)*(2729^2-1)=(351^2-1)*(2107^2-1)=(701^2-1)*(1055^2-1)<br>Case #2:<br>For n=100 there is no almost square factorisation.<br>Case #3:<br>172569415200=(456^2-1)*(911^2-1)<br>Case #4:<br>3467754019458593280=(20513^2-1)*(90781^2-1)</pre>