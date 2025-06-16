<p>There are <strong>N</strong> toilets around Duck, each of them will begin to release <strong>O<sub>i</sub></strong> units of odors after <strong>i</strong> units of time. For example, there are three toilets producing 20, 10, 15 units of odors respectively. The first toilet will immediately release smells, the second one will release smells after 1 seconds and the third is after 2 seconds. So at the time 1, the total amount of released odors is 20 * 1 = 20, at time 2 is 20 * 2 + 10 * 1 = 50 and at time 3 is 20 * 3 + 10 * 2 + 15 * 1 =&nbsp; 95. Duck can only go to toilet when the absolute difference between the total amount of released odors at a certain time and his tolerance to odors <strong>M</strong> is minimized. Please find out at what time the difference is minimized. If there are two answers, choose the larger time.</p>
<p>After that, Duck will enter one of the toilets randomly. Given a string <strong>S</strong>, Duck knows which cubicles are available and which are occupied, 'x' means occupied and 'o' means available. Let the time that minimizes the difference be <strong>ANS</strong>, and the smallest power of 10 that equal or larger than ANS be <strong>P</strong>.<strong>&nbsp;</strong>Assuming the toilet entrance is located at the position <strong>floor(ANS / P * (len(S) - 1))</strong> of S, that is, the cubicle at that position is replaced by the entrance. You are required to select the best cubicle for Duck: available, maximizes the total distance between the nearest occupied cubicle on the left and right side as possible and it should be in the middle between the left nearest and right nearest occupied cuicle as possible (if no occupied cubicles next to the chosen range, you may assume there is an occupied cubicle on the most left and most right side and the entrance is also an occupied cubicle), and then as close to the entrance as possible. If there is more than one best choice, select the one on the right side of the entrance because Duck is always right. Please help him, he wants to excrete comfortably.</p>
<h3>Input</h3>
<p>The first line is the number of test cases <strong>T</strong>. (1 ¡Ü T ¡Ü&nbsp;50)</p>
<p>For each test case, it starts with two integers <strong>N</strong> (Number of toilets) and <strong>M</strong> (Duck's tolerance to odors). (1 ¡Ü N ¡Ü 500, N ¡Ü M ¡Ü 10<sup>18</sup>)</p>
<p>The next line is a string <strong>S</strong> consisting of 'x' and 'o', representing the status of cubicles (3 ¡Ü |S| ¡Ü 100)</p>
<p>Following N lines are the <strong>O<sub>i</sub></strong> units of odors released by i th toilet (1 ¡Ü O<sub>i</sub>&nbsp;¡Ü 10<sup>5</sup>)</p>
<p>It is guaranteed that in S, 'o' will appear at least twice, so the answer always exists.</p>
<h3>Output</h3>
<p>Print two integers in format 'x y' without quotes, where x is the time minimizes the absolute difference between the total amount of released odors at a certain time and M, y is the position of best cubicle counting from 0</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 98.4px; width: 1px; height: 1px; overflow: hidden;">2</div>2

4 78
ooxoxxoooxxxxxooooxoooo
2
13
1
5

5 35
xxoooxoooxx
1
2
3
4
5
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 98.4px; width: 1px; height: 1px; overflow: hidden;">5</div>
<strong>Output:</strong>
5 15
5 7<span style="white-space: normal;">
</span></pre>
<h3>Explanation</h3>
<p>In case one, the time is 5 because 2 * 5 + 13 * 4 + 1 * 3 + 5 * 2 = 75 minimizes the difference between it and 78. The length of S is 23, so the entrance is at position floor(5 / 10 * 22) = 11, and S becomes 'ooxoxxoooxxExxooooxoooo', and we can see that the cubicle at position 15 is available, as far away from the nearest occupied cubicles as possible, and as close to the entrance as possible.</p>
<p>In case two, at time 5, the minimized difference is 0. So S becomes 'xxoooEoooxx'. There are two best cubicles: position 3 and 7, and we choose the right one, so the answer is 7.</p>