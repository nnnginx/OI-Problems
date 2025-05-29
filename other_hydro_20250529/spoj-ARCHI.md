<p>Architecture, a tightrope walk between engineering and art! There are probably few invariants shared by the architectural styles around the world and throughout time. Precisely this diversity makes the domain so interesting and challenging.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img src="../../../content/imuteb:Architecture" alt="" width="356" height="341"></p>
<p>&nbsp;</p>
<p>Any domains may serve as sources of inspiration, mathematical shapes, nature, organisms and even arched slices of Swiss cheese J. Some of our university friends from architecture plan to participate in the prestigious Erect a Palace From Lines (EPFL) contest. This contest is about designing a huge single-floor palace by building horizontal and vertical walls inside the preset square fundament.</p>
<p>The students just finished their creative prototypes, and you are to revise their projects before they enter the contest. Some were obviously overwhelmed by the cryptographic protocol required for the palace description and do not know how many rooms their palace has. Walls are one unit thick and are described by their horizontal and vertical start and end positions. As the palace is huge, these coordinates are expressed in a base 26 system (the latin alphabet). Having overlapping walls is not a problem. For the encryption, read ��A�� as zero and ��Z�� as twenty-five. All other letters cover the remaining range in the conventional lexicographic order.</p>
<p>&nbsp;</p>
<p><strong>INPUT</strong></p>
<p>The input consists of several test-cases, separated by an empty line. Each test-case starts with the side length of the square palace <em>n</em> (A&lt;=n&lt;=Z<sup>Z</sup>) and the number of walls <em>w</em> (0&lt;=w&lt;=500) the student placed inside the palace. The palace��s interior spreads thus from 0 to <em>n-1</em>, vertically and horizontally. The following <em>w</em> lines each describe a wall in the form x1 y1 x2 y2, the horizontal and vertical endpoints of the wall such that (0&lt;=x1,y1,x2,y2&lt;=n-1). Input terminates on a test-case with <em>n</em>=A and <em>w</em>=0, which must not be processed. You may safely assume that no student placed walls that transgress the fundaments of the palace and that no palace has more than 10��000 rooms.</p>
<p>&nbsp;</p>
<p><strong>OUTPUT</strong></p>
<p>For each test-case, output the number of rooms in the palace.</p>
<p>&nbsp;</p>
<p><strong>SAMPLE INPUT</strong></p>
<p>P 17</p>
<p>G N G F</p>
<p>F G C G</p>
<p>F O F K</p>
<p>G M N M</p>
<p>C F C M</p>
<p>I E K E</p>
<p>O C O E</p>
<p>B L B N</p>
<p>J M J E</p>
<p>M O J O</p>
<p>H O C O</p>
<p>L H L I</p>
<p>N F K F</p>
<p>M E O E</p>
<p>N D O D</p>
<p>E C E L</p>
<p>G O G L</p>
<p>&nbsp;</p>
<p>ZZZZZZZZZZZZZZZZ 4</p>
<p>A GH ZZZZZZZZZZZZZZZY GH</p>
<p>POLYPROG SELECTION POLYPROG CONTEST</p>
<p>TOBE ORNOT TOBE THATSTHEQUESTION</p>
<p>LEADINGZEROS NO LEADINGAS NO</p>
<p>&nbsp;</p>
<p><strong>SAMPLE OUTPUT</strong></p>
<p>&nbsp;</p>
<p>4</p>
<p>2</p>