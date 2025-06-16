<pre><span style="white-space: normal;"><h2><span style="font-weight: normal;">given the elements of the table ... draw the table :D</span></h2><h2 style="font-family: 'Times New Roman';"><span style="color: #ff0000; font-size: medium;">INPUT&nbsp;</span></h2>
<p style="font-family: 'Times New Roman'; font-size: medium;">The input consists of one or more table descriptions, followed by a line whose first character is '*', which signals the end of the file. Each description begins with a header line containing one or more characters that define the number and alignment of columns in the table. Each character in the header line is either '&lt;', '=', or '&gt;', and indicates a left-justified, centered, or right-justified column. Following the header are at least two and at most 21 data lines that contain the entries for each row. Each data line consists of one or more nonempty entries separated by an ampersand ('&amp;'), where the number of entries is equal to the number of columns defined in the header line. The first data line contains entries for the column titles, and the remaining data lines contain entries for the body of the table. Spaces may appear within an entry, but never at the beginning or end of an entry. The characters '&lt;', '=', '&gt;', '&amp;', and '*' will not appear in the input except where indicated above.</p>
<h2 style="font-family: 'Times New Roman';"><span style="color: #ff0000; font-size: medium;">OUTPUT&nbsp;</span></h2>
<p style="font-family: 'Times New Roman'; font-size: medium;">For each table description, output the table using the exact format shown in the examples. Note that</p>
<ul style="font-family: 'Times New Roman'; font-size: medium;">
<li>The total width of the table will never exceed 79 characters (not counting end-of-line).</li>
<li>Dashes ('<tt>-</tt>') are used to draw horizontal lines, not underscores ('<tt>_</tt>'). 'At' signs ('<tt>@</tt>') appear at each of the four outer corners. Plus signs ('<tt>+</tt>') appear at intersections&nbsp;<em>within</em>&nbsp;the line separating the title from the body.</li>
<li>The largest entry in a column is always separated from the enclosing bars ('<tt>|</tt>') by exactly one space.</li>
<li>If a centered entry cannot be&nbsp;<em>exactly</em>&nbsp;centered within a column, the extra space goes on the right of the entry.</li>
</ul>
<p style="font-family: 'Times New Roman'; font-size: medium;">Input and correct output files satisfy all the requirements listed in&nbsp;<em>Notes to Teams</em>,&nbsp;<strong>except</strong>&nbsp;that the output may contain two or more consecutive spaces. There are no spaces at the beginning or end of lines, and only spaces are used (never tabs).</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>
<h2 style="font-family: 'Times New Roman';"><span style="color: #ff0000; font-size: medium;">SAMPLE INPUT:&nbsp;</span></h2>
<pre>&lt;&gt;=&gt;
TITLE&amp;VERSION&amp;OPERATING SYSTEM&amp;PRICE
Slug Farm&amp;2.0&amp;FreeBSD&amp;49.99
Figs of Doom&amp;1.7&amp;Linux&amp;9.98
Smiley Goes to Happy Town&amp;11.0&amp;Windows&amp;129.25
Wheelbarrow Motocross&amp;1.0&amp;BeOS&amp;34.97
&gt;
What is the answer?
42
&lt;&gt;
Tweedledum&amp;Tweedledee
"Knock, knock."&amp;"Who's there?"
"Boo."&amp;"Boo who?"
"Don't cry, it's only me."&amp;(groan)
*</pre>
<h2 style="font-family: 'Times New Roman';"><span style="color: #ff0000; font-size: medium;">SAMPLE OUTPUT:&nbsp;</span></h2>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>
<pre>@-----------------------------------------------------------------@
| TITLE                     | VERSION | OPERATING SYSTEM |  PRICE |
|---------------------------+---------+------------------+--------|
| Slug Farm                 |     2.0 |     FreeBSD      |  49.99 |
| Figs of Doom              |     1.7 |      Linux       |   9.98 |
| Smiley Goes to Happy Town |    11.0 |     Windows      | 129.25 |
| Wheelbarrow Motocross     |     1.0 |       BeOS       |  34.97 |
@-----------------------------------------------------------------@
@---------------------@
| What is the answer? |
|---------------------|
|                  42 |
@---------------------@
@---------------------------------------------@
| Tweedledum                 |     Tweedledee |
|----------------------------+----------------|
| "Knock, knock."            | "Who's there?" |
| "Boo."                     |     "Boo who?" |
| "Don't cry, it's only me." |        (groan) |
@---------------------------------------------@</pre>
</span></pre>