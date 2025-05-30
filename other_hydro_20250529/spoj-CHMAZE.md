<p>Luke Skywalker and his sister/love interest Leia are trying to get through a killer maze. And I
mean killer! Every time step, the boundaries change. If our twins/lovebirds ever visit a square the
same time a boundary appears, they��re toast. There is no need to panic; the Force will guide them
through the maze, and they will not die. However, the Force needs to know what advice to give
and is therefore asking you for help.<br><br>
Luke and Leia begin in the northwest corner of a maze. They want to make it to the southeast
corner of the maze. At any given time step, Luke and Leia can move one square north, south, east,
or west, or they can stay where they are. At every time step, the boundaries of the maze change:
there is a finite list of patterns; if Luke and Leia are still in the maze when the list of patterns
is exhausted, the maze cycles through again from the beginning of the list. You need to compute
whether Luke and Leia can make it to the southeast corner of the maze, and, if so, the minimum
number of time steps necessary for them to get there. Remember, the Force is counting on you! If
you give the Force bad advice, we��ll have to wait around for A Newer Hope and Force Knows how
long that could take!


</p><h3>Input</h3>
<p>The input consists of several test cases. Each case (but the last) will begin with a line containing
three decimal integers. The first is the number of rows in the maze; the second is the number of
columns in the maze; the third is the number of patterns in the list. The first two numbers will
be inclusively between 1 and 20; the third will be inclusively between 1 and 10. The integers will
be separated by exactly one space and will be followed by one <eol>. Immediately following this
line will be a number of patterns, equal to the number specified on the first line. Each pattern will
consist of r lineas each containing c characters, where r is the number of rows and c is the number
of columns indicated on the first line. Each character will be either 0 (indicating no boundary) or
1 (indicating a boundary). Each line will be terminated by <eol>, and an extra <eol> will follow
each pattern. The northwest corner of the first pattern will always be zero, since Luke and Leia
will be starting from there. The last case will be three zeros, separated by exactly one space and
followed by exactly one <eol>. This case is not to be processed; it indicates the end of input.


</eol></eol></eol></eol></p><h3>Output</h3>
<p>The output cases are to appear in the same order in wich they appear in the input. Each output
case should be of the form <i>Case c: Luke and Leia can escape in s steps.</i> or of the form
<i>Case c: Luke and Leia cannot escape.</i> c and s are decimal integers. c in the number of the
case being processed (starting with 1) and s is the minimum number of time steps Luke and Leia
require to reach the southeast corner. Each line should be terminated by exactly one <eol>.


</eol></p><h3>Example</h3>

<pre><b>Input:</b>
5 5 1
00000
00000
00000
00000
00000
5 5 2
00000
00000
00000
00000
00000
01110
01110
11111
01110
01110
0 0 0

<b>Output:</b>
Case 1: Luke and Leia can escape in 8 steps.
Case 2: Luke and Leia cannot escape.

</pre>