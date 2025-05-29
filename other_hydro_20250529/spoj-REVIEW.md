<p>For scientific conferences, scientists submit papers presenting their ideas, and  then review each other¡¯s papers to make sure only good papers are presented at the conference.  Each paper must be reviewed by at least one scientist, and scientists must not review papers written by people they collaborate with (including themselves), or review  the same paper more than once.</p>
<p>You have been asked to write a program to check if your favorite conference is doing things right. Whether a paper is being reviewed too much, too little, or by the wrong people - the organizers must know before it is too late!</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The first line in each test case has two integers, <em>K</em> (1 ¡Ü <em>K</em> ¡Ü 5) and <em>N</em> (1 ¡Ü <em>N</em> ¡Ü 1000). <em>K</em> is the number of reviews that  each paper will receive, while <em>N</em> is the number of papers to be reviewed. The conference only accepts papers with a single author, and authors can only  present a single paper at the conference.</p>
<p>Each of the next <em>N</em> lines describes an author and includes the name of the institution to which  the author belongs, followed by the list of the <em>K</em> papers he or she has been requested to review.  It is assumed that researchers from the same institution collaborate with each other,  whereas researchers from different institutions don¡¯t. All institution names are shorter than 10 characters, and contain only upper  or lowercase letters and no whitespace. Since we have as many papers as authors, papers are identified by their author¡¯s index; paper 1 was written by the first author in the list, and paper <em>N</em> was written by the last author.</p>
<p>The end of the test cases is marked with a line containing <em>K</em>=0 and <em>N</em>=0. You  should generate no output for this line.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>For each test case, your program should output <tt>NO PROBLEMS FOUND</tt> (if all rules are being followed) or <tt><em>P</em></tt><tt> PROBLEMS FOUND</tt>, where <em>P</em> is  the number of rule violations found (counting at most 1 violation per paper).  If there is exactly one rule violation overall, your program should output  <tt>1 PROBLEM FOUND</tt>.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<pre class="verbatim">2 3
UCM 2 3
UAM 1 3
UPM 1 2
2 3
UCM 2 3
UAM 1 2
UPM 2 2
0 0
</pre>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<pre class="verbatim">NO PROBLEMS FOUND
3 PROBLEMS FOUND
</pre>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Manuel Freire</em></blockquote>