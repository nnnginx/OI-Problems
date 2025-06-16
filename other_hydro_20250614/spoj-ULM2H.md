<p><span style="font-family: 'Times New Roman'; font-size: 16px;">The Museum of Modern Art has a really exciting exhibition: a kind of a longish hall composed of a sequence of quadratic-shaped rooms. Each room is equipped with a water fountain. Each fountain is characterized by a number&nbsp;</span><em>p</em><span style="font-family: 'Times New Roman'; font-size: 16px;">&nbsp;and acts independent of the others. It will be turned on for exactly&nbsp;</span><em>p</em><span style="font-family: 'Times New Roman'; font-size: 16px;">&nbsp;seconds, then it will be turned off for exactly&nbsp;</span><em>p</em><span style="font-family: 'Times New Roman'; font-size: 16px;">&nbsp;seconds, then on again, then off again, and so on for good. However, different fountains may have different values of&nbsp;</span><em>p</em><span style="font-family: 'Times New Roman'; font-size: 16px;">. And even if they share the same value, they still may perform not identically, for they might have been started at different times.</span></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">You stand in front of the first room, and want to cross the hall to the other end. Each of your steps takes exactly 1 second. You are able to move one room forward (unless you already reached the other end), one room backward (unless you are at the beginning), or just stay at your current position. Calculate the shortest time to reach the other end, if it is possible at all.</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">Since you do not want to get wet, you can only move into a room where the water fountain will be off during the second after your step. For example, suppose that the fountain in the next room behaves so, that it is on at times 0, 1, 2, then off at times 3, 4, 5, 6, then on at times 7, 8, 9, 10, then off again (which indicates&nbsp;<em>p=4</em>&nbsp;with an offset of 7). Then, you can move at time 2 into the room, arriving there at time 3, when the fountain is off. But you cannot move at time 6 into the room, because at time 7 it will be on.</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><strong>Input Specification</strong></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">The input contains several test cases. Each test case starts with the number of fountains&nbsp;<em>n</em>. Input is terminated by&nbsp;<em>n=0</em>. Otherwise,&nbsp;<em>1¡Ün¡Ü100</em>. Then follow&nbsp;<em>n</em>&nbsp;numbers&nbsp;<em>p<sub>i</sub></em>&nbsp;denoting the time each fountain is on and off, where&nbsp;<em>0¡Üp<sub>i</sub>¡Ü10</em>. A value of&nbsp;<em>0</em>&nbsp;for&nbsp;<em>p<sub>i</sub></em>&nbsp;indicates that fountain&nbsp;<em>i</em>&nbsp;is out of order (i.e. constantly off). Then follow&nbsp;<em>n</em>&nbsp;numbers&nbsp;<em>q<sub>i</sub></em>&nbsp;denoting the offset of each fountain, where&nbsp;<em>0¡Üq<sub>i</sub>&lt;2*p<sub>i</sub></em>, unless the fountain is out of order, in which case&nbsp;<em>q<sub>i</sub></em>&nbsp;is meaningless. Otherwise it means that fountain&nbsp;<em>i</em>&nbsp;will be on at time&nbsp;<em>q<sub>i</sub></em>, but off just one second before.</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><strong>Output Specification</strong></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">For each test case output on a line a single number&nbsp;<em>t</em>&nbsp;denoting the shortest time needed to reach the end of the hall (i.e. to enter the place after the last room). Assume, that you are in front of the first room at time&nbsp;<em>0</em>&nbsp;(i.e. you can enter the first room at time&nbsp;<em>1</em>, if the fountain is off at time&nbsp;<em>1</em>). If it is impossible to go through the hall of fountains, print&nbsp;<em>0</em>&nbsp;instead.</p>
<table style="margin: auto; width: 100%;" border="0" cellpadding="0">
<tbody>
<tr>
<td valign="TOP">
<p style="font-family: Times, serif; text-align: justify;"><strong>Sample Input</strong></p>
<p style="font-family: Times, serif; text-align: justify;"><tt></tt></p>
<pre><tt>3
0 0 0
0 0 0
4
6 3 3 4
2 3 0 4
2
1 1
0 0
0
</tt></pre>
</td>
<td valign="TOP">
<p style="font-family: Times, serif; text-align: justify;"><strong>Sample Output</strong></p>
<p style="font-family: Times, serif; text-align: justify;"><tt></tt></p>
<pre><tt>4
11
0
</tt></pre>
</td>
</tr>
</tbody>
</table>