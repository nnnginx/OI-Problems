<p>In Boggle, you win points for words you find on the board which no other player finds. If another player finds the same word as you, neither player gets points for that word.<br><br>For words of 4 or fewer letters, 1 point is awarded. 5-letter words are worth 2 points, 6-letter words are worth 3 points, 7-letter words are worth 5 points, and words longer than 7 letters are worth 11 points.<br><br>Given the set of words that some boggle players found, determine the score of the winner.<br><br>Input:<br>The first line is the number of players (at most 100).<br>Each subsequent line is the space-separated list of no more than than 50 words each no more than 50 characters (ASCII 33-126) that player found<br><br>Output:<br>The score of the winning player</p>
<table style="border: none; border-collapse: collapse; width: 624px;" border="0">
<colgroup><col width="*"><col width="*"></colgroup> 
<tbody>
<tr style="height: 0px;">
<td style="border: 1px solid #000000; vertical-align: top; padding: 7px;"><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">Input</span></td>
<td style="border: 1px solid #000000; vertical-align: top; padding: 7px;"><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">Output</span></td>
</tr>
<tr style="height: 0px;">
<td style="border: 1px solid #000000; vertical-align: top; padding: 7px;"><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">2</span><br><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">one two three</span><br><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">two three four</span></td>
<td style="border: 1px solid #000000; vertical-align: top; padding: 7px;"><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">1</span></td>
</tr>
<tr style="height: 0px;">
<td style="border: 1px solid #000000; vertical-align: top; padding: 7px;"><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">3</span><br><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">good dual strange stranger would</span><br><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">dual would duality dregs gnaw</span><br><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">dual gnaw draw would student</span></td>
<td style="border: 1px solid #000000; vertical-align: top; padding: 7px;"><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">17</span></td>
</tr>
<tr style="height: 0px;">
<td style="border: 1px solid #000000; vertical-align: top; padding: 7px;"><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">2</span><br><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">grid grades dread bread thread threads</span><br><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">grid grids grade brood broods thread threads</span></td>
<td style="border: 1px solid #000000; vertical-align: top; padding: 7px;"><span style="font-size: 15px; font-family: Arial; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">9 </span></td>
</tr>
</tbody>
</table>