<!-- P { margin-bottom: 0.08in; direction: ltr; color: rgb(0, 0, 0); }P.western { font-family: "DejaVu Sans"; font-size: 12pt; }P.cjk { font-family: "DejaVu Sans"; font-size: 12pt; }P.ctl { font-family: "DejaVu Sans"; font-size: 12pt; } -->
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in;"><span style="font-size: small;">This is the hardest level of the game. There are n stages in the level. In each stage you will given qi balls. The color of the balls are denoted by an integer between 1 to k. You can pick up <strong>not more than one</strong> ball in each stage. (You can skip if you want) If you pick up a ball you will gain or lose some points depending on the last ball you have picked.  You know color of the available balls of each stage and points you'll get for a certain combination, now can you figure out the maximum point you can get?</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in;"><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in;"><span style="font-size: small;"><strong>Note that you wont gain or lose any point for the first ball you picked.</strong> One stage can contain multiple balls of same color. </span></p>
<p style="margin-bottom: 0in;"><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in;"><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in;"><span style="font-size: small;"><strong>Input Specification:</strong><br>First line of input will contain number of test cases T. </span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in;"><span style="font-size: small;">In each case first line will contain two integer n and k. Than there will be n lines which describes each stage. Each line contains an integer qi which denotes number of balls available in ith level and then q<sub>i</sub> integers will denote the colors. </span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in;"><span style="font-size: small;">Then there will be a k lines, each containing k integer, j<sup>th</sup> integer of i<sup>th</sup> line will indicate the point you will gain or lose if you pick a ball of color j after color i. Negative means you will lose point.</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in;"><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in;"><span style="font-size: small;"><strong>Output Specification:</strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">Print case number and a single integer denoting the maximum point you can get.</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in;"><span style="font-size: small;"><strong>Constraints:</strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in;"><span style="font-size: small;">T&lt;=120</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">2&lt;=n&lt;=100</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">0&gt;=qi&lt;=100</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">1&gt;=k&lt;=100</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">point gain or lose in a step will be at most 1000. </span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in;"><span style="font-size: small;"><strong>Sample Input</strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">2</span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">2 3</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">3 2 3 2</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">4 1 1 3 3</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">1 5 0</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">1 0 2</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">-4 1 -5</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">4 4</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">1 4</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">2 3 1</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">2 2 4</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">3 4 2 2</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">-5 -2 3 2</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">-5 -1 2 0</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">3 4 5 -4</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">-3 -5 0 -4</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in;"><span style="font-size: small;"><strong>Sample output:</strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">Game 1: 2</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">Game 2: 4</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;">&nbsp;</p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;">In first case you can pick color 2 in first stage and color 3 in second stage in gain 2 points.<br></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal;"><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"> </span></p>