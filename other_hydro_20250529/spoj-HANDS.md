<p style="text-align: left;">The minute hand and hour hand love each other. The ¡®Second¡¯ hand is a spy who wants to keep track on how many times they pass over each other in a given interval on a day. Help the second hand.</p>
<p style="text-align: center;"><strong>Input</strong></p>
<p>First line contains the number of test cases t. Each test case has two lines representing the start time and end time respectively. The time would be in format (hh:mm). hh will be between 00 and 23, mm will be between 00 and 59. If the minute and hour hand are overlapping right at the start time (like at 12:00) then it would <strong>not be counted</strong>. (00:00 &lt;= '<strong>start time</strong>' &lt;&nbsp;'<strong>end time</strong>' &lt;= 23:59)</p>
<p style="text-align: center;"><strong>Output</strong></p>
<p>For each test case print, on a separate line, the number of times they overlap each other.</p>
<p>Example</p>
<p>Input</p>
<p>5</p>
<p>00:00<br>03:00</p>
<p>00:00<br>00:10</p>
<p>06:00<br>12:00</p>
<p>11:59<br>12:01</p>
<p>00:00<br>12:00</p>
<p>Output</p>
<p>2<br>0<br>6<br>1<br>11</p>