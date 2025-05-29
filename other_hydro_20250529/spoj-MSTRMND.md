<p></p>
<table class="problems" style="width: 99%;" border="0">
<tbody>
<tr class="navigation">
<td><a href="/problems/MSTRMND/english/">English version</a></td>
<td><a href="/problems/MSTRMND/polski/">Wersja polska</a></td>
</tr>
</tbody>
</table>
<p><span style="line-height: normal"> 
</span></p><p>Task (<a href="http://en.wikipedia.org/wiki/Mastermind_(board_game)">the rules of the game</a>) requires to guess the code which consists of four elements. Each element of the code can have one of six different values. The same values can appear multiple times. The code should be guessed in a maximum amount of ten tries. After guessing the code (or after using up the limit of ten tries) your program should end.</p>
<p><strong>Input/output</strong></p>
<p>During each try you give your suggestion of a correct code ¨C you output four numbers from a range of one to six on the standard output. In the response you get a hint about which elements were typed correctly and which were not ¨C you read four numbers and each of them can have one of those values: 1 (the number is correct), 0 (element is not in the right place) or -1 (the element is incorrect).</p>
<p><strong>Example</strong></p>
<pre>You:    1  1  1  2
Judge:  1  1 -1  1

You:	3  4  5  6
Judge: -1 -1 -1  0

You:	1  1  6  2
Judge:	1  1  1  1
</pre>
<p><strong>Remark: </strong>Program should clear the output buffer after printing each line. It can be done using fflush(stdout) command or you can set the proper type of buffering at the beginning of the execution - setlinebuf(stdout).</p>
 <p></p>