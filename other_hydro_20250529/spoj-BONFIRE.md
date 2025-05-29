<p>Some great ideas are never implemented. This was the case with the
equatorial bonfire planned for the millenial celebration. Maybe the plan
will be rediscovered for the next turn of millenia. Before it is
completely forgotten we will tell you about it:
The idea was to put tarred logs and gun powder contiguously along the
equator and then ignite bonfires at various points of this gun powder belt
at various times. The fire would spread in both directions along the
equator and in the end, the whole equator would burn.
</p>

<p>
One concern of the architects of this celebration was what would be the
last place to catch fire and when would it happen?
</p>
<h3>Input</h3>
<p>The input file consists of at most 10 blocks, each specifying a separate proposal
for the equatorial bonfire. The first line of each block specifies the
speed of fire's advance in the degrees of longitude per hour. The next line
contains the number of bonfires <b>N ¡Ü 5000</b> along the equator. Each of the next
<b>N</b> lines contains two numbers specifying the time and the location of
a bonfire.
</p>

<p>
The time is given in hours from 12:00am GMT (all times are positive),
the location is given in the degrees of longitude (greater than -180
and less than or equal to 180). All numbers except <b>N</b> are given with
precision of at most 2 decimal places. Every block is followed by an empty
line. The last block is followed by an empty line and then a line
containing <tt>-1</tt>.
</p>
<h3>Output</h3>
<p>For every block in the input file, output a single line containing the
time and coordinate of the last place to catch fire. The time and the
coordinate should be in the same units and from the same range as input, but
with precision of 3 decimal places. If there are multiple solutions,
output the one which is the closest if you travel from the zero meridian
east (i.e. in the positive direction).
</p>
<h3>Example</h3>

<pre><b>Input:</b>

2
2
1 90
1 -90

10.0
3
1 40
2 45
6 -80

-1

<b>Output:</b>

46.000 0.000
15.500 -175.000
</pre>
<p>
Note that in the second case, the fire at 45 degrees actually starts 1.5 hours after 12:00am.
This of course does does not prevent anybody from igniting it again 2 hours after 12:00am.
</p>