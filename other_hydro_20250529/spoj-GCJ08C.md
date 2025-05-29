<p>Near the planet Mars, in a faraway galaxy eerily similar to our own, there is a fight to the death between the imperial forces and the rebels. The rebel army has N ships which we will consider as points (xi, yi, zi). Each ship has a receiver with power pi. The rebel army needs to be able to send messages from the central cruiser to all the ships, but they are tight on finances, so they cannot afford a strong transmitter.
<br><br>
If the cruiser is placed at (x, y, z), and one of the other ships is at (xi, yi, zi) and has a receiver of power pi, then the power of the cruiser's transmitter needs to be at least:
<br><br>
(|xi - x| + |yi - y| + |zi - z|) / pi
<br><br>
Your task is to find the position for the cruiser that minimizes the power required for its transmitter, and to output that power. 

</p><h3>Input</h3>
<p>The first line of input gives the number of cases, T. T test cases follow.
<br><br>
Each test case contains on the first line the integer N, the number of ships in the test case.
<br><br>
N lines follow, each line containing four integer numbers xi, yi, zi and pi, separated by single spaces. These are the coordinates of the i-th ship, and the power of its receiver. There may be more than one ship at the same coordinates.
<br><br>1 ¡Ü T ¡Ü 20
<br>0 ¡Ü xi, yi, zi ¡Ü 10^6
<br>1 ¡Ü pi ¡Ü 10^6
<br>1 ¡Ü N ¡Ü 1000

</p><h3>Output</h3>
<p>For each input case, you should output:
<br><br>
Case #X: Y
<br><br>
where X is the number of the test case and Y is the minimal power that is enough to reach all the fleet's ships. Answers with a relative or absolute error of at most 10-6 will be considered correct. 

</p><h3>Example</h3>

<pre><b>Input:</b>
3
4
0 0 0 1
1 2 0 1
3 4 0 1
2 1 0 1
1
1 1 1 1
3
1 0 0 1
2 1 1 4
3 2 3 2

<b>Output:</b>
Case #1: 3.500000
Case #2: 0.000000
Case #3: 2.333333
</pre>