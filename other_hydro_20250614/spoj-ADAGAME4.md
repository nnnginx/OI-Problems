<p>Ada the Ladybug is playing <strong>Game of Divisors</strong> against her friend Velvet Mite Vinit. The game has following rules. There is a pile of <strong>N</strong> stones between them. The player who's on move can pick at least <strong>1</strong> an at most <strong>¦Ò(N)</strong> stones (where <strong>¦Ò(N)</strong> stands for number of divisors of <strong>N</strong>). Obviously, <strong>N</strong> changes after each move. The one who won't get any stones (<strong>N == 0</strong>) loses.</p>
<p>As Ada the <strong>Lady</strong>bug is a lady, so she moves first. Can you decide who will be the winner? Assume that both players play optimally.</p>
<h3>Input</h3>
<p>The first line of input will contain <strong>1 ¡Ü T ¡Ü 10<sup>5</sup></strong>, the number of test-cases.</p>
<p>&nbsp;</p>
<p>The next <strong>T</strong> lines will contain <strong>1 ¡Ü N ¡Ü 2*10<sup>7</sup></strong>, the number of stones which are initially in pile.</p>
<h3>Output</h3>
<p>Output the name of winner, so either "Ada" or "Vinit".</p>
<h3>Example Input</h3>
<pre>8
1
3
5
6
11
1000001
1000000
29
</pre>
<h3>Example Output</h3>
<pre>Ada
Vinit
Ada
Ada
Vinit
Vinit
Ada
Ada
</pre>