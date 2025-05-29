<p>You are playing the funny game “Guess the number” with a friend. In this game, one of the players choose a positive integer and the other has to guess it by using the clues that are revealed. The i-th clue is either “Y” or “N” indicating whether the hidden number is a multiple of i or not, respectively. For instance, if the clues so far are “YYNYY” it means that the number is a multiple of 1, 2, 4 and 5, but it is not a multiple of 3. Given the clues of the game so far, you have to guess the minimum possible number according to them, or call your friend a cheater if there is no number such that the clues were correctly given.</p>

<h3>Input</h3>
<p>The input contains several test cases. Each test case is described in a single line that contains a non-empty string of at most 20 characters. The string is formed entirely of uppercase letters “<tt>Y</tt>” and “<tt>N</tt>”, and represents the clues given so far, in order from left to right. The last line of the input contains a single asterisk and should not be processed as a test case.</p>

<h3>Output</h3>
<p>For each test case output a single line with the minimum positive integer that satisfies all the clues, or <tt>−1</tt> if there is no such a number.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
YYNYY
YYYNNN
*

<strong>Output:</strong>
20
-1</pre>