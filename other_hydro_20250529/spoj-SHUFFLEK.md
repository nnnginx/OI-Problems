<p>      </p>
<table style="width: 100%;" border="0">
<tbody>
<tr style="text-align: center;">
<td width="50%"><a href="/problems/SHUFFLEK/en/">English</a></td>
<td width="50%"><a href="/problems/SHUFFLEK/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p>  </p>
<p>A deck of 2N cards with distinct values of 1,2, …, 2N is given to the shuffling machine. At the beginning, the cards are arranged in the deck in ascending order from the top to the bottom. The shuffling machine executes a sequence of M instructions determined by M integers k1, k2,…, kM for shuffling the cards. The instruction determined by the number ki (1 ≤ |ki| &lt; N), commands the machine to shuffle the cards as follows:</p>
<p><br> • If ki &gt; 0: remove a pile of 2ki cards at the middle of the deck and stacks them on top of the deck.<br> • If ki &lt; 0: remove a pile of -2ki cards at the middle of the deck and inserts them into bottom of the deck.</p>
<p>Mr. X received the deck after it has been shuffled according to M instructions. He wants to throw away some cards from the deck in such a way that the values of the remained cards are in an increasing order from the top to the bottom. Given the M instructions for the shuffling machine, your task is to write a program to help Mr. X determine the minimum number of cards to be removed after the deck has been shuffled.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img src="../../../content/huy391992:shufflek" alt="" width="752" height="274"></p>
<p>Input<br> The first line contains two positive integers N and M (2 ≤ N ≤ 10^9; 0 ≤ M ≤ 10^5) separated by a space. The second line contains M integer k1, k2,…, kM separated by a space.</p>
<p><br> Output<br> The minimum number of cards to be removed after the deck has been shuffled.</p>
<p>Sample Input</p>
<p>3 2</p>
<p>-2 1</p>
<p>Sample Output</p>
<p>2</p>
<p>  </p>