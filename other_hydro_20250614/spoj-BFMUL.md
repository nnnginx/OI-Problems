<p>Farmer Joe is a strange fellow indeed. He owns a rare breed of cow that eats chocolate and produces chocolate milk, and each cow has exactly <strong>L</strong> legs. Lately, Joe has been suffering from sore feet, and his intuition tells him that it must be from the chocolate milk. The cows, he suspects, are in pain from stepping on sharp pebbles while crossing the road with chickens in their bare hooves. Naturally, they are transferring their pain karmically through the milk. So he has taken it upon himself to make proper hoofwear for all of them. As he lives at the top of an ivory tower, he finds it most convenient to count their heads. (Each cow has exactly one head.) Joe would like to know how many shoes he must make given that he has counted <strong>H</strong> heads, and in fact he wrote a program for just this purpose but can¡¯t seem to find it. The program is written for a special computer that he constructed while he was writing his dissertation on Turing machines. He has asked for your help in replacing his program. Please help him quickly, so his cows can suffer as little as possible.</p>
<p><strong>Note:</strong> You can use any programming language you want, as long as it is brainf**k.</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>T</strong> (1 ¡Ü <strong>T</strong> ¡Ü 1000). Then follow <strong>T</strong> lines, each containing integers <strong>L</strong> and <strong>H</strong> (0 ¡Ü <strong>L</strong>,<strong>H</strong> ¡Ü 10^20) separated by a single space. Each line, including the last, is terminated by a single newline (linefeed) character, which has ASCII value 10.</p>
<h3>Output</h3>
<p><strong>T</strong> lines containing the number of shoes Farmer Joe must make.</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>5
0 0
0 42
42 0
42 42
12345 67890
</pre>
<p><strong>Output:</strong></p>
<pre>0
0
0
1764
838102050
</pre>
<h3>Additional Info</h3>
<p>There are two randomly generated data sets, one with <strong>T</strong>=1000 and the other with <strong>T</strong>=500. <strong>L</strong> and <strong>H</strong> are generated independently, and the average number of digits in either is about 11.</p>
<p>My solution at the time of publication has 410 bytes (not golfed) and runs in 0.27s with 1.8M memory footprint.</p>