<p>Martin and Isa stopped playing crazy games and finally got married. It's good news! They're pursuing a new life of happiness for both and, moreover, they're moving to a new house in a remote place, bought with most of their savings.</p>
<p>Life is different in this new place. In particular, electricity is very expensive, and  they want to keep everything under control. That's why Martin proposed to keep a daily record of how much electricity has been consumed in the house. They have an electricity meter, which displays a number with the amount of KWh (kilowatt-hour) that has been consumed since their arrival.</p>
<p>At the beginning of each day they consult the electricity meter, and write down the consumption. Some days Martin does it, and some days Isa does. That way, they will be able to look at the differences of consumption between consecutive days and  know how much has been consumed.</p>
<p>But some days they simply forget to do it, so, after a long time, their register is now incomplete. They have a list of dates and consumptions, but not all of the dates are consecutive. They want to take into account only the days for which the consumption can be precisely determined, and they need help.</p>
<h3>Input</h3>
<p>The input contains several test cases. The first line of each test case contains one integer <em>N</em> indicating the number of measures that have been taken (2   �� <em>N</em> �� 10<sup>3</sup>). Each of the <em>N</em> following lines contains four integers <em>D</em>, <em>M</em>, <em>Y</em> and <em>C</em>, separated by single spaces,  indicating respectively the day (1   �� <em>D</em> �� 31), month (1   �� <em>M</em> �� 12), year (1900   �� <em>Y</em> �� 2100), and consumption (0   �� <em>C</em> �� 10<sup>6</sup>) read at the beginning of that day. These <em>N</em> lines are increasingly ordered by date, and may include leap years. The sequence of consumptions is strictly increasing (this is, no two different readings have the same number). You may assume that <em>D</em>, <em>M</em> and <em>Y</em> represent a valid date.</p>
<p>Remember that a year is a leap year if it is divisible by 4 and not by 100, or well, if the year is divisible by 400.</p>
<p>The end of input is indicated by a line containing only one zero.</p>
<h3>Output</h3>
<p>For each test case in the input, your program must print a single line containing two integers separated by a single space:  the number of days for which a consumption can be precisely determined, and the sum of the consumptions for those days.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
9 9 1979 440
29 10 1979 458
30 10 1979 470
1 11 1979 480
2 11 1979 483
3
5 5 2000 6780
6 5 2001 7795
7 5 2002 8201
8
28 2 1978 112
1 3 1978 113
28 2 1980 220
1 3 1980 221
5 11 1980 500
14 11 2008 600
15 11 2008 790
16 12 2008 810
0


<strong>Output:</strong>
2 15
0 0
2 191

</pre>