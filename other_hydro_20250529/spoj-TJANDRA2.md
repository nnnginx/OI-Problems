<p>The 07 February 2013 was Tjandra's 19th birthday,
 I want to make a present to him and all other great SPOJ solvers by the way.
So I set this HARD puzzle problem extension of the yet good
 <a href="http://www.spoj.com/problems/TJANDRAS/">TJANDRAS</a>.
<br>
<br>
<b>Warning :</b> To solve the 'easy' task, you need a O(N^0.5) algorithm,
 but to solve this 'harder' task, you need something around O(N^0.34),
 so it's not about optimization tricks!!!
<br>
Please note that I checked my data with my 'semi-brute-force'-O(N^0.5)-Python3-solution and it took me 16 hours.
<br>
<br>
Don't forget to have fun with that problem!
</p>

<h3>The Game</h3>
<p>
This game/puzzle is about matches, given N matches,
 your task is to arrange the matches (not necessarily all)
 such that the number of rectangles (any size) is maximum.
</p>

<h3>Input</h3>
<p>
The input begins with the number T of test cases in a single line.<br>
In each of the next T lines there are one integer N.
</p>


<h3>Output</h3>
<p>
For each test case, on a single line, print the required answer
 (maximum number of rectangles).
</p>


<h3>Example</h3>
<pre><b>Input:</b>
6
3
4
8
12
15
987654321123456789

<b>Output:</b>
0
1
3
9
12
60966316127114768913148159571503206
</pre>

<h3>Constraints</h3>
<pre>1 &lt; T �� 100
1 &lt; N �� 10^18
</pre>
<p>The T numbers N are uniform-randomly chosen in the range.</p>

<h3>Explanations</h3>
<p>
First test case:<br>
No rectangle can be formed with only 3 matches.
<br>

<br>
Second test case:<br>
Only one rectangle can be formed with 4 matches.
<br>

<br>
Third test case:<br>
There are max 3 rectangles.<br>
(2 size 1x1, 1 size 2x1) can be formed with number of matches �� 8,
 here is one of the matches formation:
<br>
<img title="Case 3" src="../../content/francky:tj-case3" alt="Case 3 - Fig">
<br>

<br>
Fourth test case:<br>
There are max 9 rectangles.<br>
(4 size 1x1, 2 size 2x1, 2 size 1x2, 1 size 2x2) can be formed with number of matches �� 12, here is one of the formation:
<br>
<img title="Case 4" src="../../content/francky:tj-case4" alt="Case 4 - Fig">
<br>

<br>
Fifth test case:<br>
there are max 12 rectangles.<br>
(5 size 1x1, 3 size 2x1, 1 size 3x1, 2 size 1x2, 1 size 2x2) can be formed with number of matches �� 15, here is one of the formation:
<br>
<img title="Case 5" src="../../content/francky:tj-case5" alt="Case 5 - Fig">
<br>

<br>
Sixth test case:<br>
You have to figure by yourself how to compute that in the required time.
</p>