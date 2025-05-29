<p>Little Chikoo likes to play with numbers. Often he plays the following game:</p>
<ol>
  <li>He chooses a number N and a set of positive integers.</li>
  <li>He writes down all the numbers from 1 to N.</li>
  <li>He chooses the first number (say x) from the set and cancels out all the multiples of x from 1 to N, including x.</li>
  <li>He repeats step 3 for all the numbers from the set.</li>
</ol>
<p>One day Little Chikoo was in a mood to play pranks. So his brother asked him to play the game with a certain challenge. He made the game a little harder and asked him to find out the number of integers which aren't cancelled after he completes step 4. If he does that then Little Chikoo gets to play on his brother's Nintendo for one full day. Now Little Chikoo is in a hurry and wants to finish the job as soon as possible. He has asked for your help.</p>

<h3>Input</h3>
<p>The first line of the input contains N and K. (N &lt;= 10^9, K &lt;= 15)</p>
<p>Then K numbers follow all in a single line. All numbers are &lt;= 100.</p>

<h3>Output</h3>
<p>The output file must contain the number of integers that&nbsp;aren't cancelled&nbsp;after he finishes step 4 of the game.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
10 3
2 4 5

<strong>Output:</strong>
4
</pre>

<p>(The numbers 1, 3, 7 and 9 weren't cancelled).</p>