<p><strong>[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2015 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at <a href="http://torneoprogramacion.com.ar/wp-content/uploads/2015/09/pruebaTAP2015.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2015/09/pruebaTAP2015.pdf</a> ]</strong></p>
<p>Jaimito didn't waste any time since he was offered his stones in 2013. He no longer spends his time playing with his mother Jimena to games in which his victory is guaranteed, for he explored many stone game variants, as every child should. He even became very good at some of these games, and took part in various championships obtaining excellent results.</p>
<p>For a few months now, he has been particularly interested in a game of stones called <em>TArros con Piedras</em> (TAP). In this game there are <strong>N</strong> jars with stones inside, and two players take turns to play. In his turn, each player should take one stone from one jar, two stones from another jar, and three stones from a third one, and so on until taking <strong>N</strong> stones from some jar, so that the player takes stones from every jar in a single turn. The game continues in this way until one of the players cannot take stones from the jars in a valid way in his turn. Said player loses the match, the other player being the winner.</p>
<p>For example, consider a match with <strong>N = 3</strong> jars with one of them initially having <strong>P<sub>1</sub>&nbsp;= 3</strong> stones, another one having <strong>P<sub>2</sub>&nbsp;= 4</strong> stones and the third one having <strong>P<sub>3</sub>&nbsp;= 10</strong> stones. In this match the player who starts playing has a winning strategy, as he can take one stone from the jar originally having ten stones, two stones from the jar which had three stones, and finally three stones from the jar that initially had four stones. He would then leave the jars with <strong>P<sub>1</sub>&nbsp;= 1</strong>, <strong>P<sub>2</sub>&nbsp;= 1</strong> and <strong>P<sub>3</sub>&nbsp;= 9</strong> stones, so that the second player cannot take stones from the jars in a valid way.</p>
<p>Jaimito is taking part in a TAP championship, and he has reached the finals, where he will face Jacinta. Both of them are expert players, so they make no mistakes when they play. Jaimito has told his mother everything about the match, <em>i.e.</em> the number <strong>N</strong> of jars and how many stones each of them will start with. Jimena knows Jacinta will start playing, and she would like to know if her son will win the championship, but she can't figure it out because she is too nervous to think properly. Can you help her?</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. For each test case, the first line contains an integer <strong>N</strong> representing the number of jars in the match (<strong>1 ¡Ü N ¡Ü 10<sup>5</sup></strong>). The second line contains <strong>N</strong> integers <strong>P<sub>i</sub></strong>&nbsp;representing the number of stones in each jar before starting the match (<strong>1 ¡Ü P<sub>i</sub>&nbsp;¡Ü 10<sup>9</sup></strong> for <strong>i = 1, 2, ..., N</strong>).</p>
<h3>Output</h3>
<p>For each test case, print a line containing a charactner indicating if Jaimito will win the finals or not. The printed character should be an <strong>'<span style="font-family: 'courier new', courier;">S</span>'</strong> if Jaimito is to win, otherwise it should be an <strong>'<span style="font-family: 'courier new', courier;">N</span>'</strong>.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">3
3 4 10
2
10 3</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">N
S</span><span style="white-space: normal;">
</span></pre>