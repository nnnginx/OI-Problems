<h3>  Tichu</h3>
<!--l. 3-->
<p>Tichu is a card game played by four players. The players sit around a square table, and each player forms a team with the person sitting opposite him or her. The game is played with a standard deck of cards and four additional special cards. The basic rule of the game is as follows: the player who won the last trick can start a new trick with any legal combination of cards. Then, in turn, each next player can either pass or play the same combination of cards, but with a higher value. This continues until everyone passes, and at that point the player who played the last combination wins the trick and can start a new trick. The main goal is to get rid of all of your cards as soon as possible. <!--l. 15--></p>
<p>These basic rules make it a good tactic to combine the cards in such a way that they can be played in as few combinations as possible. For simplicity we consider here a slightly modified version of the game. We ignore the special cards, so that leaves a standard deck of 52 cards, ranging over the values <tt>2 </tt>to <tt>Ace </tt>and over the suits <tt>hearts</tt>, <tt>diamonds</tt>, <tt>clubs</tt>, and <tt>spades</tt>. The suits are indicated by the lowercase letters <tt>h</tt>, <tt>d</tt>, <tt>c</tt>, and <tt>s</tt>, while the values are indicated in increasing order by <tt>2</tt>�C<tt>9</tt>, <tt>T</tt>, <tt>J</tt>, <tt>Q</tt>, <tt>K</tt>, <tt>A</tt>. <!--l. 26--></p>
<p>The following list is a complete set of legal combinations:<a id="fn1x0-bk" href="#fn1x0"><sup>1</sup></a></p>
<ul>
<li>any single card; </li>
<li>a pair of cards of the same value; </li>
<li>three cards of the same value; </li>
<li>four cards of the same value; </li>
<li>a full house, that is, three cards of the same value and two cards of another, same       value, for example <tt>444KK</tt>; </li>
<li>a straight of length at least five, that is, at least five cards of consecutive increasing       values, for example <tt>89TJQK</tt>.</li>
</ul>
<!--l. 40-->
<p>In this problem, your task is to determine the minimum number of combinations that your hand of 13 cards can be partitioned into. <!--l. 43--></p>
<p>&nbsp;</p>
<h4>Input</h4>
<!--l. 44-->
<p>On the first line a positive integer: the number of test cases, at most 100. After that per test case:</p>
<ul>
<li>one line that describes your hand of 13 cards. A card is described by two characters:       the value followed by the suit. All cards in your hand are different.</li>
</ul>
<!--l. 53-->
<p>&nbsp;</p>
<h4>Output</h4>
<!--l. 54-->
<p>Per test case:</p>
<ul>
<li>one line containing an integer <em>n</em>: the minimum number of combinations that your       hand can be partitioned into. </li>
<li><em>n </em>lines that describe a minimal set of combinations of cards from your hand. Each line       should contain the cards in one legal combination, in the same format as in the input.       All cards from your hand must occur exactly once in one of the combinations. No       specific ordering of the combinations or the cards within a combination is required.</li>
</ul>
<!--l. 66-->
<p>&nbsp;</p>
<h4>Sample in- and output</h4>
<table align="center" id="TBL-1" border="1" cellspacing="5" cellpadding="5" rules="groups">
<colgroup><col id="TBL-1-1"></colgroup><colgroup id="TBL-1-2g"><col id="TBL-1-2"></colgroup>
<tbody>
<tr id="TBL-1-1-" style="vertical-align:baseline;">
<td id="TBL-1-1-1" style="white-space:wrap; text-align:left;"><!--l. 43-->
<p><span>Input</span></p>
</td>
<td id="TBL-1-1-2" style="white-space:wrap; text-align:left;"><!--l. 43-->
<p><span>Output</span></p>
</td>
</tr>
<tr id="TBL-1-2-" style="vertical-align:baseline;">
<td id="TBL-1-2-1" style="white-space:wrap; text-align:left;"><!--l. 46-->
<pre>2
2h 3c 4d 5d 6s Th Qc Qs Ad Tc Ts 9c 9d
2h 3h 4h 5h 6d 7s 8h 8d 8c 8s 9c Td Js</pre>
</td>
<td id="TBL-1-2-2" style="white-space:wrap; text-align:left;"><!--l. 50-->
<pre>4
2h 3c 4d 5d 6s
Th Ts Tc Qc Qs
9d 9c
Ad
2
2h 3h 4h 5h 6d 7s 8d 9c Td Js
8h 8s 8c </pre>
</td>
</tr>
</tbody>
</table>
<hr>
<p><a id="fn1x0" href="#fn1x0-bk"><sup>1</sup></a>Those who know the game of Tichu might have noticed that we removed consecutive pairs of cards as a valid combination.</p>
<h4>Copyright notice</h4>
<p>
This problem text is copyright by the NWERC 2011 jury. It is
licensed under the Creative Commons Attribution-Share Alike license
version 3.0; The complete license text can be found at:
<a href="http://creativecommons.org/licenses/by-sa/3.0/legalcode">http://creativecommons.org/licenses/by-sa/3.0/legalcode</a>
</p>