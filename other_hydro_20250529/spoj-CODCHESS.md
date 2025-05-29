<p><span style="color: #333333; font-family: 'lucida grande', tahoma, verdana, arial, sans-serif; font-size: 12.800000190734863px; line-height: 13.600000381469727px;">A and B are playing a very interesting variant of the ancient Indian game 'shatranj(also known as chess)' on a 'maidaan'(chessboard) n¡Án in size.</span></p>
<p><span style="color: #333333; font-family: 'lucida grande', tahoma, verdana, arial, sans-serif; font-size: 12.800000190734863px; line-height: 13.600000381469727px;">They take turns to put game pieces called 'ghoda'(knight) so that no two 'ghodas'(knights) could threat each other.</span></p>
<p><span style="color: #333333; font-family: 'lucida grande', tahoma, verdana, arial, sans-serif; font-size: 12.800000190734863px; line-height: 13.600000381469727px;"> A 'ghoda' located in square (a,b) can threat squares (a+1,b+2),(a-1,b+2),(a+1,b-2),</span><span style="color: #333333; font-family: 'lucida grande', tahoma, verdana, arial, sans-serif; font-size: 12.800000190734863px; line-height: 13.600000381469727px;">(a-1,b-2),(a+2,b-1),(a+2,b+1),</span><span style="color: #333333; font-family: 'lucida grande', tahoma, verdana, arial, sans-serif; font-size: 12.800000190734863px; line-height: 13.600000381469727px;">(a-2,b-1),(a-2,b+1).</span></p>
<p><span style="color: #333333; font-family: 'lucida grande', tahoma, verdana, arial, sans-serif; font-size: 12.800000190734863px; line-height: 13.600000381469727px;">The player who can't put a new 'ghoda' during his move loses. Find out which player wins considering that both players play optimally well and A starts.</span></p>
<h3>Input</h3>
<p><span style="color: #333333; font-family: 'lucida grande', tahoma, verdana, arial, sans-serif; font-size: 12.800000190734863px; line-height: 13.600000381469727px;">The first line contains integer T (1¡ÜT¡Ü10^4) ¡ª the number of 'maidaans' (boards), for which you should determine the winning player. Next T lines contain T integers ni (1¡Üni¡Ü10^5) ¡ª the sizes of the 'maidaans'(chessboards).</span></p>
<h3>Output</h3>
<p><span style="color: #333333; font-family: 'lucida grande', tahoma, verdana, arial, sans-serif; font-size: 12.800000190734863px; line-height: 13.600000381469727px;">For each ni¡Áni board print on a single line "0" if A wins considering both players play optimally well. Otherwise, print "1".</span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2</pre>
<pre>2</pre>
<pre>1

<strong>Output:</strong>
1</pre>
<pre>0</pre>