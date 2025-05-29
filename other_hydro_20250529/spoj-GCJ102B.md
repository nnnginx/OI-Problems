<h3>Problem</h3>
<p>After four years, it is the World Cup time again and Varva is on his way  to South Africa, just in time to catch the second stage of the  tournament.</p>
<p>In the second stage (also called the knockout stage), each match always  has a winner; the winning team proceeds to the next round while the  losing team is eliminated from the tournament. There are 2<sup>P</sup> teams competing in this stage, identified with integers from 0 to 2<sup>P</sup> - 1. The knockout stage consists of P rounds. In each round, each  remaining team plays exactly one match. The exact pairs and the order of  matches are determined by successively choosing two remaining teams  with lowest identifiers and pairing them in a match. After all matches  in one round are finished, the next round starts.</p>
<p><br><br> &nbsp;&nbsp;&nbsp;<img src="file://rYvFEuHI.png" alt=""> <br><br></p>
<p>In order to help him decide which matches to see, Varva has compiled a  list of constraints based on how much he likes a particular team.  Specifically, for each team <code>i</code> he is  <strong>willing to miss at most</strong> <code>M[i]</code> matches the team plays in the tournament.</p>
<p>Varva needs to buy a set of tickets that will guarantee that his  preferences are satisfied, regardless of how the matches turn out. Other  than that, he just wants to spend as little money as possible. Your  goal is to find the <strong>minimal amount of money</strong> he needs to spend on the tickets.</p>
<p>Tickets for the matches need to be purchased in advance (before the  tournament starts) and the ticket price for each match is known. Note  that, in the small input, ticket prices for all matches will be equal,  while in the large input, they may be different.</p>
<h3>Example</h3>
<p>A sample tournament schedule along with the ticket prices is given in  the figure above. Suppose that the constraints are given by the array <code>M = {1, 2, 3, 2, 1, 0, 1, 3}</code>,  the optimal strategy is as follows: Since we can't miss any games of  team 5, we'll need to spend  50, 400, and 800 to buy tickets to all the  matches team 5 may play in. Now, the constrains for the other teams are  also satisfied by these tickets, except for team 0. The best option to  fix this is to buy the ticket for team 0's first round match, spending  another 100, bringing the total to 1350.</p>
<h3>Input</h3>
<p>The first line of the input gives the number of test cases, <strong>T</strong>.  <strong>T</strong> test cases follow.  Each case starts with a line containing a single integer <strong>P</strong>. The next line contains 2<sup>P</sup> integers -- the constraints <code>M[0]</code>, ..., <code>M[2<sup>P</sup>-1]</code>.</p>
<p>&nbsp;</p>
<p>The following block of <strong>P</strong> lines contains the ticket prices for all matches: the first line of the block contains 2<sup>P-1</sup> integers -- ticket prices  for first round matches, the second line of the block contains 2<sup>P-2</sup> integers -- ticket prices for second round matches, etc. The last of the <strong>P</strong> lines contains a single integer -- ticket price for the final match of  the World Cup. The prices are listed in the order the matches are  played.</p>
<h3>Output</h3>
<p>For each test case, output one line containing "Case #x: y", where x is  the case number (starting from 1) and y is the minimal amount of money  Varva needs to spend on tickets as described above.</p>
<h3>Limits</h3>
<p>1 ¡Ü <strong>T</strong> ¡Ü 50<br> 1 ¡Ü <strong>P</strong> ¡Ü 10<br> Each element of <strong>M</strong> is an integer between 0 and <strong>P</strong>, inclusive.</p>
<h4>Large dataset</h4>
<p>All the prices are integers between 0 and 100000, inclusive.</p>
<h3>Sample</h3>
<table border="0">
<tbody>
<tr>
<td><br> <span>Input</span> <br>&nbsp;</td>
<td><br> <span>Output</span> <br>&nbsp;</td>
</tr>
<tr>
<td><code> 2 <br> 2 <br> 1 1 0 1 <br> 1 1 <br> 1 <br> 3 <br> 1 2 3 2 1 0 1 3 <br> 100 150 50 90 <br> 500 400 <br> 800 <br> </code></td>
<td><code> Case #1: 2<br> Case #2: 1350<br> </code></td>
</tr>
</tbody>
</table>