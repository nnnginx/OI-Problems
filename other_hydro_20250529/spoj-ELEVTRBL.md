<p>You are on your way to your first job interview as a program tester, and you are already late. The interview is in a skyscraper and you are currently in  floor <i>s</i>, where you see an elevator. Upon entering the elvator, you learn that it has only two buttons, marked "UP <i>u</i>" and "DOWN <i>d</i>". You conclude that the UP-button takes the elevator <i>u</i> floors up (if there aren't enough floors, pressing the UP-botton does nothing, or at least so you assume), whereas the DOWN-button takes you <i>d</i> stories down (or none if there aren't enough). Knowing that the interview is at floor <i>g</i>, and that there are only <i>f</i> floors in the building, you quickly decide to write a program that gives you the amount of button pushes you need to perform. If you simply cannot reach the correct  floor, your program halts with the message "<tt>use the stairs</tt>". </p>

<p>
Given input <i>f</i>, <i>s</i>, <i>g</i>, <i>u</i> and <i>d</i> (floors, start, goal, up, down), find the shortest sequence of button presses you must press in order to get from <i>s</i> to <i>g</i>, given a building of floors, or output "<tt>use the stairs</tt>" if you cannot get from <i>s</i> to <i>g</i> by the given elevator.
</p>

<h3>Input</h3>
<p>The input will consist of one line, namely <tt>f s g u d</tt>, where 1 &lt;= s, g &lt;= f &lt;= 1000000 and 0 &lt;= u, d &lt;= 1000000. The  floors are one-indexed, i.e. if there are 10 stories, s and g be in [1; 10].</p>

<h3>Output</h3>
<p>You must reply with the minimum numbers of pushes you must make in order to get from s to g, or output "<tt>use the stairs</tt>" if it is impossible given the conguration of the elevator.</p>

<h3>Example</h3>

<pre><strong>Input:</strong>
10 1 10 2 1

<strong>Output:</strong>
6</pre>

<pre><strong>Input:</strong>
100 2 1 1 0 

<strong>Output:</strong>
use the stairs</pre>