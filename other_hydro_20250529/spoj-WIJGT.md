<meta http-equiv="Content-Type" content="text/html; charset=iso-8859-1">
<title>Documento sin t¨ªtulo</title>



<div align="justify">
  <p>Indiana Jones is in a deserted city, annihilated during a war. Roofs of all houses have been destroyed 
    and only portions of walls are still standing. The ground is so full of mines that the only safe way to
    move around the city is walking over the remaining walls. The mission of our hero is to save a person
    who is trapped in the city. In order to move between two walls which are not connected Indiana Jones
    thought of taking with him a wooden board which he could place between the two walls and then
    cross from one to the other.</p>
  <p align="center"><img src="/content/boodah:WIJGT.JPG" width="371" height="251"> </p>
  <p align="justify">Initial positions of Indiana Jones and the trapped person are both on some section of the walls. 
    Besides, walls are either in the direction South-North or West-East.
    You will be given a map of the city remains. Your mission is to determine the minimum length of the
    wooden board Indiana Jones needs to carry in order to get to the trapped person.<br>
  </p>
  <p align="justify"><strong>Input</strong><br>
    Your program should process several test cases. Each test case starts with an integer
    N
    indicating the
    number of wall sections remaining in the city (2
&lt;=
N
&lt;=
1000). Each of the next
N
lines describes a wall
section. The first wall section to appear is the section where Indiana Jones stands at the beginning.
The second section to appear is the section where the trapped person stands. Each wall section
description consists of three integers
X
,
Y
and
L
(¨C10000
&lt;=
X
,
Y
,
L
&lt;= 10000), where
X
an
Y
define
either the southernmost point of a wall section (for South-North sections) or the westernmost point<br>
(for West-East wall sections). The value of
L
determines the length and direction of the wall: if
L
&gt;
0,
the section is West-East, with length
L
; if
L&lt; 0, the section is North-South, with length
    |
    L
    |
    . The end
    of input is indicated by
    N
    = 0.<br>
  </p>
  <p align="justify"><strong>Output</strong><br>
    For each test case in the input your program should produce one line of output, containing a real value
  representing the length of the wooden board Indiana Jones must carry. The length must be printed as a real number with two-digit precision, and the last decimal digit must be rounded. The input will not
  contain test cases where differences in rounding are significant.</p>
  <p align="justify"><strong>Sample input</strong><br>
    14<br>
    1 1 5<br>
    6 8 2<br>
    7 2 -2<br>
    5 3 3<br>
    2 5 2<br>
    2 3 2<br>
    2 3 -2<br>
    4 3 -2<br>
    0 7 1<br>
    1 8 2<br>
    3 6 -2<br>
    4 7 2<br>
    6 6 1<br>
    6 6 -2<br>
    3<br>
    -10 0 20<br>
    -5 1 10<br>
    50 50 100<br>
  0</p>
  <p align="justify"><strong>Output for the sample input</strong><br>
    1.41<br>
  1.00</p>
</div>