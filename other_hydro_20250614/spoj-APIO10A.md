<p style="text-align: center;"><strong>Commando</strong></p>
<p style="text-align: justify;"><br>You are the commander of a troop of n soldiers, numbered from 1 to n. For the battle ahead, you plan to divide these n soldiers into several com-mando units. To promote unity and boost morale, each unit will consist of a contiguous sequence of soldiers of the form (i, i+1, . . . , i+k).</p>
<p style="text-align: justify;">Each soldier i has a battle effectiveness rating xi . Originally, the battle effectiveness x of a commando unit (i, i+1, . . . , i+k) was computed by adding up the individual battle effectiveness of the soldiers in the unit. In other words, x = x<sub>i</sub> + x<sub>i</sub>+1 + · · · + x<sub>i</sub>+k .</p>
<p style="text-align: justify;"><br>However, years of glorious victories have led you to conclude that the battle effectiveness of a unit should be adjusted as follows: the adjusted effectiveness x is computed by using the equation x = ax<sup>2</sup> + bx + c, where a,b, c are known coefficients(a &lt; 0), x is the original effectiveness of the unit.</p>
<p style="text-align: justify;">&nbsp;</p>
<p style="text-align: justify;">Your task as commander is to divide your soldiers into commando units in order to maximize the sum of the adjusted effectiveness of all the units.</p>
<p style="text-align: justify;">&nbsp;</p>
<p style="text-align: justify;">For instance, suppose you have 4 soldiers, x<sub>1</sub> = 2, x<sub>2</sub> = 2, x<sub>3</sub> = 3, x<sub>4</sub> = 4. Further, let the coefficients for the equation to adjust the battle effectiveness of a unit be a = −1, b = 10, c = −20. In this case, the best solution is to divide the soldiers into three commando units: The first unit contains soldiers 1 and 2, the second unit contains soldier 3, and the third unit contains soldier 4. The battle effectiveness of the three units are 4, 3, 4 respectively, and the<br>adjusted effectiveness are 4, 1, 4 respectively. The total adjusted effectiveness for this grouping is 9 and it can be checked that no better solution is possible.</p>
<p style="text-align: justify;"><strong>Input format:</strong></p>
<p style="text-align: justify;">First Line of input consists <strong>number of cases T</strong>.</p>
<p style="text-align: justify;">Each case consists of three lines. The first line contains a positive integer n, the total number of soldiers. The second line contains 3 integers a, b, and c, the coefficients for the equation to adjust the battle effectiveness of a commando unit. The last line contains n integers x1 , x2 , . . . , xn , sepa-rated by spaces, representing the battle effectiveness of soldiers 1, 2, . . . , n, respectively.</p>
<p style="text-align: justify;"><strong>Constraints:</strong></p>
<p style="text-align: justify;">T&lt;=3</p>
<p style="text-align: justify;">n ≤ 1, 000, 000,</p>
<p style="text-align: justify;">−5 ≤ a ≤ −1</p>
<p style="text-align: justify;">|b| ≤ 10, 000, 000</p>
<p style="text-align: justify;">|c| ≤ 10, 000, 000</p>
<p style="text-align: justify;">1 ≤ xi ≤ 100.</p>
<p style="text-align: justify;">&nbsp;</p>
<p style="text-align: justify;"><br><strong>Output format</strong>:</p>
<p style="text-align: justify;">Output each answer in a single line.</p>
<p style="text-align: justify;"><br class="_mce_marker"></p>
<p style="text-align: justify;"><strong>Input:</strong></p>
<p style="text-align: justify;">3<br>4 <br>-1 10 -20 <br>2 2 3 4 <br>5<br>-1 10 -20<br>1 2 3 4 5<br>8<br>-2 4 3<br>100 12 3 4 5 2 4 2</p>
<p style="text-align: justify;"><strong>Output</strong>:</p>
<p style="text-align: justify;">9<br>13<br>-19884</p>
<p style="text-align: justify;">&nbsp;</p>
<p style="text-align: justify;"><strong>(Official dataset of APIO was NOT used in this problem.)</strong></p>