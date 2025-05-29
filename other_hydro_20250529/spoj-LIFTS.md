<p>Serj likes old games very much. Recently he has found one arcade game in his computer. When controlling the hero it is necessary to move on a map and collect various items. At a certain stage of the game Serj has faced an unexpected problem. To continue his adventures the hero should get past over a chasm. For this purpose it is possible to use consistently located lifts which look like horizontal platforms. Each lift moves up-down vertically between some levels. The hero can pass between the next adjacent platform, however it can be done only at the moment when they are at the same level. Similarly, passing from the edge of a chasm onto the lift and vice versa is only possible at the moment when the lift appears on the level of the edge. </p>
<p>
Each lift has a width equal to 4 meters. At the beginning the hero is in at a distance of two meters from the edge of a chasm. He should finish travel two meters after the opposite edge of the chasm. The hero moves at a speed of 2 meters a second. Thus, if the hero is in the initial position or in the center of the lift and wishes to pass to the next lift (or to descend from last lift onto the opposite edge of a chasm), he should begin movement exactly one second before they meet at one level. In two seconds the hero appears in the center of the next lift (or in the final position on the other side).</p>
<p>
The edges of the chasm are at the same level. For each lift the range of heights between which it moves, its initial position and the direction of movement at the initial moment are given. All lifts move with a speed of one meter a second. Find out whether the hero can get over to the opposite edge of the chasm, and if so what the minimal time required for this purpose is.
</p>
<img src="/content/turbo:lifts.png" alt="A sample illustration">

<h3>Input</h3>
<p><i>t</i> ¨C the number of test cases, then <i>t</i> test cases follows. <br>
[empty line]<br>
A test case begins with <i>n</i> - the number of lifts, a positive integer (<i>n</i> &lt;= 100), then n lines follow. The i-th line (<i>0 &lt; i &lt;= n</i>) contains four integers <i>li ui si di</i>, where:
<i>li</i> - lowest position of the lift, <i>ui</i> - highest position of the lift, 
<i>si</i> - initial position of the lift, 
<i>di</i> - initial direction of movement (1 means up, -1 means down); (-100 &lt;= <i>li</i> &lt;= <i>si</i> &lt;= <i>ui</i> &lt;= 100, <i>l1</i> &lt; <i>ui</i>).

</p><h3>Output</h3>
<p>For each test case output the minmal time in seconds, required to get to the opposite edge of the chasm. If it is impossible output -1.<br>

</p><h3>Example</h3>
<pre><b>Input:</b>
1

4
-1 2 1 -1
0 3 0 1
-4 0 0 -1
-2 1 0 -1
</pre>

<pre><b>Output:</b>
29
</pre>