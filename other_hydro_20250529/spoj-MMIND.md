<p>
If you want to buy a&nbsp;new cellular phone, there are many various types to
choose from. To decide which one is the best for you, you have to consider
several important things: its size and weight, battery capacity, WAP support,
colour, price. One of the most important things is also the list of games the
phone provides. Nokia is one of the most successful phone makers because of
its famous Snake and Snake&nbsp;II. ACM wants to make and sell its own phone and
they need to program several games for it. One of them is Master-Mind, the
famous board logical game.

</p><p>
The game is played between two players. One of them chooses a&nbsp;<em>secret code</em>
consisting of <var>P</var>&nbsp;ordered pins, each of them having one of the predefined set of
<var>C</var>&nbsp;colours. The goal of the second player is to guess that secret sequence of
colours. Some colours may not appear in the code, some colours may appear more
than once.

</p><p>
The player makes guesses, which are formed in the same way as the secret
code. After each guess, he/she is provided with an&nbsp;information on how
successful the guess was. This feedback is called a&nbsp;<em>hint</em>. Each hint
consists of <var>B</var> black points and <var>W</var> white points. The black point stands for
every pin that was guessed right, i.e. the right colour was put on the right
position. The white point means right colour but on the wrong position. For
example, if the secret code is "white, yellow, red, blue, white" and the
guess was "white, red, white, white, blue", the hint would consist of one
black point (for the white on the first position) and three white points
(for the other white, red and blue colours). The goal is to guess the
sequence with the minimal number of hints.

</p><p>
The new ACM phone should have the possibility to play both roles. It can make
the secret code and give hints, but it can also make its own guesses. Your
goal is to write a&nbsp;program for the latter case, that means a&nbsp;program that
makes Master-Mind guesses.

</p><p>
</p><h3>Input</h3>

<p>
There is a&nbsp;single positive integer <var>T</var> on the first line of input. It stands
for the number of test cases to follow. Each test case describes one game
situation and you are to make a&nbsp;guess. On the first line of each test case,
there are three integer numbers, <var>P</var>, <var>C</var> and <var>M</var>. <var>P</var> (
1 &lt;= <var>P</var> &lt;= 10) is
the number of pins, <var>C</var> (1 &lt;= <var>C</var> &lt;= 100) is the number of colours, and <var>M</var> 
(1 &lt;= <var>M</var> &lt;= 100) is the number of already played guesses.

</p><p>
Then there are 2 <var>x M</var> lines, two lines for every guess. At the first line of
each guess, there are <var>P</var> integer numbers representing colours of the guess.
Each colour is represented by a&nbsp;number <var>G</var><sub><var>i</var></sub>, 
1 &lt;= <var>G</var><sub><var>i</var></sub> &lt;= <var>C</var>. The second
line contains two integer numbers, <var>B</var> and <var>W</var>, stating for the number of
black and white points given by the corresponding hint.

</p><p>
Let's have a&nbsp;secret code 
<var>S</var><sub>1</sub>, <var>S</var><sub>2</sub>, ... <var>S</var><sub><var>P</var></sub> and the guess

<var>G</var><sub>1</sub>, <var>G</var><sub>2</sub>, ... <var>G</var><sub><var>P</var></sub>. Then we can make a&nbsp;set <var>H</var> containing pairs of numbers
(<var>I</var>,<var>J</var>) such that <var>S</var><sub><var>I</var></sub> = <var>G</var><sub><var>J</var></sub>, and that any number can appear at most once on
the first position and at most once on the second position. That means for
every two different pairs from that set, (<var>I</var><sub>1</sub>,<var>J</var><sub>1</sub>) and (<var>I</var><sub>2</sub>,<var>J</var><sub>2</sub>), we
have 
<var>I</var><sub>1</sub> &lt;&gt; <var>I</var><sub>2</sub> and 
<var>J</var><sub>1</sub> &lt;&gt; <var>J</var><sub>2</sub>. Then we denote <var>B</var>(<var>H</var>) the number of
pairs in the set, that meet the condition <var>I</var> = <var>J</var>, and <var>W</var>(<var>H</var>) the number of
pairs with <var>I</var> &lt;&gt; <var>J</var>.

</p><p>
We define an&nbsp;ordering of every two possible sets <var>H</var><sub>1</sub> and <var>H</var><sub>2</sub>. Let's say

<var>H</var><sub>1</sub> &lt;= <var>H</var><sub>2</sub> if and only if one of the following holds:
</p><div align="left">
<ul>
<li>
<var>B</var>(<var>H</var><sub>1</sub>) &lt; <var>B</var>(<var>H</var><sub>2</sub>), or
</li><li>
<var>B</var>(<var>H</var><sub>1</sub>)  =  <var>B</var>(<var>H</var><sub>2</sub>) and 
<var>W</var>(<var>H</var><sub>1</sub>) &lt;= <var>W</var>(<var>H</var><sub>2</sub>)</li></ul></div><p>Then we can find a&nbsp;maximal set <var>H</var><sub><var>max</var></sub> according to this ordering. The
numbers 
<var>B</var>(<var>H</var><sub><var>max</var></sub>) and 
<var>W</var>(<var>H</var><sub><var>max</var></sub>) are the black and white points for that
hint.

</p><p>
</p><h3>Output</h3>

<p>
For every test case, print the line containing <var>P</var> numbers representing <var>P</var> 
colours of the next guess. Your guess must be valid according to all previous
guesses and hints. The guess is valid if the sequence could be a&nbsp;secret code,
i.e. the sequence was not eliminated by previous guesses and hints.

</p><p>
If there is no valid guess possible, output the sentence
<tt>You are cheating!</tt>. If there are more valid guesses, output the one
that is lexicographically smallest. I.e. find such guess <var>G</var> that for every
other valid guess <var>V</var> there exists such a&nbsp;number <var>I</var> that:
</p><div align="left">
<ul>
<li><var>G</var><sub><var>J</var></sub> = <var>V</var><sub><var>J</var></sub> for every <var>J</var>&lt;<var>I</var>, and
</li><li><var>G</var><sub><var>I</var></sub>&lt;<var>V</var><sub><var>I</var></sub>.
</li></ul></div>
<h3>Example</h3>
<p>Sample Input:</p>

<pre><tt>3
4 3 2
1 2 3 2
1 1
2 1 3 2
1 1
4 6 2
3 3 3 3
3 0
4 4 4 4
2 0
8 9 3
1 2 3 4 5 6 7 8
0 0
2 3 4 5 6 7 8 9
1 0
3 4 5 6 7 8 9 9
2 0
</tt></pre>

<p>Sample Output</p>

<pre><tt>1 1 1 3
You are cheating!
9 9 9 9 9 9 9 9
</tt></pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>