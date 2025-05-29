<p>In a galaxy, far far away, there was a planet, Gringo quite similar to our own. Maybe it is because the planet has a similar "Sun" and "Moon". In Gringo, people use a calendar which is identical to ours. It is said this calendar was made by one of many kings in Gringo's history thousands of years ago. In the legend, it says the king liked programming very much, and at one night he solved a very difficult problem. He was so happy that he wanted to make a new calendar to congratulate. Hence in his calendar, this very midnight with full moon is first second.</p>
<p>&nbsp;</p>
<p>In this calendar, names of periods of time are same to ours, like days, months, years, minutes and seconds. In Gringo planet, the planet will reach same position on its revolution around the "Sun" every T1 seconds, the time between two neighbor full moons is T2 seconds and the time between two neighbor midnights is T3 seconds. It's very clear that a year is T1 seconds and a day is T3 seconds. And luckily, T1 is divisible by T3. So a leap year is unnecessary.</p>
<p>&nbsp;</p>
<p>But T2 may be not divisible by T3, which is very troublesome. But our king was very clever, he made following rules.</p>
<p>&nbsp;</p>
<p>1. A new day comes when a midnight come.</p>
<p>2. A new year comes when the planet reaches the same position with the "first midnight" on its revolution around the "Sun". Of course it will be a midnight and a new day will come, too.</p>
<p>3. When a new day comes, if the "Moon" will be full in this day, a new month will come, too.</p>
<p>4. When a new year comes, a new month will come, too. The "Moon" may not be full. So the month was called "0th month" of a year, until a new full moon come.</p>
<p>5. Due to these complex rules, it is very difficult to calculate how many days in a month. Now many people in Gringo are turning to you for help.</p>
<p>&nbsp;</p>
<p><strong>Input</strong></p>
<p>&nbsp;</p>
<p>There are multiple test cases. The first line of input contains an integer T (T&lt;= 20), indicating the number of test cases. Then T test cases follow. There is a blank line between different test cases. The first line of each test case contains 3 integers T1, T2 and T3 (1&lt;=T3&lt;=10000, 5&lt;=T1/T3&lt;=1000, T1 is divisible by T3, T3&lt;T2&lt;T1). The next line contains an integer Q (1&lt;=Q&lt;=100). Then Q lines follow, each line contains two integer Yi and Mi, means the Mith month in Yith year, (1 &lt;= Yi &lt;=5000, 0&lt;= Mi &lt;= 5000).</p>
<p>&nbsp;</p>
<p><strong>Output</strong></p>
<p>&nbsp;</p>
<p>For each month, output how many days in that months. If there is no such month, output 0.</p>
<p>&nbsp;</p>
<p><strong>Sample Input</strong></p>
<p>1</p>
<p>3650 295 10</p>
<p>4</p>
<p>1 1</p>
<p>1 2</p>
<p>2 0</p>
<p>2 13</p>
<p>&nbsp;</p>
<p><strong>Sample Output</strong></p>
<p>29</p>
<p>30</p>
<p>18</p>
<p>0</p>