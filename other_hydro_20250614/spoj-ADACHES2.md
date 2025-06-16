<p>Ada the Ladybug was playing <a href="https://en.wikipedia.org/wiki/Chess_piece">chess</a> agains her good friend Velvet Mite Vinit. They came up with new figure, called <strong>palace</strong>. In fact, palace is just <strong>tower</strong> with <strong>king</strong> inside. It can attack as king and tower combined: Either anywhere to same column or row <strong>or</strong> anywhere to adjacent (by side or diagonal) field.</p>
<p>Their question is simple: How many ways can <strong>N</strong> palaces be placed on <strong>NxN</strong> chessboard so none of them attacks any other. Since this number might be pretty big, output answer modulo <strong>10<sup>9</sup>+7</strong></p>
<h3>Input</h3>
<p>The first line of input will contain <strong> 1 ¡Ü T ¡Ü     10<sup>5</sup></strong>, the number of test-cases.</p>
<p>Each of the testcases will contain single integer <strong>1 ¡Ü N ¡Ü     10<sup>7</sup></strong>, the size of chessboard.</p>
<h3>Output</h3>
<p>For each test-case output the number of possibilities modulo 1000000007.</p>
<h3>Example Input</h3>
<pre>8
1
2
3
7
10
1000
10000
9999999
</pre>
<h3>Example Output</h3>
<pre>1
0
0
646
479306
711794305
450342414
838796194
</pre>