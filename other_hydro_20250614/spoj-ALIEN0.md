<p>There's a line of <strong><em>N</em></strong> numbers where each number is a positive integer that is less than <strong><em>10<sup>9</sup></em></strong>. Every second, an alien comes down to the Earth and ask a certain problem. "How many zeros are there after all the other digits when you multiply all the number in range <strong><em>L&nbsp;</em></strong>and<strong><em>&nbsp;R&nbsp;</em></strong>?". Unfortunately, the alien don't know base 10 numbers. In fact, there're <strong><em>6</em></strong> species of alien in the UFO, the first species use base-1 number, second use base-2 and so on. (Yes, the first species do not exist, and therefore will not come down to the Earth).<br><br>You are given a task to answer the aliens' questions in their numerical system for a day, which mean there're up to <strong><em>100,000</em></strong> questions to be answer.</p>
<h3>Input</h3>
<p>First line,<strong><em> </em></strong><em><strong><em>N &lt;= 100000</em></strong> </em>which is mentioned above<em>&nbsp;</em>and <strong><em>Q &lt;= 100000</em>&nbsp;</strong>representing number of questions.<br>Next line, <em><strong style="font-style: italic;">N </strong>positive integers</em>&nbsp;on the line on earth, each not exceeding <strong><em>10<sup>9</sup></em></strong>.<br>Next <em><strong>Q</strong> </em>lines, <em><strong>1 &lt;=&nbsp;L &lt;= R &lt;= N</strong> </em>representing a range each alien mentioned, and <em><strong>2 &lt;=&nbsp;S &lt;= 6</strong>&nbsp;</em>representing the alien species.</p>
<h3>Output</h3>
<p><em>Q lines, </em>each line is a number represent the answer for each alien.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 3<br>2 3 6 5 100<br>1 5 2<br>1 3 6<br>1 2 3&nbsp;</pre>
<pre><strong>Output:</strong>
4<br>2<br>1&nbsp;</pre>