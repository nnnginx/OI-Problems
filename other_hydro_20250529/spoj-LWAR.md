<p>A major cosmic battle was getting over. The InterGalactic
SuperPower had been under attack, but it had defended itself quite
well. It was about to launch its final retaliatory assault. But the
number of enemy ships was quite large and they could scatter very
easily. Their only hope, or so their Space Warfare expert said, was to
bomb the enemies (who happened to be lined up in a long line!) using
the strategy described below.</p>

<p>Because the number of ships will be a power of 2, to bomb all the ships (numbered 0 to 2<sup>N</sup> -1), the strategy to be used, which we will call <strong>BombStrat</strong>, goes like this:<br>
  1. Bomb it¡¯s first half, [0 to 2<sup>N-1</sup> -1], in the left to right direction.<br>
  2. Of the remaining half, bomb its latter half part in reverse direction, i.e., bomb ships 2<sup>N</sup>-1, 2<sup>N</sup>-2,...., 2<sup>N-1</sup>+2<sup>N-2</sup> in that order.<br>

  3. Then use <strong>BombStrat</strong> on the remaining ships: [2<sup>N-1</sup> to 2<sup>N-1</sup> + 2<sup>N-2</sup> -1 ]</p>
<p>For example, when N=3, i.e., with ships numbered from 0 to 2<sup>3</sup> -1, this is what happens:<br>

  Step 1: Ships 0,1,2,3 get bombed in that order.<br>
  Step 2: Ships 7, 6 go down next.<br>
  Step 3: Now, the remaining ships [4, 5] are destroyed using the same strategy.</p>
<p>So the bombing is done in the order 0 -&gt; 1 -&gt; 2 -&gt; 3 -&gt;

7 -&gt; 6 -&gt; 4 -&gt; 5. To make the job easier for the InterGalactic
SuperPower¡¯s ships¡¯ pilots, they want to find which ship should be
bombed when. This is your task. Given N, and the description of a ship,
return the 0-based serial number of the bomb will blast it. </p>
<h3>Input</h3>
<p>T ¨C the number of test cases, T&lt;=50.<br>
For each test case:<br>

</p><p>One line containing a binary number, describing the number of the place. The length of this string will equal N (it will be padded with leading zeroes if necessary). N&lt;=30000.</p>
<h3>Output</h3>
<p>For each test case, output the index of a bomb, represented in the same format, as binary digits, whose length is exactly N.</p>
<h3>Example</h3>
<tt>
<p>Sample Input:<br>
  3<br>
  111<br>
  100<br>

  1100</p>
<p>Sample Output:<br>
  100<br>
  110<br>
  1011<br>
</p>
</tt>