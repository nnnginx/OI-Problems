<p>Starting from the number '1', every time you can choose a digit from the current number and add it to the number itself.  23, for example, could be changed into 25 or 26. To get 100, using the above scheme, paths A and B are both possible. A requires 21 steps, but B needs only 17 (which is also the minimum) <br><br>

A. 1-2-4-8-16-17-18-19-20-22-24-28-36-39-48-56-62-68-76-83-91-100<br>
B. 1-2-4-8-16-17-24-28-36-39-48-56-62-68-76-83-91-100<br><br>

C is another 17 step solution for 100.<br>
<br>
C. 1-2-4-8-16-22-24-28-36-39-48-56-62-68-76-83-91-100<br>
<br>

Now, you are given several numbers, for each number, print the minimum steps S and number of solutions T. As T could be quite large, you should print T%1000000007 instead.<br>

</p><h3>Input</h3>
<p>Each line of input contains a integer K as a test case. Input ends with End Of File.

</p><h3>Output</h3>
<p>For each test case print the minimum steps and solutions in a single line. If it's impossible to get the number, print "IMPOSSIBLE" instead. ( without the quotes ).

</p><h3>Example</h3>

<pre><b>Input:</b>
16
100
87

<b>Output:</b>
4 1
17 2
IMPOSSIBLE
</pre>

<h3>Constraints and Limits</h3>
<p>Number of test cases ¡Ü 100, 1 ¡Ü K ¡Ü 10^9.
</p>