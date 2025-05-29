<p>
<img src="./23948/file/nie4Y27P.png">
</p>
<p>
The only printer in the computer science students' union is
experiencing an extremely heavy workload. Sometimes there are
a hundred jobs in the printer queue and you may have to wait
for hours to get a single page of output.
</p>
<p>
Because some jobs are more important than others, the Hacker General
has invented and implemented a simple priority system for the print
job queue.  Now, each job is assigned a priority between 1 and 9 (with 9 being
the highest priority, and 1 being the lowest), and the printer
operates as follows.

</p><ul>
<li> The first job <em>J</em> in queue is taken from the queue.
</li><li> If there is some job in the queue with a higher priority than job <em>J</em>, then move <em>J</em> to the end of the queue without printing it.

</li><li> Otherwise, print job <em>J</em> (and do not put it back in the queue).
</li></ul>
<p></p>
<p>
In this way, all those important muffin recipes that the Hacker
General is printing get printed very quickly.  Of course, those
annoying term papers that others are printing may have to wait for
quite some time to get printed, but that's life.
</p>
<p>
Your problem with the new policy is that it has become quite tricky to
determine when your print job will actually be completed.  You decide
to write a program to figure this out.  The program will be given the
current queue (as a list of priorities) as well as the position of
your job in the queue, and must then calculate how long it will take
until your job is printed, assuming that no additional jobs will be
added to the queue.  To simplify matters, we assume that printing a
job always takes exactly one minute, and that adding and removing jobs
from the queue is instantaneous.
</p>
<h3>Input</h3>
<p>
One line with a positive integer: the number of test cases (at most 100). Then
for each test case:
</p><ul>
<li>
One line with two integers <em>n</em> and <em>m</em>, where <em>n</em>

is the number of jobs in the queue (1 ¡Ü <em>n</em> ¡Ü 100) and
<em>m</em> is the position of your job (0 ¡Ü m ¡Ü n-1).  The
first position in the queue is number 0, the second is number 1, and
so on.
</li><li>
One line with <em>n</em> integers in the range 1 to 9, giving the priorities
of the jobs in the queue.  The first integer gives the priority of the
first job, the second integer the priority of the second job, and so
on.

</li></ul>
<p></p>
<h3>Output</h3>
<p>For each test case, print one line with a single integer; the number
of minutes until your job is completely printed, assuming that no
additional print jobs will arrive.
</p>
<h3>Example</h3>

<pre><b>Input:</b>
3
1 0
5
4 2
1 2 3 4
6 0
1 1 9 1 1 1

<b>Output:</b>
1
2
5
</pre>