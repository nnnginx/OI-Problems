<p>A new type of mobile robot has been developed for environmental earth observation. It moves around on the ground, acquiring and recording various sorts of observational data using high precision sensors. Robots of this type have short range wireless communication devices and can exchange observational data with ones nearby. They also have large capacity memory units, on which they record data observed by themselves and those received from others.

</p><p></p><p>
Figure 1 illustrates the current positions of three robots A, B, and C and the geographic coverage of their wireless devices. Each circle represents the wireless coverage of a robot, with its center representing the position of the robot. In this figure, two robots A and B are in the positions where A can transmit data to B, and vice versa. In contrast, C cannot communicate with A or B, since it is too remote from them. Still, however, once B moves towards C as in Figure 2, B and C can start communicating with each other. In this manner, B can relay observational data from A to C. Figure 3 shows another example, in which data propagate among several robots instantaneously. 

</p><center><img src="/content/steinersp:Mobile1.gif" alt="subir imagenes" border="0"><br>Figure 1: The initial configuration of three robots</center>

<p>
</p><center><img src="/content/steinersp:Mobile2.gif" alt="subir imagenes" border="0"><br>Figure 2: Mobile relaying</center>

<p>
</p><center><img src="/content/steinersp:Mobile3.gif" alt="subir imagenes" border="0"><br>Figure 3: Instantaneous relaying among multiple robots</center>

<p></p><p>
As you may notice from these examples, if a team of robots move properly, observational data quickly spread over a large number of them. Your mission is to write a program that simulates how information spreads among robots. Suppose that, regardless of data size, the time necessary for communication is negligible.
</p><h3>Input</h3>
<p>The input consists of multiple datasets, each in the following format.

</p><p></p><p>
    <i>N T R<br>
    nickname and travel route of the first robot<br>
    nickname and travel route of the second robot<br>
    ...<br>
    nickname and travel route of the N-th robot</i><br>

</p><p></p><p><br>
The first line contains three integers <i>N, T, and R</i> that are the number of robots, the length of the simulation period, and the maximum distance wireless signals can reach, respectively, and satisfy that 1 &lt;= <i>N</i> &lt;= 100, 1 &lt;= <i>T</i> &lt;= 1000, and 1 &lt;= <i>R</i> &lt;= 10.

</p><p></p><p>
The <i>nickname and travel route</i> of each robot are given in the following format.

</p><p></p><p>
    <i>nickname<br>
    t0 x0 y0<br>
    t1 vx1 vy1<br>
    t2 vx2 vy2<br>
    ...<br>
    tk vxk vyk</i><br>

</p><p></p><p>
<i>Nickname</i> is a character string of length between one and eight that only contains lowercase letters. No two robots in a dataset may have the same nickname. Each of the lines following nickname contains three integers, satisfying the following conditions.

</p><p></p><p>
    <i>0 = t<sub>0</sub> &lt; t<sub>1</sub> &lt; ... &lt; t<sub>k</sub> = T<br>
    -10 &lt;= vx<sub>1</sub>, vy<sub>1</sub>, ..., vx<sub>k</sub>, vy<sub>k</sub>&lt;= 10</i><br>

</p><p></p><p>
A robot moves around on a two dimensional plane. (x<sub>0</sub>, y<sub>0</sub>) is the location of the robot at time 0. From time t<sub>i-1</sub> to t<sub>i</sub> (0 &lt; i &lt;= k), the velocities in the x and y directions are vx<sub>i</sub> and vy<sub>i</sub>, respectively. Therefore, the travel route of a robot is piecewise linear. Note that it may self-overlap or self-intersect.

</p><p></p><p>
You may assume that each dataset satisfies the following conditions.

</p><ul>
<li> The distance between any two robots at time 0 is not exactly R.
</li><li> The x- and y-coordinates of each robot are always between -500 and 500, inclusive.
</li><li> Once any robot approaches within R + 10<sup>-6</sup>. of any other, the distance between them will become smaller than R - 10<sup>-6</sup>. while maintaining the velocities.
</li><li> Once any robot moves away up to R - 10<sup>-6</sup>. of any other, the distance between them will become larger than R + 10<sup>-6</sup>. while maintaining the velocities.
</li><li> If any pair of robots mutually enter the wireless area of the opposite ones at time t and any pair, which may share one or two members with the aforementioned pair, mutually leave the wireless area of the opposite ones at time t', the difference between t and t' is no smaller than 10<sup>-6</sup>. time unit, that is, |t - t' | &gt;= 10<sup>-6</sup>. 
</li></ul>

<p></p><p>
A dataset may include two or more robots that share the same location at the same time. However, you should still consider that they can move with the designated velocities.

</p><p></p><p>
The end of the input is indicated by a line containing three zeros. 

</p><h3>Output</h3>
<p>
For each dataset in the input, your program should print the nickname of each robot that have got until time <i>T</i> the observational data originally acquired by the first robot at time 0. Each nickname should be written in a separate line in dictionary order without any superfluous characters such as leading or trailing spaces.

</p><h3>Example</h3>

<pre><b>Input:</b>
3 5 10
red
0 0 0
5 0 0
green
0 5 5
5 6 1
blue
0 40 5
5 0 0
3 10 5
atom
0 47 32
5 -10 -7
10 1 0
pluto
0 0 0
7 0 0
10 3 3
gesicht
0 25 7
5 -7 -2
10 -1 10
4 100 7
impulse
0 -500 0
100 10 1
freedom
0 -491 0
100 9 2
destiny
0 -472 0
100 7 4
strike
0 -482 0
100 8 3
0 0 0

<b>Output:</b>
blue
green
red
atom
gesicht
pluto
freedom
impulse
strike
</pre>