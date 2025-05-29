<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>After numerous unfortunate freak fatalities and the     lawsuits, settlements, protests, and boycotts that naturally     followed, the beleaguered executives at ACME Clock     Manufacturers have decided they need to finally fix their     disastrous quality control issues. It has been known for years     that the digital clocks they manufacture have an unacceptably     high ratio of faulty liquid-crystal display (LCD) screens, and     yet these heartless souls have repeatedly failed to address the     issue, or even warn their hapless consumers!</p>
<p>You have been called in as a quality consultant to finally     put a stop to the madness. Your job is to write an automated     program that can test a clock and find faults in its     display.</p>
<p>These clocks use a standard 7-segment LCD display for all     digits (shown in figure below), plus two small     segments for the <strong>:</strong>, and show all times in a 24-hour format.     The minute before midnight is 23:59, and midnight is 0:00. The     <strong>:</strong> segments of a working clock are on at all times. The     representation of each digit using the seven segments is shown     below.</p>
<p><img src="../../../content/john_jones:fn16clk.jpg" alt=""></p>
<p>Your program will be given the display of a clock at several     consecutive minutes, although you do not know exactly what time     these displays start. Some of the LCD segments are burnt out     (permanently off) and some are burnt in (permanently on). Your     program must determine, where possible, which segments are     definitely malfunctioning and which are definitely in working     order.</p>
<h3>Input</h3>
<p>Multiple test cases. Please process until EOF is reached. For each test case:</p>
<p>The first input line contains a single integer      $n$ ($1     \leq n \leq 100$), which is the number of consecutive     minutes of a clock s display. The next      $8n-1$ lines contain      $n$ ASCII images of these clock     displays of size $7 \times     21$. Every representation is followed by a blank line except the last one of each test case.</p>
<p>All digit segments are represented by two characters, and     each colon segment is represented by one character. The     character <tt class="tt">X</tt> indicates a segment that is     on. The character <tt class="tt">.</tt> indicates anything     else (segments that are off or non-segment portions of the     display). See the sample input/output for details; the first     output shows every possible LCD segment along with the smaller     segments used to represent the <strong>:</strong> . No clock representation has     an <tt class="tt">X</tt> in a non-segment position or only     half of a segment showing.</p>
<h3>Output</h3>
<p>For each test case, display a $7 \times 21$     ASCII image with a <tt class="tt">0</tt> for every segment     that is burnt out, a <tt class="tt">1</tt> for every segment     that is burnt in, a <tt class="tt">W</tt> for every segment     that is definitely working, and a <tt class="tt">?</tt> for     every segment for which the status cannot be determined. Use     <tt class="tt">.</tt> for non-segments. If the given displays     cannot come from consecutive minutes, display <tt class="tt">impossible</tt>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
......XX.....XX...XX.
.....X..X...X..X....X
.....X..X.X.X..X....X
.............XX...XX.
.....X..X......X.X..X
.....X..X......X.X..X
......XX.....XX...XX.

......XX.....XX...XX.
.....X..X...X..X....X
.....X..X.X.X..X....X
.............XX...XX.
.....X..X......X.X..X
.....X..X......X.X..X
......XX.....XX...XX.

.............XX...XX.
........X...X..X....X
........X.X.X..X....X
.............XX......
........X...X..X.X..X
........X...X..X.X..X
......XX.....XX...XX.
2
......XX.....XX...XX.
...X....X...X..X.X..X
...X....X.X.X..X.X..X
......XX..........XX.
...X.X....X.X..X.X..X
...X.X......X..X.X..X
......XX.....XX...XX.

......XX.....XX......
...X....X...X..X.....
...X....X.X.X..X.....
......XX.............
...X.X....X.X..X.....
...X.X......X..X.....
......XX.....XX......

<strong>Output:</strong>
.??...WW.....??...??.
?..?.W..?...?..1.0..?
?..?.W..?.?.?..1.0..?
.??...??.....11...WW.
?..?.W..?.0.W..?.1..?
?..?.W..?...W..?.1..?
.??...11.....??...??.
impossible
</pre>