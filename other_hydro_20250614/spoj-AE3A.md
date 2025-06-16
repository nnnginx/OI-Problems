<pbyteman is="" the="" person="" in="" charge="" of="" a="" team="" that="" looking="" for="" crude="" oil="" reservoirs.="" he="" has="" made="" two="" boreholes:="" found="" point="" and="" out="" there="" no="" b.="" it="" known="" reservoir="" occupies="" connected="" fragment="" segment="" ab="" with="" one="" end="" at="" a.="" now="" byteman="" to="" check,="" how="" far,="" along="" connecting="" points="" b,="" does="" reach.="" not="" simple,="" however,="" because="" some="" locations="" can="" drill="" faster="" than="" other="" locations.="" moreover,="" byteman&#8217;s="" rather="" small,="" so="" they="" most="" location="" time.="" boss="" would="" like="" him="" predetermine="" when="" will="" be="" able="" identify="" boundary="" reservoir.<="" p="">
<p>Byteman has asked you for help. He has divided the segment connecting points A and B into n+1 segments
of equal length. If we assume that point A has coordinate 0, and point B coordinate n + 1, then there are
n points with coordinates 1, 2, . . . , n between them. It is enough to find the farthest from A of these points
in which some crude oil occurs. Byteman has informed you about the amounts of time necessary for making
boreholes in these points ¡ª they are equal to t<sub>1</sub>, t<sub>2</sub>, . . . , t<sub>n</sub> respectively. You should create such a plan of
drilling, that the time necessary to identify the oil reservoir¡¯s boundary is shortest possible, assuming the
worst-case scenario.</p>

<h3>Input</h3>
<p>The first line of the standard input contains a single positive integer n (1 ¡Ü n ¡Ü 2000). The second line contains
n positive integers t1, t2, . . . , tn separated by single spaces (1 ¡Ü t<sub>i</sub> ¡Ü 10<sup>6</sup>).</p>

<h3>Output</h3>
<p>Your program should write a single integer to the standard output¡ªthe smallest amount of time that Byteman
has to spend (assuming the worst-case scenario) drilling in search of oil, to be sure that he will identify the
reservoir¡¯s boundary.</p>
<h3>Example</h3>
<p>
For the input data:
</p><pre>4
8 24 12 6
</pre>
<p></p>
<p>the correct result is:
</p><pre>42
</pre>
<p></p>
<p><b>Explanation of the example.</b>
</p><p>Assume that Byteman makes the first borehole at point 1, what takes him
time 8. It can then turn out that he finds crude oil there and he will have to check, how far to the right does
the reservoir reach. He will need two more boreholes, making which requires 36 units of time in the worst case.
Therefore, in this case Byteman will spend in total 44 units of time drilling.</p>
<p>It turns out that it is better to start at point 2. If there is no crude oil there, it is sufficient to check point
1. However, in the worst case Byteman will have to make two more boreholes in points 3 and 4 and end his
work in total time equal to 42. </p><p></p>
</pbyteman>