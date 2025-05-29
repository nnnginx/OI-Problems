<p>Note: The problem description is same as <a title="GCJPURE" href="../GCJPURE/" target="_blank">GCJPURE</a>, but with more higher constraints (to become more challenging), more strict time limit (to reject bad complexity), and more strict source limit (to reject hardcoded precomputation). Good Luck.</p>
<h3 style="text-align: center;">Problem Description</h3>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Pontius: You know, I like this number 127, I don't know why.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Woland: Well, that is an object so pure. You know the prime numbers.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Pontius: Surely I do. Those are the objects possessed by our ancient masters hundreds of years ago. Oh, yes, why then? 127 is indeed a prime number as I was told.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Woland: Not... only... that. 127 is the 31st prime number; then, 31 is itself a prime, it is the 11th; and 11 is the 5th; 5 is the 3rd; 3, you know, is the second; and finally 2 is the 1st.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Pontius: Heh, that is indeed... purely prime.</div>
<blockquote>
<p style="text-align: center;"><span style="background-color: #c0c0c0;"><span style="font-size: x-small;"><span style="background-color: #ffffff;">Pontius: You know, I like this number 127, I don't know why.</span></span></span></p>
<p style="text-align: center;"><span style="background-color: #c0c0c0;"><span style="font-size: x-small;"><span style="background-color: #ffffff;">Woland: Well, that is an object so pure. You know the prime numbers.</span></span></span></p>
<p style="text-align: center;"><span style="background-color: #c0c0c0;"><span style="font-size: x-small;"><span style="background-color: #ffffff;">Pontius: Surely I do. Those are the objects possessed by our ancient masters hundreds of years ago. Oh, yes, why then? 127 is indeed a prime number as I was told.</span></span></span></p>
<p style="text-align: center;"><span style="background-color: #c0c0c0;"><span style="font-size: x-small;"><span style="background-color: #ffffff;">Woland: Not... only... that. 127 is the 31st prime number; then, 31 is itself a prime, it is the 11th; and 11 is the 5th; 5 is the 3rd; 3, you know, is the second; and finally 2 is the 1st.</span></span></span></p>
<p style="text-align: center;"><span style="background-color: #c0c0c0;"><span style="font-size: x-small;"><span style="background-color: #ffffff;">Pontius: Heh, that is indeed... purely prime.</span></span></span></p>
</blockquote>
<p>The game can be played on any subset S of positive integers. A number in S is considered pure with respect to S if, starting from it, you can continue taking its rank in S, and get a number that is also in S, until in finite steps you hit the number 1, which is not in S.</p>
<p>When n is given, in how many ways you can pick S, a subset of {2, 3, ..., n}, so that n is pure, with respect to S? The answer might be a big number, you need to output it modulo 10<sup>9</sup>+7.</p>
<h3>Input</h3>
<p>The first line of the input gives the number of test cases, <strong>T</strong>. <strong>T</strong> lines follow. Each contains a single integer <strong>n</strong>.</p>
<h3>Output</h3>
<p>For each test case, output one line containing "Case #x: y", where x is the case number (starting from 1) and y is the answer as described above.</p>
<h3>Constraints</h3>
<p><strong>T</strong>&lt;10<sup>5</sup></p>
<p>2��<strong>n</strong>��10<sup>5</sup></p>
<p>Note: This constraints was selected carefully</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>2</pre>
<pre>5</pre>
<pre>6

<strong>Output:</strong></pre>
<pre>Case #1: 5</pre>
<pre>Case #2: 8</pre>
<p>&nbsp;</p>
<h3 style="white-space: normal;">Other Info</h3>
<h3 style="white-space: normal;"><span style="font-size: 10px; font-weight: normal;">Sorry for slow language user, I've made an experiment and the result is if I set constraints that allow slow languages to be accepted with 'good' complexity O(f(n)), then the 'bad' complexity O(f(n)*log(n)) could be accepted too using fast language (Because slow language is ~80x slower than fast language). I don't want this happen. But don't feel so bad :-) I've made <a href="../BUGTEST/" target="_blank">this tutorual problem</a> that allow slow languages to be accepted (except maybe: PIKE).<br></span></h3>
<p><em><span style="text-decoration: underline;">Time limit ~4��&nbsp;My Program top speed (25.53s using 1744B of C code).</span></em></p>
<p><em>You can see my submission history and time record for this problem</em>: <a title="My submission history" href="http://4.bp.blogspot.com/-it5U2HvbObg/UZu-iOe8AsI/AAAAAAAAAU4/qDvZDNxqGyY/s1600/EGCJPURE.png" target="_blank">here</a></p>
<p><strong>See also:</strong> <a title="TJANDRA" href="../TJANDRA/" target="_blank">Another problem added by Tjandra Satria Gunawan</a></p>