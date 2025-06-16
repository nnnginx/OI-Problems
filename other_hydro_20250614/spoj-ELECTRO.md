<p>Scientist Frank, majoring in electrochemistry, has developed line-shaped strange electrodes called F-electrodes.
During being activated, each F-electrode causes a special potential on and between the two lines touching the
F-electrode's endpoints at a right angle. Then electrically-charged particles located inside the potential area get
to move in the direction parallel to the potential boundary (i.e. perpendicular to the F-electrode), either toward or
against F-electrode. The moving direction can be easily controlled between the two possibles; it is also possible
to get particles to pass through F-electrodes. In addition, unlike ordinary electrodes, F-electrodes can affect
particles even infinitely far away, as long as those particles are located inside the potential area. On the other
hand, two different F-electrodes cannot be activated at a time, since their potentials conflict strongly.
</p><p>We can move particles on our will by controlling F-electrodes. However, in some cases, we cannot lead them to
the desired positions due to the potential areas being limited. To evaluate usefulness of F-electrodes from some
aspect, Frank has asked you the following task: to write a program that finds the shortest distances from the
particles' initial positions to their destinations with the given sets of F-electrodes.
</p><center><img src="/content/crazyb0y:ELECTRO.jpg"></center>

<h3>Input</h3>
<p>The input consists of multiple test cases. The first line of each case contains N(1 ¡Ü N ¡Ü 100) which represents
the number of F-electrodes. The second line contains four integers xs, ys, xt and yt, where (xs, ys) and (xt , yt)
indicate the particle¡¯s initial position and destination. Then the description of N F-electrodes follow. Each line
contains four integers F<sub>xs</sub>, F<sub>ys</sub>, F<sub>xt</sub> and F<sub>yt</sub>, where (F<sub>xs</sub>, F<sub>ys</sub>) and (F<sub>xt</sub> , F<sub>yt</sub>) indicate the two endpoints of an
F-electrode. All coordinate values range from 0 to 100 inclusive.
</p><p>The input is terminated by a case with N = 0.

</p><h3>Output</h3>
<p>Your program must output the case number followed by the shortest distance between the initial position to
the destination. Output "<tt>Impossible</tt>" (without quotes) as the distance if it is impossible to lead the elementary
particle to the destination. Your answers must be printed with five digits after the decimal point.</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
2 1 2 2
0 0 1 0
0 1 0 2
0

<b>Output:</b>
Case 1: 3.00000
</pre>