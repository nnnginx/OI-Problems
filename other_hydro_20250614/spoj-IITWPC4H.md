<p id="docs-internal-guid-64c7d870-ec80-a56c-9e2a-608886dec8ad" style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt; text-indent: 36pt;" dir="ltr"><span style="font-size: small;"><strong><span style="color: #000000; background-color: transparent; font-weight: normal; font-style: normal; font-variant: normal; text-decoration: none; vertical-align: baseline;">Given two strings s and t of size n and m respectively. You can construct a string w of size n+m using s and t such that it should contain both s and t as its subsequences. <br><strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong></span></strong><span style="color: #000000; background-color: transparent; font-weight: normal; font-style: normal; font-variant: normal; text-decoration: none; vertical-align: baseline;">String w must satisfy this condition: For each character from 'a' to 'z', count of the character in w should be equal to sum of count in s and t. Additionally every character of w must belong to the subsequence for either s or t.</span><strong><span style="color: #000000; background-color: transparent; font-weight: normal; font-style: normal; font-variant: normal; text-decoration: none; vertical-align: baseline;">&nbsp;</span></strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;"><strong> </strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt; text-indent: 36pt;" dir="ltr"><span style="font-size: small;"><strong><span style="color: #000000; background-color: transparent; font-weight: normal; font-style: normal; font-variant: normal; text-decoration: none; vertical-align: baseline;">eg. if s = ab and t = cd, Then w can be abcd, acbd, cdab, cabd, acdb, cadb. Note that adcb is not correct, As t is not a subsequence in it.</span></strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;"><strong> </strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt; text-indent: 36pt;" dir="ltr"><span style="font-size: small;"><strong><span style="color: #000000; background-color: transparent; font-weight: normal; font-style: normal; font-variant: normal; text-decoration: none; vertical-align: baseline;">¡°Cuteness value¡± of a string is defined as the maximum length of consecutive equal characters in the string. </span></strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;"><strong> </strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt; text-indent: 36pt;" dir="ltr"><span style="font-size: small;"><strong><span style="color: #000000; background-color: transparent; font-weight: normal; font-style: normal; font-variant: normal; text-decoration: none; vertical-align: baseline;">For all possible string w that you can construct, find out the maximum value of ¡°Cuteness value¡±.</span></strong></span></p>
<h3>Input<span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;"><span style="font-size: x-small;">&nbsp;</span></span></h3>
<p><span style="font-size: small;"> First line contains T: number of test cases </span></p>
<p><span style="font-size: small;">For each test you case you are given a single line containing two space separated strings s and t. (1 &lt;= size (s), size (t) &lt;= 10^5).</span></p>
<p><span style="font-size: small;">Both the strings s and t will have characters from 'a' to 'z' of English alphabet only.</span></p>
<p><span style="font-size: small;">Note:Sum of length of all the input string is less than 5*10^6.</span></p>
<h3>Output</h3>
<p>For each test case, output the answer as given in problem statement.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1<br>ab ab

<strong>Output:</strong>
2</pre>