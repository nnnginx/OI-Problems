<p style="padding-top: 2px; padding-right: 4px; padding-bottom: 2px; padding-left: 4px; font-family: Arial, Helvetica, sans-serif; font: normal normal normal 12px/1.4em Arial, sans-serif; line-height: 1.5em; margin: 0px;">N ports are to be constructed on the bytelandian river. Since trade occurs only along a Y miles stretch of the river, the distance between the start point and the last port must be Y. (Consider start point has the 0th port.)</p>
<p style="padding-top: 2px; padding-right: 4px; padding-bottom: 2px; padding-left: 4px; font-family: Arial, Helvetica, sans-serif; font: normal normal normal 12px/1.4em Arial, sans-serif; line-height: 1.5em; margin: 0px;">To optimize the ship movement between important ports, the distance between any two consecutive ports has been fixed to be within a range of possible distances. Also, distance between two consecutive ports can only be an integer number of miles.</p>
<p style="padding-top: 2px; padding-right: 4px; padding-bottom: 2px; padding-left: 4px; font-family: Arial, Helvetica, sans-serif; font: normal normal normal 12px/1.4em Arial, sans-serif; line-height: 1.5em; margin: 0px;">As a programmer you have been assigned the job of evaluating the number of different possible arrangements of ports modulo 1000000007.</p>
<p>&nbsp;</p>
<div><strong>Input</strong></div>
<p style="padding-top: 2px; padding-right: 4px; padding-bottom: 2px; padding-left: 4px; font-family: Arial, Helvetica, sans-serif; font: normal normal normal 12px/1.4em Arial, sans-serif; line-height: 1.5em; margin: 0px;">First line of input contains t. The number of test cases. (t&lt;100)</p>
<p style="padding-top: 2px; padding-right: 4px; padding-bottom: 2px; padding-left: 4px; font-family: Arial, Helvetica, sans-serif; font: normal normal normal 12px/1.4em Arial, sans-serif; line-height: 1.5em; margin: 0px;">First line of each test case contains two integers: N, the number of ports to be built (N&lt;=20) and Y, the ditance between the start point and the last port. (Y&lt;100000)</p>
<p style="padding-top: 2px; padding-right: 4px; padding-bottom: 2px; padding-left: 4px; font-family: Arial, Helvetica, sans-serif; font: normal normal normal 12px/1.4em Arial, sans-serif; line-height: 1.5em; margin: 0px;">Next N lines of the test case contains the range of distances between consecutive ports, with ith line giving two integers, the minimum and maximum gap between (i-1)th and ith port.</p>
<p style="padding-top: 2px; padding-right: 4px; padding-bottom: 2px; padding-left: 4px; font-family: Arial, Helvetica, sans-serif; font: normal normal normal 12px/1.4em Arial, sans-serif; line-height: 1.5em; margin: 0px;">&nbsp;</p>
<div><strong>Output</strong></div>
<p>Print one of output for each test case which is the number of possible arrangements modulo 1000000007.</p>
<p>&nbsp;</p>
<p><strong>Example</strong></p>
<pre><strong>Input:</strong></pre>
<pre>1</pre>
<pre>2 4</pre>
<pre>0 3</pre>
<pre>0 3</pre>
<pre><strong>Output:</strong></pre>
<pre>3</pre>