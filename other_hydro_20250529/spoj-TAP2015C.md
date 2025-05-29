<p><span style="font-weight: bold;">[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2015 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at </span><a style="font-weight: bold;" href="http://torneoprogramacion.com.ar/wp-content/uploads/2015/09/pruebaTAP2015.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2015/09/pruebaTAP2015.pdf</a><span style="font-weight: bold;"> ]</span></p>
<p>You may remember from a previous edition of TAP about CompuTenis, that sport specially adapted to a public without any mensurable physical qualities and whose rules involve coding with your elbow glued to your ear. This time we will have another problem concerning this exciting subject, in case you found the solution to that one too easy.</p>
<p>Once more, for the purposes of this problem the only thing you have to know about CompuTenis is that two players, which we will call A and B, compete in a match. The match is won by the player who first wins <strong>S</strong> sets, each set being composed of one or more games. In each set the two players play as many games as is required for one of them to win in at least <strong>J</strong> games, with a difference of at least <strong>D</strong> games won in excess of his opponent. The player satisfying both of these conditions is then the winner of the corresponding set.</p>
<p>The Modern Club Association (MCA) has recently found a trove of records of pre-historic CompuTenis matches. Each record consists of a string composed of <strong>N</strong> characters <strong>'<span style="font-family: 'courier new', courier;">A</span>'</strong> or <strong>'<span style="font-family: 'courier new', courier;">B</span>'</strong>, indicating which player won each of the <strong>N</strong> games the match had, in the order in which they occurred. Now the MCA wants to know, for each record, what the result of the match was.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. For each test case, the first line contains four integers <strong>N, S, J</strong> and <strong>D</strong>. The value <strong>N</strong> represents the number of games in the record to be analyzed (<strong>1 ¡Ü N ¡Ü 10<sup>5</sup></strong>). The value <strong>S</strong> indicates the number of sets a player is required to win in order to win the match (<strong>1 ¡Ü S ¡Ü 10</strong>). The value <strong>J</strong> is the minimum number of games it is necessary to win in order to win a set, whereas the value <strong>D</strong> indicates that a player should win at least that number of games more than his opponent in order to win the set (<strong>1 ¡Ü D ¡Ü J ¡Ü 100</strong>). The second line contains a string composed of <strong>N</strong> characters <strong>'<span style="font-family: 'courier new', courier;">A</span>'</strong> or <strong>'<span style="font-family: 'courier new', courier;">B</span>'</strong>. The <strong>i</strong>-th character of the string indicates which player won the <strong>i</strong>-th game played in the match. The input string will represent a valid record of a complete match.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print a single line containing two integers representing the number of sets won by player A and player B, respectively.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">10 5 2 1
AAAAAAAAAA
21 3 3 2
AABABBBABBBABABABBABB</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">5 0
1 3</span><span style="white-space: normal;">
</span></pre>