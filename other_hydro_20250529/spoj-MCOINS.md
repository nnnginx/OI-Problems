<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MCOINS/en/">English</a></td>
<td width="50%"><a href="/problems/MCOINS/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Asen and Boyan are playing the following game. They choose two different positive integers K and L, and start the game with a tower of N coins. Asen always plays first, Boyan ¨C second, after that ¨C Asen again, then Boyan, and so on. The boy in turn can take 1, K or L coins from the tower. The winner is the boy, who  takes  the  last  coin  (or  coins). After  a  long,  long playing, Asen  realizes  that  there  are cases in which he could win, no matter how Boyan plays. And in all other cases Boyan being careful can win, no matter how Asen plays.</p>
<p>
So, before the start of the game Asen is eager to know what game case  they have. Write a program coins which help Asen  to predict  the game  result  for given K, L and N.
</p>

<h3>INPUT</h3>
<p>The input describes m games.</p>
<p>The first line of the standard input contains the integers K, L and m, 1 &lt; K &lt; L &lt; 10, 3 &lt; m &lt; 50. The second  line contains m integers N1, N2, ¡­, Nm, 1 ¡Ü Ni ¡Ü 1 000 000,  i = 1, 2, ¡­., m, representing  the number of coins in each of the m towers</p>

<pre>SAMPLE INPUT<br>2 3 5 <br>3 12 113 25714 88888</pre>

<h3>OUTPUT</h3>
<p>The  standard output contains a  string of  length m composed of letters A and B.  If Asen wins  the  ith game (no matter how the opponent plays), the ith letter of the string has to be A. When Boyan wins the ith game (no matter how Asen plays), the ith letter of the string has to be B.</p>

<pre>SAMPLE OUTPUT<br>ABAAB<br></pre>
<p><strong>Problem for kid - Please, think like kid.</strong>  </p>