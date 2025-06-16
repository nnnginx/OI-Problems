<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Lucky numbers are positive integers composed only of the digits ‘4’ and ‘7’. &nbsp;For example,&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">47477 and 777 are lucky numbers while 457 and 1232 are not.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Super lucky numbers have the following additional properties:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">• &nbsp;They are a lucky number themselves</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">• &nbsp;Number of digits in them is a lucky number</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">• &nbsp;The number of ‘4’s or the number of ‘7’s in them is a lucky number (or both counts are&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">lucky numbers).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">A palindrome is an integer that reads the same forwards and backwards. &nbsp;For example, 547745</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">and 343 are palindromes while 74 and 12345 are not. &nbsp;A super lucky palindrome is a positive&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">integer that is both a super lucky number and a palindrome.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The Problem:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Given a number k, print the k</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">th</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">smallest super lucky palindrome.</div>
<p>Lucky numbers are positive integers composed only of the digits ‘4’ and ‘7’. &nbsp;For example,&nbsp;</p>
<p>47477 and 777 are lucky numbers while 457 and 1232 are not.</p>
<p>Super lucky numbers have the following additional properties:</p>
<p>• &nbsp;They are a lucky number themselves</p>
<p>• &nbsp;Number of digits in them is a lucky number</p>
<p>• &nbsp;The number of ‘4’s or the number of ‘7’s in them is a lucky number (or both counts are&nbsp;</p>
<p>lucky numbers).</p>
<p>A palindrome is an integer that reads the same forwards and backwards. &nbsp;For example, 547745</p>
<p>and 343 are palindromes while 74 and 12345 are not. &nbsp;A super lucky palindrome is a positive&nbsp;</p>
<p>integer that is both a super lucky number and a palindrome.</p>
<p>The Problem:</p>
<p>Given a number k, print the k-th smallest super lucky palindrome.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first input line contains a positive integer, n, indicating the quantity of numbers to check.&nbsp;</p>
<p>Each of the next n lines contains a single integer, k (1 ≤ k ≤ 10^18).</p>
<h3>Output</h3>
<p>For each query, first output the heading “Query #d: ”, where d is the query number, starting with 1.</p>
<p>Then, for the value k given in the query, print the k-th smallest super lucky palindrome.</p>
<p>Follow the format illustrated in Sample Output.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
1
2
3
5
100

<strong>Output:</strong>
Query #1: 4444
Query #2: 7777
Query #3: 4444444
Query #4: 4747474
Query #5: 44444444744744444444444444444444744744444444
</pre>