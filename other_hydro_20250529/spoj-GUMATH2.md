<p>Guardian is very weak at maths but still to compete in a certain exam he has to get good grades in mathematics this time. In the first class of the semester the Prof. asked students to find the number of ways deck (having N cards) could be shuffled that exactly one card is at the same position as before, and the students who successfully do this will be awarded with good marks in mid terms. Help Guardian solve this problem.</p>

<h3>Input</h3>
<p>The input begins with the number T of test cases in a single line.<br>
In each of the next T lines there are one integer N.</p>

<h3>Output</h3>
<p>For each test case you have to output on a single line the number of ways possible meeting the Prof.'s requirements.<br>
As the answer can be a huge number, simply output it modulo 10000009.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
3

<b>Output:</b>
3
</pre>

<p>
Let's say the initial deck configuration was {1,2,3}, then three possible shuffles are {1,3,2}, {2,1,3}, {3,2,1}.</p>

<h3>Constraints</h3>
<pre>1 &lt; T &lt; 10^4
0 &lt; N &lt; 10^18
</pre>
<p>@speed addicts : my C code ran in 0.08s, and my python3 code ran in 3.2s. (Total time with Pyramid cluster)<br>
Edit 19/I/2015 : Now the problem use Cube cluster, rejudge of my old code gave 0.01s with C, and 0.57s with Py3.2 (this last one ends in 0.42s with PY3.4)<br>
Edit 11-02-2017, after compiler changes : 0.00s with C, 0.22s with PY3.5. New TL.</p>