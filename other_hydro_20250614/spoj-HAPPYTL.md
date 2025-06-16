<p>In the land of Eden, all phone conversations are happy ones. People complaining on the phone are immediately put in jail. To enforce this law, the police taps all phone conversations.</p>
<p>The police wants to hire the appopiate number of operators to listen to all conversations in a given period of time. Unfortunately, each of their operators can listen to one conversation only before needing a really long break to rest from the effort.</p>
<p>As a contractor of the police department, you have been asked to provide a program capable of determining the required number of operators. If the program does not work correctly, you will be put in jail as well, along with all the unhappy complainers. Do you really want to end up there?</p>
<p><strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>Each test case starts with two integers denoting the number of phone calls <em>N</em> (1 �� <em>N</em> &lt; 10&nbsp;000) and the number of intervals <em>M</em> (1 �� <em>M</em> &lt; 100). This is followed by <em>N</em> lines describing the telephone calls, each one consisting of four integers <em>Source</em>, <em>Destination</em>, <em>Start</em> and <em>Duration</em>. <em>Source</em> and <em>Destination</em> identify the pair of telephone numbers establishing the connection (0 �� <em>Source</em>, <em>Destination</em> �� 10&nbsp;000&nbsp;000). <em>Start</em> and <em>Duration</em> are the start time and duration of the call in seconds (1 �� <em>Duration</em> �� 10&nbsp;000 and <em>Start</em> �� 0). You can safely assume that the sum of <em>Start</em> and <em>Duration</em> fits into a 32-bit signed integer.</p>
<p>Afterwards follow <em>M</em> lines containing the time intervals the police are interested in, each described by two integers <em>Start</em> and <em>Duration</em>, in the same format and with the same meaning and constraints as those in the telephone calls. The last test case is represented by <em>N</em> = <em>M</em> = 0 and must not be processed.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>For each of the <em>M</em> intervals of each test case, print the number of calls that are active during at least one second of the interval.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">3 2
3 4 2 5
1 2 0 10
6 5 5 8
0 6
8 2
1 2
8 9 0 10
9 1
10 1
0 0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">3
2
1
0
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Manuel Freire</em><em>&nbsp;</em></blockquote>