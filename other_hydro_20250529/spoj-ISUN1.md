<p>When LL and ErBao were young, they liked jumping rubber-rope (Tiao Pi Jin) very much. They jumped every day happily. But one day HH came and brought away the peaceful days. HH sometimes threw stones to them, and sometimes pushed them down suddenly. Seeing ErBao crying sadly, LL got angry finally, and decided to give HH some color see see.<br>There were n trees on the ground (regarded as points), and LL planed to use his rubber-rope to wrap all the trees and form a big circle, then fooled HH into it and threw stones to him. Before finding out how to fool HH into the circle, LL wants to know how big the rubber-rope circle would be, say, the perimeter.<br>But LL found it difficult than expected, because their playing territory and the trees were in a bigger fence (a simple polygon with m vertices). So, the rubber-rope mustn¡¯t be out of the fence either. It¡¯s your turn to help LL find the perimeter of the circle.</p>
<p>&nbsp;</p>
<p><strong>sample 1</strong></p>
<p><img src="./22974/file/11mkCv6I.png" alt="" width="298" height="214"></p>
<p>&nbsp;</p>
<p><strong>sample 2</strong></p>
<p><img src="./22974/file/9wYARpKn.png" alt=""></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The input contains multiple cases terminated with EOF.<br>For each case, first line contains two integers: m, n.<br>(3 &lt;= m &lt;= 500, 0 &lt;= n &lt;= 500)<br>Next m lines each contain two integers: Xfi, Yfi ----coordinate of the fence¡¯s ith vertex, in Counterclockwise order.<br>Next n lines each contain two integers: Xti, Yti ----coordinate of the ith tree.<br>It¡¯s guaranteed that all trees were strictly in the fence, and the fence doesn¡¯t intersect or touch itself.<br>The absolute value of the coordinates doesn¡¯t exceed 10000.</p>
<h3>Output</h3>
<p>For each case output the perimeter of the rubber-band with three digits after the dot.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>8 2<br>0 0<br>30 0<br>30 20<br>20 20<br>20 10<br>10 10<br>10 20<br>0 20<br>5 15<br>25 15<br><br>12 5<br>5 5<br>5 20<br>-5 20<br>-5 5<br>-20 5<br>-20 -5<br>-5 -5<br>-5 -20<br>5 -20<br>5 -5<br>20 -5<br>20 5<br>0 0<br>0 17<br>0 -17<br>17 0<br>-17 0<br><br><strong>Output:</strong><br>Case #1: 48.284<br>Case #2: 104.000<br><br></pre>