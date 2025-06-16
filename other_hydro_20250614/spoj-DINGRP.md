<p>On the way to dinner, the CCC competitors are lining up for their delicious curly fries. The <var>N</var> (1 �� <var>N</var> �� 100) competitors have lined up single-file to enter the cafeteria.</p>

<p>Doctor V, who runs the CCC, realized at the last minute that programmers simply hate standing in line next to programmers who use a different language. Thankfully, only two languages are allowed at the CCC: Gnold and Helpfile. Furthermore, the competitors have decided that they will only enter the cafeteria if they are in a group of at least <var>K</var> (1&nbsp;��&nbsp;<var>K</var>&nbsp;��&nbsp;6) competitors.</p>

<p>Doctor V decided to iterate the following scheme:</p>
<ul>
  <li> He will find a group of <var>K</var> or more competitors who use the same language standing next to each other in line and send them to dinner.</li>
  <li> The remaining competitors will close the gap, potentially putting similar-language competitors together.</li>
</ul>

<p>So Doctor V recorded the sequence of competitors for you. Can all the competitors dine? If so, what is the minimum number of groups of competitors to be sent to dinner?</p>

<h3 align="left">Input</h3>
<p>The first line contains two integers <var>N</var> and <var>K</var>.<br>
  The second line contains <var>N</var> characters that are the sequence of competitors in line (H represents Helpfile, G represents Gnold)</p>

<h3 align="left">Output</h3>
<p>Output, on one line, the single number that is the minimum number of groups that are formed for dinner. If not all programmers can dine, output -1.</p>

<h3 align="left">Sample Input</h3>
<pre>7 2
GHHGHHG</pre>

<h3 align="left">Sample Output</h3>
<pre>3
</pre>

<h3 align="left">Explanation</h3>
<p>There are seven competitors: a Gnold programmer followed by two Helpfile programmers, followed by another Gnold programmer, followed by another two Helpfile programmers followed by a final Gnold programmer. Programmers want to go to dinner in pairs.</p>

<p>First send the first pair of Hs to dinner, leaving GGHHG. Then send the second pair of Hs to dinner, leaving GGG; finally, send in the group of Gs. It might be coincidental that the two pairs of Helpfile programmers entered the cafeteria successively. </p>