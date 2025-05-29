<p>
There are N cubes in a toy box which has 1-unit height, the width is double the height. The teacher organizes a tower-building game. The tower is built by the cubes. The height of the tower is H (h levels). The bottom of the tower contains M cubes; and for all above level, each must contains a number of cubes which is exactly 1 less than or greater than the number of cubes of the level right below it.  

Your task is to determine how many different towers can be there. Two towers are considered different if there is at least one number i (1&lt; i &lt;=H) so that the i'th level of one tower contains a different number of cubes to the i'th level of the other tower.

</p><h3>Input</h3>
<p>
The first line of input file is the integer number t ( 0 &lt; t &lt; 1002 ) , the number of test cases . Each test case in one line , the line contains three positive number N, H and M (N &lt;= 32767, H&lt;=60, M&lt;=10). 
</p><h3>Output</h3>
<p>
With each test case , write in one line , the total of different towers that can be founded. 

</p><h3>Example</h3>

<pre><b>Input:</b>
2
7 3 2
22 5 4
<b>Output:</b>
2
10
(* In the first test case , all the towers are : 2-1-2 , 2-3-2 . *)
</pre>