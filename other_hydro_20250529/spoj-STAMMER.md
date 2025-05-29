<p>Dr.&nbsp;Ellie Arroway has established contact with an extraterrestrial civilization. However, all efforts to decode their messages have failed so far because, as luck would have it, they have stumbled upon a race of stuttering aliens! Her team has found out that, in every long enough message, the most important words appear repeated a certain number of times as a sequence of consecutive characters, even in the middle of other words. Furthermore, sometimes they use contractions in an obscure manner. For example, if they need to say <em>bab</em> twice, they might just send the message <em>babab</em>, which has been abbreviated because the second <em>b</em> of the first word can be reused as the first <em>b</em> of the second one.</p>
<p>Thus, the message contains possibly overlapping repetitions of the same words over and over again. As a result, Ellie turns to you, S.R.&nbsp;Hadden, for help in identifying the gist of the message.</p>
<p>Given an integer <em>m</em>, and a string <em>s</em>, representing the message, your task is to find the longest substring of <em>s</em> that appears at least <em>m</em> times. For example, in the message <em>baaaababababbababbab</em>, the length-5 word <em>babab</em> is contained 3 times, namely at positions 5, 7 and 12 (where indices start at zero). No substring appearing 3 or more times is longer (see the first example from the sample input). On the other hand, no substring appears 11 times or more (see example 2).</p>
<p>In case there are several solutions, the substring with the rightmost occurrence is preferred (see example 3).</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The input contains several test cases. Each test case consists of a line with an integer <em>m</em> (<em>m</em> ¡Ý 1), the minimum number of repetitions, followed by a line containing a string <em>s</em> of length between <em>m</em> and 40&nbsp;000, inclusive. All characters in <em>s</em> are lowercase characters from ¡°a¡± to ¡°z¡±. The last test case is denoted by <em>m</em> = 0 and must not be processed.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>Print one line of output for each test case. If there is no solution, output <tt>none</tt>; otherwise, print two integers in a line, separated by a space. The first integer denotes the maximum length of a substring appearing at least <em>m</em> times; the second integer gives the rightmost possible starting position of such a substring.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">3
baaaababababbababbab
11
baaaababababbababbab
3
cccccc
0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">5 12
none
4 2
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: David Garc¨ªa Soriano</em></blockquote>