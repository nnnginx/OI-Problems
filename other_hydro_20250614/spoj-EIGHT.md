<p>What is an Eight Directions Crossword? It's a filled crossword in which all the words are hidden in eight directions (up, down, left and right and also up-left, down-right etc.) You have to find these hidden words in each crossword.</p>
<p>Đuro has made an N x N eight-directions-crossword. His crossword is a bit strange: you are given only one word and you have to find it in a crossword. To make things more difficult, you can skip some letters in the crossword while looking for the given word. More precisely, the given word is the subsequence of not necesarily consecutive letters in a row, column or a diagonal of the crossword in one of the eight directions.</p>
<p>Now you discover that, under these conditions, you can read the given word in the crossword in multiple ways. How many?</p>
<h3>Input</h3>
<p>In the first line of the input there is an integer N (2 ≤ N ≤ 1000), the crossword dimension, followed by space and the given word you are to find. This word has 2-10 letters.</p>
<p>N lines follow, representing the crossword. All letters in the crossword and in the given word are small letters of the English alphabet.</p>
<h3>Output</h3>
<p>Print the required number of ways. (This number will fit into int64 in Pascal or long long in C/C++.)</p>
<h3>Example</h3>
<table border="0">
<tbody>
<tr>
<td style="text-align: left; width: 100px;" valign="top"><span style="font-size: 12px; font-weight: bold;">input</span><br style="font-family: Arial; font-size: 12px;">
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">2 aa
aa
aa</pre>
<p>&nbsp;</p>
<p><span style="font-size: 12px; font-weight: bold;">output</span><br style="font-family: Arial; font-size: 12px;"></p>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px; text-align: left;">12</pre>
</td>
<td style="text-align: left; width: 100px;" valign="top"><span style="font-size: 12px; font-weight: bold;">input</span><br style="font-family: Arial; font-size: 12px;">
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">3 aa
aaa
aaa
aaa</pre>
<p>&nbsp;</p>
<p><span style="font-size: 12px; font-weight: bold;">output</span><br style="font-family: Arial; font-size: 12px;"></p>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">56</pre>
</td>
<td style="text-align: left; width: 100px;" valign="top"><span style="font-size: 12px; font-weight: bold;">input</span><br style="font-family: Arial; font-size: 12px;">
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">8 silba
siolobba
oooaoooo
oooboooo
aooooooo
oboloooo
oolooooo
oooioooo
ooossooo</pre>
<p>&nbsp;</p>
<p><span style="font-size: 12px; font-weight: bold;">output</span><br style="font-family: Arial; font-size: 12px;"></p>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">4</pre>
</td>
</tr>
</tbody>
</table>