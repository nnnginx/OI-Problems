<p>Bullshit Bingo is a game to make lectures, seminars or meetings less
boring.
Every player has a card with 5 rows and 5 columns. Each of the 25 cells
contains
a word (the cell in the middle has always the word "BINGO"
written in it).
Whenever a player hears a word which is written on his card, he can
mark it. The cell in the middle is already marked when the game starts. If a player
has marked all the words in a row, a column or a diagonal,
he stands up and shouts "BULLSHIT". After this, the game starts over
again.</p>
<p>Sitting in a lecture, you observe that some students in the audience
are
playing Bullshit Bingo.
You wonder what the average number of different words is until
"BULLSHIT" is exclaimed. For the purpose of this problem, a word
consists of letters of the English alphabet ('a' to 'z' or 'A' to 'Z').
Words are separated by characters other than letters (for example
spaces,
digits or punctuation).
Do the comparison of words case-insensitively, i.e. "Bingo" is the
same word
as "bingo". When counting the number of different words, ignore the word
BULLSHIT (indicating the end of the game), and consider only
the words of the current game, i.e., if a word has already occurred in a previous
game, you may still count it in the current game.
If the last game is unfinished, ignore the words of that game.
</p>
<h3>Input Specification</h3>
<p>The input file consists of the text of the lecture, with "BULLSHIT"
occurring occasionally. The first game starts with the first word in the input.
Each occurrence of "BULLSHIT" indicates the end of one game.<br>
You may assume, that
</p><ul>
<li>the word "BULLSHIT" occurs only in uppercase letters</li>
<li>every word has at most 25 characters, and each line has at most 100
characters</li>
<li>there are at most 500 different words before a game ends</li>
<li>the players follow the rules, so there is no need to check if a game is valid or not</li>
<li>at least one game is completed</li>
</ul>
<p></p>
<h3>Output Specification</h3>
<p>The output consists of one number: the average number of different
words needed to win a game.
Write the number as a reduced fraction in the format shown below. Reduced fraction means that
there should be no integer greater than 1 which
divides both the numerator and denominator.
For example if there were 10 games,
and the number of different words in each game summed up to 55,
print "11 / 2".
</p>
<h3>Sample Input</h3>
<pre>Programming languages can be classified BULLSHIT into following types:
- imperative and BULLSHIT procedural languages
- functional languages
- logical BULLSHIT programming languages
- object-oriented BULLSHIT languages
</pre>
<h3>Sample Output</h3>
<pre>9 / 2
</pre>
<hr>
<i>In the sample input, there are 4 completed games.
The number of different words is 5, 5, 4 and 4, respectively.</i>