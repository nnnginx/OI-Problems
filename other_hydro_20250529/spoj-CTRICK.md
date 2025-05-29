<p>The magician shuffles a small pack of cards, holds it face down and performs the following procedure:

</p><ol>
  <li>The top card is moved to the bottom of the pack. The new top card is dealt face up onto the table. It is the Ace of Spades.</li>
  <li>Two cards are moved one at a time from the top to the bottom. The next card is dealt face up onto the table. It is the Two of Spades.</li>
  <li>Three cards are moved one at a time¡­</li>
  <li>This goes on until the nth and last card turns out to be the n of Spades.</li>
</ol>

<p>
This impressive trick works if the magician knows how to arrange the cards beforehand (and knows how to give a false shuffle). Your program has to determine the initial order of the cards for a given number of cards, 1 ¡Ü n ¡Ü 20000.
</p>

<h3>Input</h3>
<p>On the first line of the input is a single positive integer, telling the number of test cases to follow. Each case consists of one line containing the integer n.</p>

<h3>Output</h3>
<p>For each test case, output a line with the correct permutation of the values 1 to n, space separated. The first number showing the top card of the pack, etc¡­</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
4
5

<b>Output:</b>
2 1 4 3
3 1 4 5 2</pre>