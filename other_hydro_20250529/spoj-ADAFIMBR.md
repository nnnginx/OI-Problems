<p>Ada the Ladybug is playing a games against her good friend Velvet Mite Vinit. They are playing a game which they call Fimber: There will be a few piles of seeds. In each move, the one who is in move can choose a pile and take <strong>K</strong> seeds from it, where <strong>K</strong> is equal to some Fibonacci number. They alternate in their turns. The one who can't move will lose.</p>
<p>Fibonacci number will be defined as <strong>F<sub>0</sub>=1, F<sub>1</sub>=1,     F<sub>N</sub>=F<sub>N-1</sub>+F<sub>N-2</sub></strong></p>
<p>As ladies go first Ada starts. Can you determine who will if both will play optimaly?</p>
<h3>Input</h3>
<p>The first line of each test-case will contain an integer <strong>1 ¡Ü N ¡Ü     10<sup>5</sup></strong>, the number of piles.</p>
<p>The next line will contain <strong>N</strong> integers <strong>0 ¡Ü A<sub>i</sub> ¡Ü     3*10<sup>6</sup></strong>, the number of seeds in each pile.</p>
<h3>Output</h3>
<p>For each test-case, print the name of winner (so either "<strong>Ada</strong>" or "<strong>Vinit</strong>").</p>
<h3>Example Input</h3>
<pre>6
3 3 1 8 3 4
</pre>
<h3>Example Output</h3>
<pre>Ada
</pre>
<h3>Example Input</h3>
<pre>1
10
</pre>
<h3>Example Output</h3>
<pre>Vinit
</pre>
<h3>Example Input</h3>
<pre>4
3 9 5 2
</pre>
<h3>Example Output</h3>
<pre>Ada
</pre>
<h3>Example Input</h3>
<pre>5
10 10 6 8 10
</pre>
<h3>Example Output</h3>
<pre>Ada
</pre>
<h3>Example Input</h3>
<pre>1
4
</pre>
<h3>Example Output</h3>
<pre>Vinit
</pre>
<h3>Example Input</h3>
<pre>4
6 1 7 3
</pre>
<h3>Example Output</h3>
<pre>Ada
</pre>
<h3>Example Input</h3>
<pre>5
7 10 9 3 10
</pre>
<h3>Example Output</h3>
<pre>Ada
</pre>
<h3>Example Input</h3>
<pre>6
4 6 10 9 3 8
</pre>
<h3>Example Output</h3>
<pre>Vinit
</pre>