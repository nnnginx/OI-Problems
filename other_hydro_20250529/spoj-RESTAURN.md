<!--HEVEA command line is: /usr/bin/hevea a.tex --> <!--CUT DEF section 1 --><!--TOC section   <FONT COLOR=black> </FONT><DIV CLASS="center"><FONT COLOR=black> <FONT SIZE=6> A<BR> Working at the Restaurant<BR> 1cm </FONT></FONT></DIV><FONT COLOR=black> </FONT>-->
<h2 class="section"><!--SEC ANCHOR --> <span style="font-size: large;"><span style="color: black;"> </span> </span>
<div class="center"><span style="font-size: large;"><br></span></div>
</h2>
<p>Last night, Tom went on a date with a really nice girl. However, he forgot to take his credit card with him and he had no cash in his wallet, so he ended up working at the restaurant to pay for the bill. His task is to take plates from the waiter when he comes from the tables, and pass them along when the diswasher requests them. It is very important for the plates to be washed in the same order as they are brought from the tables, as otherwise it could take too long before a plate is washed, and leftover food might get stuck. Trying to hold all the plates in his hands is probably not a great idea, so Tom puts them on a table as soon as the waiter hands them over to him, and picks them up from the table again when the time comes to pass them along to the dishwasher. There is space for only two piles of plates on the table, which will be referred to as pile 1 and pile 2. There is only one table Tom can use.</p>
<p>Tom won last year��s SWERC, so he is certainly capable of optimizing for efficiency. You have to output a transcript of one possible way in which Tom might decide to organize the plates on the table during the process, given the sequence of plates and requests he receives.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The input has several test cases. Each case begins with a line containing a number <em>N</em> (1 �� <em>N</em> �� 1&nbsp;000), followed by <em>N</em> lines, which contain either <tt>DROP m</tt> or <tt>TAKE m</tt>, where <em>m</em> &gt; 0 is the number of plates to take or drop. <tt>DROP m</tt> represents that the next event is the waiter bringing <em>m</em> plates to Tom, one by one, so he has to drop them on the table;  <tt>TAKE m</tt> represents that the next event is Tom taking <em>m</em> plates from the table, one by one, and passing them along in the right order. You can assume that he never receives a <tt>TAKE m</tt> instruction when there are fewer than <em>m</em> plates on the table, and that the sum <em>M</em> of all values of <em>m</em> corresponding to <tt>DROP</tt> operations does not exceed 100&nbsp;000. Note that there might be plates left on Tom��s table when the last request is issued, as Tom might be relieved of his duty to stay until the restaurant closes.</p>
<p>The input ends with a line with <em>N</em> = 0, which must not be processed.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>For every test case, the output will be a series of lines describing the operations to be performed with the plates. The content of each line will be one of the following:</p>
<ul class="itemize">
<li class="li-itemize"><tt>DROP 1 m</tt> (<tt>DROP 2 m</tt>), <em>m</em>&gt;0, if Tom needs to take a plate from the waiter, drop it on top of pile 1 (pile 2), and repeat this operation <em>m</em> times in total.</li>
<li class="li-itemize"><tt>TAKE 1 m</tt> (<tt>TAKE 2 m</tt>), <em>m</em>&gt;0, if Tom needs to take a plate from the top of pile 1 (pile 2), pass it along to the dishwasher, and repeat <em>m</em> times in total.</li>
<li class="li-itemize"><tt>MOVE 1-&gt;2 m</tt> (<tt>MOVE 2-&gt;1 m</tt>), <em>m</em>&gt;0, if Tom needs to take a plate from the top of pile 1 (pile 2), drop it on top of pile 2 (pile 1), and repeat <em>m</em> times in total.</li>
</ul>
<p>You must output at most 6<em>N</em> lines, and the total number of movements of plates in your transcript (that is, the sum of the <tt>m</tt>��s printed in your output, for all three kinds of operations), must be at most 6<em>M</em>, as otherwise Tom won��t be able to cope with all the work.</p>
<p>Note that Tom must obey the commands in the same order as they are issued. This means that, if he receives a TAKE <tt>m</tt> command, he must perform a certain number of MOVE and TAKE operations such that the sum of the numbers of plates <strong>taken</strong> adds up exactly to <tt>m</tt> before performing the operations corresponding to the next command; and if he receives a <tt>DROP m</tt> command, he must perform a number of DROP or MOVE operations for which the sum of the numbers of plates <strong>dropped</strong> adds up exactly to <tt>m</tt> before performing the operations corresponding to the next command.</p>
<p>Of course, it is also forbidden to take plates from the waiter or pass them along to the dishwasher in the absence of the corresponding order.</p>
<p>There <strong>must</strong> be an empty line between the outputs of different cases.</p>
<p>Any solution satisfying these conditions will be accepted.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">3
DROP 100
TAKE 50
TAKE 20
3
DROP 3
DROP 5
TAKE 8
0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">DROP 2 100
MOVE 2-&gt;1 100
TAKE 1 50
TAKE 1 20

DROP 2 3
DROP 2 5
MOVE 2-&gt;1 8
TAKE 1 8
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Abel Molina Prieto</em><em>&nbsp;</em></blockquote>