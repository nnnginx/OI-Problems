<pre><span style="font-family: verdana, geneva;"><span style="font-size: small;">You are given a string. You have to count the total lengths of all <strong>WOW</strong> substrings.<br></span></span><span style="font-family: verdana, geneva;"><span style="font-size: small;"><strong>WOW</strong> substrings are defined as a contiguous substring of a string<br></span></span><span style="font-size: small; font-family: verdana, geneva;">where there is no any character occurring more than one times.<br></span><span style="font-family: verdana, geneva;"><span style="font-size: small;">That means, all the characters of substring are unique.<br></span></span><span style="font-family: verdana, geneva;"><span style="font-size: small;">As answer could be very large, so print it modulo <strong>100007</strong>. (NOTE THAT: 100007 is not a prime number!!)</span></span></pre>
<h3>Input</h3>
<p><span style="font-size: small;">Input starts with an integer&nbsp;<strong>TC</strong>(&lt;=50), denoting the number of test cases.<br>Each case starts with N and M, denoting respectively length of string and<br> total characters of string  represented as integers from 1 to M. Then,follows<br>a line with space separated N integers ( each in the range 1 to M ).</span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input starts with an integer TC(&lt;=50), denoting the number of test cases.Each case starts with a string S.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">All characters in string will consists of only lowercase letters of English alphabets.</div>
<h3>Output</h3>
<p><span style="font-size: small;">For each case, print the case number and total lengths of all WOW substrings of given string modulo&nbsp;</span><strong>100007</strong><span style="font-size: small;">.</span></p>
<h3>
<p style="font-size: 10px; font-weight: normal;"><strong><span style="font-size: small;">Constraints:</span></strong></p>
<p style="font-size: 10px; font-weight: normal;"><strong><span style="font-size: small;">1&lt;=TC&lt;=50.</span></strong></p>
<p style="font-size: 10px; font-weight: normal;"><strong><span style="font-size: small;">1&lt;=N&lt;=500000. (Length of string)</span></strong></p>
<p style="font-size: 10px; font-weight: normal;"><strong><span style="font-size: small;">1&lt;=M&lt;=1000000.(Character id range)</span></strong></p>
</h3>
<h3>Example</h3>
<pre><strong><span style="font-size: small;">Input:</span></strong>
<p style="white-space: normal;"><strong><span style="font-size: small;">2<br></span></strong><strong><span style="font-size: small;">3 2</span></strong></p><p style="white-space: normal;"><strong><span style="font-size: small;">1 2 1</span></strong></p><p style="white-space: normal;"><strong><span style="font-size: small;">4 3</span></strong></p><p style="white-space: normal;"><strong><span style="font-size: small;">2 1 3 2</span></strong></p>
<strong><span style="font-size: small;">Output:</span></strong>
<span style="font-size: small;"><strong>Case</strong><strong>&nbsp;1: 7<br></strong></span><strong><span style="font-size: small;">Case 2: 16</span></strong>
</pre>