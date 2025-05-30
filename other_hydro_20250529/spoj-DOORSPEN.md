<p>The organizers of the Annual Computing Meeting have invited a number of vendors to set up booths in a large exhibition hall during the meeting to showcase their latest products. As the vendors set up their booths at their assigned locations, they discovered that the organizers did not take into account an important fact �� each vendor supports either the Doors operating system or the Penguin operating system, but not both. A vendor supporting one operating system does not want a booth next to one supporting another operating system.

Unfortunately the booths have already been assigned and even set up. There is no time to reassign the booths or have them moved. To make matter worse, these vendors in fact do not even want to be in the same room with vendors supporting a different operating system.

Luckily, the organizers found some portable partition screens to build a wall that can separate the two groups of vendors. They have enough material to build a wall of any length. The screens can only be used to build a straight wall. The organizers need your help to determine if it is possible to separate the two groups of vendors by a single straight wall built from the portable screens. The wall built must not touch any vendor booth (but it may be arbitrarily close to touching a booth). This will hopefully prevent one of the vendors from knocking the wall over accidentally. 

</p><h3>Input</h3>
<p>The input consists of a number of cases. Each case starts with 2 integers on a line separated by a single space: D and P, the number of vendors supporting the Doors and Penguins operating system, respectively (1 �� D, P �� 500). The next D lines specify the locations of the vendors supporting Doors. This is followed by P lines specifying the locations of the vendors supporting Penguins. The location of each vendor is specified by four positive integers: x1, y1, x2, y2. (x1, y1) specifies the coordinates of the southwest corner of the booth while (x2, y2) specifies the coordinates of the northeast corner. The coordinates satisfy x1 &lt; x2 and y1 &lt; y2. All booths are rectangular and have sides parallel to one of the compass directions. The coordinates of the southwest corner of the exhibition hall is (0, 0) and the coordinates of the northeast corner is (15000, 15000). You may assume that all vendor booths are completely inside the exhibition hall and do not touch the walls of the hall. The booths do not overlap or touch each other.

The end of input is indicated by D = P = 0. 

</p><h3>Output</h3>
<p>For each case, print the case number (starting from 1), followed by a colon and a space. Next, print the sentence:

It is possible to separate the two groups of vendors.

if it is possible to do so. Otherwise, print the sentence:

It is not possible to separate the two groups of vendors.

Print a blank line between consecutive cases. 

</p><h3>Example</h3>

<pre><b>Input:</b>
3 3
10 40 20 50
50 80 60 90
30 60 40 70
30 30 40 40
50 50 60 60
10 10 20 20
2 1
10 10 20 20
40 10 50 20
25 12 35 40
0 0


<b>Output:</b>
Case 1: It is possible to separate the two groups of vendors.

Case 2: It is not possible to separate the two groups of vendors.

</pre>