<p>Amr M. believes in conspiracies. He is very suspicious about everything, and he is always trying to uncover the truth to everyone (or so he thinks). Lately he became very suspicious of TV ads, especially the ones that are made of 2 words: ad1 and ad2, and thinks they carry hidden messages.</p>
<p>After contacting his top secret resources, he found out the process that the evil people use to hide the message. The original message is always two strings: orig1 and orig2.</p>
<p>The transformation happened as follows:</p>
<ol>
<li>The letters from orig1 are shuffled.</li>
<li>The letters from orig2 are shuffled.</li>
<li>One letter from either orig1 or orig2 is replaced with its next or previous letter in the alphabet.</li>
</ol>
<p>This produces ad1 and ad2 from orig1 and orig2 respectively. For example for orig1 = "bcd", orig2 = "wcy" we may have ad1 = "dcb", ad2 = "cxy" (shuffled to cwy and 'w' replaced with 'x')</p>
<p>After more research, Amr also found out the distance X, which is equal to distance(orig1,ad1)+distance (orig2,ad2). The distance between 2 strings is the sum of absolute difference between the letters at same positions (e.g. difference("ab","cd") =&nbsp; abs('a'-'c')+abs('b'-'d') = 4)</p>
<p>But the number of possible original messages appears to be very high, so Amr hired you to count them. Given string ad1 and ad2, and X = distance(orig1,ad1) + distance (orig2,ad2), return the number of possible strings orig1 &amp; orig2.</p>
<p><strong>Input Specification:</strong></p>
<p>The first line of input contains an integer T that represents the number of test cases, then follow T lines each line is in format ad1 ad2 X, space separated where ad1, ad2 are composed from English small-case letters.</p>
<p>1 ¡Ü length (ad1),&nbsp; length(ad2) &nbsp;¡Ü 10, 'b' ¡Ü ad1[i], ad2[i] ¡Ü 'y' and 0 ¡Ü X ¡Ü 100000</p>
<p><strong>Output Specification:</strong></p>
<p>For each test case, output a single line of output in the form <strong>¡°Case K: cnt¡±</strong> where K is the number of the test case and cnt is the number of possible strings orig1 &amp; orig2.</p>
<p><strong>Sample input:</strong></p>
<p>2<br>c n 1<br>kbenh kbenh 5</p>
<p><strong>Sample Output:</strong></p>
<p>Case 1: 4<br>Case 2: 16</p>
<p>&nbsp;</p>