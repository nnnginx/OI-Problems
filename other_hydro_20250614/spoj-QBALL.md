<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">Xima has <strong>N</strong> balls arranged together in a line, the <strong>i</strong>-th&nbsp;<strong>(1 ¡Ü i ¡Ü N)</strong>&nbsp;ball has a value of <strong>A<sub>i</sub></strong>.</p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">Tzaph asks <strong>Q</strong> queries to Xima. There are two types of queries:</p>
<ul style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">
<li style="margin: 2px; padding: 1px;"><strong>1 i k</strong>: The value of the <strong>i</strong>-th&nbsp;ball is changed into <strong>k</strong>. In other words, <strong>A<sub>i</sub>&nbsp;=&nbsp;</strong><strong>k</strong><strong>. <strong>Take note that A<sub>i</sub>&nbsp;and k could have a same value. In this case, Xima shouldn't do anything.</strong></strong></li>
<li style="margin: 2px; padding: 1px;"><strong>2 i</strong>: Tzaph removes the <strong>i</strong>-th ball out from the line. Print the number of pairs <strong>(x, y)</strong> such that the <strong>x</strong><strong>-th</strong>&nbsp;and the <strong>y</strong><strong>-th</strong>&nbsp;ball is in the line,&nbsp;&nbsp;<strong>x &lt; y</strong>, and <strong>A<sub>x</sub>=A<sub>y</sub></strong>. After this query, Tzaph returns the <strong>i</strong>-th ball back to the line in it's original position.</li>
</ul>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">However, Tzaph asks too much queries and Xima has too much balls. Xima asks you to help him answer all of Tzaph's queries. Help him out!</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Input Format</strong></p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">The first line contains two integers <strong>N</strong> and <strong>Q</strong>.</p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">The second line consists of <strong>N</strong> integers, where the <strong>i</strong>-th integer represents <strong>A<sub>i</sub></strong>.</p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">The next <strong>Q</strong> lines represents the queries with format explained in the description.</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Output Format</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">For every second type of query, print the answer required.</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Sample Input 1</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">5 5<br> 1 2 3 4 5<br> 1 2 3<br> 1 5 4<br> 2 1<br> 1 2 4<br> 2 4</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Sample Output 1</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">2<br> 1</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Sample Input 2</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">1 3<br> 1<br> 2 1<br> 1 1 3<br> 2 1</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Sample Output 2</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">0<br> 0</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Constraints</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; "><strong>1 ¡Ü&nbsp;N, Q, A<sub>i</sub>, k ¡Ü&nbsp;10<sup>5</sup></strong></p>