<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">One of the most anxiously awaited occasions in any school is its annual day. Great excitement and hurried activities are visible all around. The prize-winners and those who are participating in the cultural programme are especially elated.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Raheem has volunteered to help organize the event, and he¡¯s in charge of the prize distribution ceremony for the kindergarten painting competition. Before the prizes are announced, the participants will be brought in and seated in the front row. There are N participants, and their paintings have been ranked from 1 to N by the judges (1 being the best). However, since all the entries were amazing, the judges have decided that everyone deserves a prize. So, Raheem has arranged N seats in the front row.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">All was well until Raheem realized that if both the neighbours of a participant (i.e the participants sitting on the chairs adjacent to his/her¡¯s) are ranked higher than him/her, then he/she will feel inferior and start crying (after all he/she is in kindergarten!). Raheem, being a puzzle-lover, wonders how many ways there are to seat the participants in the front row, so that none of them feel inferior. More importantly, Raheem also wants to find out what is the expected number of participants who will feel inferior if they are seated randomly, so that he can have that many people ready to take care of crying kindergarteners.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Notes :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1. Two seatings are different if there is at least one chair which is occupied by different students in the two arrangements.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2. ¡°Seated randomly¡± means each arrangement is equally likely to be chosen.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3. The participants sitting on the leftmost chair and the rightmost chair will never feel inferior, as they have only one neighbour.</div>
<p>One of the most anxiously awaited occasions in any school is its annual day. Great excitement and hurried activities are visible all around. The prize-winners and those who are participating in the cultural programme are especially elated.&nbsp;</p>
<p>Raheem has volunteered to help organize the event, and he¡¯s in charge of the prize distribution ceremony for the kindergarten painting competition. Before the prizes are announced, the participants will be brought in and seated in the front row. There are N participants, and their paintings have been ranked from 1 to N by the judges (1 being the best). However, since all the entries were amazing, the judges have decided that everyone deserves a prize. So, Raheem has arranged N seats in the front row.</p>
<p>All was well until Raheem realized that if both the neighbours of a participant (i.e the participants sitting on the chairs adjacent to his/hers) are ranked higher than him/her, then he/she will feel inferior and start crying (after all he/she is in kindergarten!). Raheem, being a puzzle-lover, wonders how many ways there are to seat the participants in the front row, so that none of them feel inferior. More importantly, Raheem also wants to find out what is the expected number of participants who will feel inferior if they are seated randomly, so that he can have that many people ready to take care of crying kindergarteners.&nbsp;</p>
<p><strong>Notes</strong> :</p>
<p>1. Two seatings are different if there is at least one chair which is occupied by different students in the two arrangements.</p>
<p>2. ¡°Seated randomly¡± means each arrangement is equally likely to be chosen.</p>
<p>3. The participants sitting on the leftmost chair and the rightmost chair will never feel inferior, as they have only one neighbour.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains the number of test cases T. T lines follow, one for each test case. Each line contains an integer N, denoting the number of students.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Output one line for each test case, containing two integers.&nbsp;</p>
<p>The first should be the number ways of seating the participants in the front row, so that none of them feel inferior. As this number can be very large, output it modulo 1000000007 (i.e. 10<sup>9&nbsp;</sup>+ 7).</p>
<p>The second should be the greatest integer less than or equal to the expected number of participants who will feel inferior if they are seated randomly.</p>
<p>&nbsp;</p>
<h3>Constraints</h3>
<p>0 &lt; T &lt; 20</p>
<p>0 &lt; N &lt; 10^9</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input</strong><strong>:</strong></pre>
<pre>2
1
3

<strong><strong>Output</strong></strong><strong>:</strong></pre>
<pre>1 0
</pre>
<pre>4 0</pre>
<pre><strong><strong>Explanation</strong></strong>:</pre>
<pre><p style="white-space: normal;">In the second test case, there are 2 arrangements in which 1 participant (the one ranked 3rd) feels inferior, namely 132 and 231. In the other 4 arrangements, namely 123, 213, 321 and 312, none of the participants feel inferior. The expected number of participants feeling inferior is 0*4/6 + 1*2/6 = 0.33.</p></pre>