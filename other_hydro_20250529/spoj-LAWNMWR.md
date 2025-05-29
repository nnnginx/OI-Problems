<p>The International Collegiate Soccer&nbsp;Competition (ICSC) is famous for its well-kept rectangular stadiums. The grass playing fields in ICSC stadiums are always 100 meters long, and 75 meters wide. The grass is mowed every week with special lawn mowers, always using the same strategy: first, they make a series of passes along the length of the field, and then they do the same along the width of the field. All passes are straight lines, parallel to the sides of the field.</p>
<blockquote class="figure">
<div class="center">
<hr size="2">
</div>
<div class="center"><img src="../../../content/elhipercubo:lawnmower.jpg" alt="" width="600" height="400"></div>
<div class="center">
<hr size="2">
</div>
</blockquote>
<p>The ICSC has hired a new lawn-mower, Guido. Guido is very chaotic, and instead of covering the field incrementally, he likes to choose random starting positions for each of his passes. But he is afraid of not doing a good job and being fired by the ICSC, so he has asked you to help him. Write a program to make sure that the grass in the field is perfectly cut: all parts of the field have to be mowed at least once when the mower goes from end to end, and again when the mower goes from side to side.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>Each test case contains 3 lines. The first line contains two integers, <em>n</em><sub><em>x</em></sub> (0 &lt; <em>n</em><sub><em>x</em></sub> &lt; 1&nbsp;000) and <em>n</em><sub><em>y</em></sub> (0 &lt; <em>n</em><sub><em>x</em></sub> &lt; 1&nbsp;000), and a real number <em>w</em> (0 &lt; <em>w</em> ¡Ü 50), which represents the width of the cut of that particular lawn mower. The next line describes the end-to-end passes (along the length of the field), and contains <em>n</em><sub><em>x</em></sub> real numbers <em>x</em><sub><em>i</em></sub> (0 ¡Ü <em>x</em><sub><em>i</em></sub> ¡Ü 75) describing the starting positions of the mower¡¯s center in Guido¡¯s end-to-end passes. The last line describes the side-to-side passes, with <em>n</em><sub><em>y</em></sub> real numbers <em>y</em><sub><em>i</em></sub> (0 ¡Ü <em>y</em><sub><em>i</em></sub> ¡Ü 100).</p>
<p>The end of the test cases is signalled with a line that contains the numbers <tt>0 0 0.0</tt>. You should generate no output for this line, as it is not a test case.</p>
<p>Real numbers for <em>w</em>, <em>x</em><sub><em>i</em></sub> and <em>y</em><sub><em>i</em></sub> can have up to 7 digits after the decimal point, and any cut will also include its boundaries. For example, if a 2.0-meter wide cut is performed along the 10.0-meter mark, then a strip of grass from 9.0 to 11.0 (including both) will be considered ¡°cut¡±.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>Print <tt>YES</tt> if Guido has done a good job, or <tt>NO</tt> if some part of the field has not been mowed at least once when the mower was travelling along the length of the field, and again when it was travelling along the width.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">8 11 10.0
0.0 10.0 20.0 30.0 40.0 50.0 60.0 70.0
0.0 10.0 20.0 30.0 40.0 50.0 60.0 70.0 80.0 90.0 100.0
8 10 10.0
0.0 10.0 20.0 30.0 40.0 50.0 60.0 70.0
0.0 10.0 30.0 40.0 50.0 60.0 70.0 80.0 90.0 100.0
4 5 20.0
70.0 10.0 30.0 50.0
30.0 10.0 90.0 50.0 70.0
4 5 20.0
60.0 10.0 30.0 50.0
30.0 10.0 90.0 50.0 70.0
0 0 0.0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">YES
NO
YES
NO
</pre>
</div>
<!--BEGIN NOTES document--> 
<hr class="footnoterule">
<dl class="thefootnotes"><dt class="dt-thefootnotes"> <a name="note1"></a></dt><dd class="dd-thefootnotes">The ICSC is sponsored by the Association for Sports Machinery (ASM), which started out in the US, so they prefer to use the term ¡®soccer¡¯ instead of ¡®football¡¯. </dd></dl> <!--END NOTES--> <!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Manuel Freire</em></blockquote>