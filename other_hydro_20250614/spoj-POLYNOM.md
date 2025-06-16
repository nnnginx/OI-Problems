<p>The number of spectators at the FIFA World Cup increases year after year. As you sell the advertisement slots during the games for the coming years, you need to come up with the price a company has to pay in order to get an advertisement slot. For this, you need a good estimate for the number of spectators in the coming games, based on the number of spectators in the past games.</p>
<p>Your intuition tells you that maybe the number of spectators could be modeled precisely by a polynomial of degree at most <em>3</em>. The task is to check if this intuition is true.</p>
<h3>Input</h3>
<p>The input starts with a positive integer <em>N</em>, the number of test   cases. Each test case consists of one line. The line starts with an   integer <em>1 ¡Ü n ¡Ü 500</em>, followed by <em>n</em> integers <em>x<sub>1</sub>, ...,   x<sub>n</sub></em> with <em>0 ¡Ü x<sub>i</sub> ¡Ü 50000000</em> for all <em>i</em>, the number of   spectators in past games.</p>
<h3>Output</h3>
<p>For each test case, print <strong>YES</strong> if there is a polynomial <em>p</em> (with real coefficients) of degree at most <em>3</em> such that <em>p(i) = x<sub>i</sub></em> for all <em>i</em>. Otherwise, print <strong>NO</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
1 3
5 0 1 2 3 4
5 0 1 2 4 5

<strong>Output:</strong>
YES
YES
NO
</pre>