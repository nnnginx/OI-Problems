<p>How far can you make a stack of cards overhang a table?  If you have
one card, you can create a maximum overhang of half a card length.
(We're assuming that the cards must be perpendicular to the table.) With
two cards you can make the top card overhang the bottom one by half a
card length, and the bottom one overhang the table by a third of a card
length, for a total maximum overhang of 1/2 <tt>+</tt> 1/3 <tt>=</tt>
5/6 card lengths. In general you can make <i>n</i> cards overhang by 1/2

<tt>+</tt> 1/3 <tt>+</tt> 1/4 <tt>+</tt> ... <tt>+</tt> 1/(<i>n</i>
<tt>+</tt> 1) card lengths, where the top card overhangs the second by
1/2, the second overhangs tha third by 1/3, the third overhangs the
fourth by 1/4, etc., and the bottom card overhangs the table by
1/(<i>n</i> <tt>+</tt> 1).  This is illustrated in the figure below.</p>

<center><img src="./22711/file/MPQURQpX.png"></center>

<h3>Input</h3>

<p>The input consists of one or more test cases, followed by a line
containing the number 0.00 that signals the end of the input.  Each test
case is a single line containing a positive floating-point number <i>c</i>
whose value is at least 0.01 and at most 5.20; <i>c</i> will contain
exactly three digits.</p>

<h3>Output</h3>

<p>For each test case, output the minimum number of
cards necessary to achieve an overhang of at least <i>c</i> card
lengths. Use the exact output format shown in the examples.</p>


<pre><b>Input:</b>
1.00
3.71
0.04
5.19
0.00
</pre>

<pre><b>Output:</b>
3 card(s)
61 card(s)
1 card(s)
273 card(s)
</pre>