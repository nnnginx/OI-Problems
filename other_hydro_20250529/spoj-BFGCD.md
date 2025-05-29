<p>Budi is a rope seller, He initially has two ropes to sell with length&nbsp;<strong>a</strong>&nbsp;and&nbsp;<strong>b</strong>&nbsp;where&nbsp;<strong>a</strong>&nbsp;and&nbsp;<strong>b</strong>&nbsp;is positive integer less than 10<sup>100</sup>. One day he meet with strange rich customer, the customer want to buy all rope with equal length only. Budi has an idea to sell all his rope to that customer: cut the rope until all his rope become equal length. Because Budi want maximum profit, he need to minimize the "cut" operation. But the customer doesn't like waiting, so budi must calculate and do "cut" operation quickly. <em>The customer can wait 60 seconds only, Budi can cut the rope in exactly 10 seconds, so Budi have 50 seconds to calculate number of "cut" operation needed.</em>&nbsp;Help Budi to calculate number of "cut" operation and length of each rope after cutting process done. But unfortunately your modern calculator isn't working, so the only way to do is using <span style="text-decoration: underline;">brainf**k</span> calculator, with 8 valid commands only. Will you help Budi?</p>
<h3>Input</h3>
<p>First line of input there is an integer <strong>T</strong>&nbsp;�� 1000 denoting number of test case.</p>
<p>Next <strong>T</strong>&nbsp;lines there're two positive integer <strong>a</strong>&nbsp;and <strong>b</strong>&nbsp;denoting length of rope that Budi has initially. Separated by a space (ASCII:32).</p>
<p>Each line is terminated with newline character (ASCII:10).&nbsp;</p>
<h3>Output</h3>
<p>For each case, output two number: first number is minimum number of cut operation, and second number is length of each rope after cutting process done.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>4</pre>
<pre>1 42</pre>
<pre>42 1</pre>
<pre>42 42</pre>
<pre>12345 67890</pre>
<pre><strong>Output:</strong></pre>
<pre>41 1
</pre>
<pre>41 1</pre>
<pre>0 42</pre>
<pre>5347 15</pre>
<h3>Other Info</h3>
<p>Input: generated 99.9% random with average digit is about 74.8 digits<br>Output: Average digit for "cut" operation is about 34.7 digits, and length of rope after cutting process done is about 49.0 digits.<br>This problem is using custom judge, so you can see the detail after you get AC/WA.<br>Judge output format is like this: ("<span style="text-decoration: underline;">Code Length (Valid Command only)</span>")"<span style="text-decoration: underline;">Cell Used</span>"("<span style="text-decoration: underline;">BF Command executed</span>").<br><a title="My Submission" href="http://3.bp.blogspot.com/-m7Fl1ucvFPg/UeM70qCoGdI/AAAAAAAAAWw/KCHWZi4847Y/s1600/cut+the+rope.png" target="_blank">Click here to see my submission result for this problem.</a><br>Judge output for my BF code is: (11820)1157(6571171311) meaning that my Valid BF commands = 11820 commands and My code using 1157 BF cell and 6571171311 commands executed.<br>You can click (AC/WA) status for more detail.<br>My code running time is 6.95s and using 1.9M of memory.<br>Time limit is ~7�� my BF program speed.</p>
<hr>
<p><strong>See also:</strong> <a title="TJANDRA" href="../TJANDRA/" target="_blank">Another problem added by Tjandra Satria Gunawan</a></p>