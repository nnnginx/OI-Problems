<p>On his birthday, Perrin received a very unusual puzzle. It consists of an NxN grid of lightbulbs, all of them initially at the off state. The goal is to turn on some of the lights, such that there is exactly one lit bulb in each row, and exactly one lit bulb in each column. Normally this would be an easy exercise, but this puzzle has an additional constraint. For each lightbulb, there is exactly one critical moment of time that the lightbulb can be switched on. As Perrin is a busy man, he does not want to spend a lot of time on the puzzle. Help Perrin calculate the minimum time taken to achieve the goal. Note that the time taken to solve the puzzle is defined as the time difference between the first and the last switching on events.</p>
<h3>Input</h3>
<p>The first line contains T, the number of test cases. T test cases follow.<br>The first line of each test case contains a single integer N. N lines follow each containing N integers. The j th integer in the i th of these lines represent the critical time for the bulb in row i, column j.<br>For any two lightbulbs, the critical times will be different</p>
<h3>Output</h3>
<p>Output T lines, each with one integer as the answer for the corresponding test case.</p>
<h3>Constraints</h3>
<p>T &lt;= 100<br>1 &lt;= N &lt;= 50<br>0 &lt;= critical times &lt;= 1000000000</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>2<br>3 6<br>9 8<br>4<br>10 41 38 66<br>91 13 95 70<br>49 32 43 52<br>51 98 36 19

<strong>Output:</strong>
3<br>29<br></pre>
<h3><strong>Explanation:</strong></h3>
<p>In the first test case, one can either turn on bulbs at times 3 and 8, or at times 6 and 9.Time taken to solve is 5 for the first option and 3 for the second. So the answer is 3.</p>
<p>In the second test case, one optimal way is to turn on lights at times 41,43,51,70.</p>