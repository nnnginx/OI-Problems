<p>As a member of the Association of Coin Minters (ACM), you are fascinated by all kinds of coins and one of your hobbies involves collecting national currency from different countries. Your friend, also an avid coin collector, has her heart set on some of your precious coins and has proposed to play a game that will allow the winner to acquire the loser¡¯s collection (or part thereof).</p>
<p>She begins by preparing two envelopes, each of them enclosing two coins that come from different countries. Then she asks you to choose one of the two envelopes. You can see their contents before making your choice, and also decline the offer and take neither. This process is repeated for a total of <em>r</em> times. As the game progresses, you are also allowed to change your mind about your previous picks if you think you can do better. Eventually, your friend examines the envelopes in your final selection, and from among them she picks a few envelopes herself. If her selection is non-empty and includes an even number of coins from every country (possibly zero), she wins and you must hand over your entire coin collection to her, which would make years of painstaking effort go to waste and force you to start afresh. But if you win, you get to keep the coins from all the envelopes you picked.</p>
<p>Despite the risks involved, the prospect of enlarging your collection is so appealing that you decide to take the challenge. You¡¯d better make sure you win as many coins as possible.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The first line of each test case is the number <em>r</em> of rounds (1 ¡Ü <em>r</em> ¡Ü 300); a line with <em>r</em> = 0 indicates the end of the input. The next <em>r</em> lines contain four non-negative integers 0 ¡Ü <em>a</em>, <em>b</em>, <em>c</em>, <em>d</em> &lt; 10,000, meaning that your friend puts coins from countries labelled <em>a</em> and <em>b</em> inside one of the envelopes, and <em>c</em> and <em>d</em> inside the other one. A blank line separates test cases.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>Print a line per test case containing the largest number of coins you are guaranteed.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<pre class="verbatim">4
0 1 0 5
5 1 0 5
1 2 0 1
1 5 2 0

6
1 4 1 4
2 4 2 4
0 3 0 3
0 4 0 4
4 3 4 3
1 3 1 3

0
</pre>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<pre class="verbatim">6
8
</pre>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: David Garc¨ªa Soriano</em></blockquote>