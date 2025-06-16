<p><em>Original statement in spanish at <a href="http://www.dc.uba.ar/events/icpc/download/problems/taip2011-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/taip2011-problems.pdf</a></em></p>
<p>As we all know, Humberto is really lazy. He is so lazy that he sticks his nose out of the window so that the wind will blow it for him. Obviously, he hasn't worked at all in his whole life. However, he got lucky and won a lot of money in the lottery. With some of that money he bought an empty field, and made build several houses inside of it, where he moved with his family and friends. Thus, Humberto can go in a straight line from any point in his field to any other, without having to make detours because of urban design (for the sake of simplicity, we consider the objects in Humberto's field as dots, so they don't interfere in Humberto's way).</p>
<p>Sadly, that was not enough for Humberto, so in order to walk even less he decided to have installed some catapults in strategic points of his field. Each catapult can send him from the point where it is installed, to any point at a certain fixed distance (that depends on the range of the catapult).</p>
<p>But, in spite of simplifying his life, the catapults made the task of choosing a way in the field a real headache, because Humberto wants to walk as less as possible. As tired as he is of all his problems, he decided to use the rest of his money to hire you to tell him the minimum distance he has to walk to move from a given point in the field to another.</p>
<h3>Input</h3>
<p>The input contains several test cases. Each test case is described in several lines. The first line contains five integers <strong>N</strong>, <strong>P_X</strong>, <strong>P_Y</strong>, <strong>L_X</strong> and <strong>L_Y</strong>. <strong>N</strong> represents the number of catapults in the field (1 &lt;= <strong>N</strong> &lt;= 100). The pair (<strong>P_X</strong>, <strong>P_Y</strong>) indicates the coordinates in the XY plane ot the starting point for Humberto, while the pair (<strong>L_X</strong>, <strong>L_Y</strong>) indicates analogously the destination point (1 &lt;= <strong>P_X</strong>, <strong>P_Y</strong>, <strong>L_X</strong>, <strong>L_Y</strong> &lt;= 10<sup>9</sup>). Each of the next <strong>N</strong> lines describes a different catapult, using three integers <strong>C_X</strong>, <strong>C_Y</strong> and <strong>F</strong>, that indicate the point (<strong>C_X</strong>, <strong>C_Y</strong>) where the catapult of strength <strong>F</strong> is installed. This means that Humberto may move, without walking, from the point (<strong>C_X</strong>, <strong>C_Y</strong>) to any point in the plane that is at a distance of <em>exactly</em> <strong>F</strong> from (<strong>C_X</strong>, <strong>C_Y</strong>). Assume that in each test case all the points given in the plane are different. The end of the input is indicated by a single line containing the number -1 five times, and it should not be processed as a test case.</p>
<h3>Output</h3>
<p><strong>F</strong>or each test case, output a single line containing a rational number that represents the minimum distance Humberto has to walk in order to get from the starting point to the destination point, using some or none of the catapults. Round the answer to the nearest rational with two decimal digits. In case of a tie, round up. Print exactly two digits after the decimal point, even if that means ending the number with 0's.</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>1 10 10 20 10
11 10 9
1 20 10 10 10
11 10 9
2 1 1 12 1
3 1 6
8 1 5
1 12 12 1 1
6 6 9
5 10 10 1 1
3 3 7
8 3 7
8 8 7
3 8 7
5 5 5
-1 -1 -1 -1 -1
</pre>
<p><strong>Output:</strong></p>
<pre>1.00
10.00
4.00
10.41
5.11
</pre>