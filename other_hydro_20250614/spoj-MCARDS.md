<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MCARDS/en/">English</a></td>
<td width="50%"><a href="/problems/MCARDS/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>&nbsp;</p>
<p>Dave¡¯s little son Maverick likes to play card games, but being only four years old, he always lose when playing with his older friends. Also, arranging cards in his hand is quite a problem to him.</p>
<p>When Maverick gets his cards, he has to arrange them in groups so that all the cards in a group are of the same color. Next, he has to sort  the cards in each group by their value ¨C card with lowest value should be the leftmost in its group. Of course, he has to hold all the cards  in his hand all the time.</p>
<p>He has to arrange his cards as quickly as possible, i.e. making as  few moves as possible. A move consists of changing a position of  one of his cards.</p>
<p>Write a program that will calculate the lowest number of moves needed  to arrange cards.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line of input file contains two integers C, number of colors (1 ¡Ü C ¡Ü 4), and N, number of cards of the same color (1 ¡Ü N ¡Ü 100),  separated by a space character.</p>
<p>Each of the next C*N lines contains a pair of two integers X  and Y, 1 ¡Ü X ¡Ü C, 1 ¡Ü Y ¡Ü N, separated by a space character.</p>
<p>Numbers in each of those lines determine a color (X) and a value (Y)  of a card dealt to little Maverick. The order of lines corresponds  to the order the cards were dealt to little Maverick. No two lines describe the same card.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>The first and only line of output file should contain the lowest number  of moves needed to arrange the cards as described above.</p>
<p>&nbsp;</p>
<h3>Sample</h3>
<pre>CARDS.IN

2 2
2 1
1 2
1 1
2 2

CARDS.OUT

2
 
CARDS.IN

4 1
2 1
3 1
1 1
4 1

CARDS.OUT

0
 
CARDS.IN

3 2
3 2
2 2
1 1
3 1
2 1
1 2

CARDS.OUT
2
</pre>
<p> </p>