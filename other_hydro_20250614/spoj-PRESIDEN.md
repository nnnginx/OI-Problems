<p style="font-family: 'Times New Roman'; font-size: medium;">Finally, it is time to vote for a new president and you are really excited about that. You know that the final results may take weeks to be announced, while you can't really wait to see the results.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">Somehow you managed to get the preferences list for every voter (we don't care how you managed to get this piece of information!). Each voter sorted out all candidates starting by his most preferred candidate and ending with his least preferred one. When voting, a voter votes for the candidate who comes first in his preferences list. For example, if there are 5 candidates (numbered 1 to 5), and the preferences list for one voter is [3, 2, 5, 1, 4] and the current competing candidates in the voting process are candidates 2 and 4, the voter will vote for candidate number 2.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">Here are the rules for the election process:</p>
<ol style="font-family: 'Times New Roman'; font-size: medium;">
<li>There are&nbsp;<span><em>C</em></span>&nbsp;candidates (numbered from 1 to&nbsp;<span><em>C</em></span>), and&nbsp;<span><em>V</em></span>&nbsp;voters (<span><em>V</em></span>&nbsp;is always an odd number).</li>
<li>The election process consists of up to 2 rounds. All candidates compete in the the first round. If a candidate receives more than 50% of the votes, he wins, otherwise another round takes place, in which only the top 2 candidates compete for the presidency. The candidate who receives more votes than his opponent wins and becomes the new president.</li>
<li>You can safely assume that the given preferences will never cause a situation in which the second and the third candidates from the first round receive the same number of votes.</li>
<li>The voters' preferences are the same in both rounds, and each voter must vote exactly once in each round for a currently competing candidate according to his preferences.</li>
</ol>
<p style="font-family: 'Times New Roman'; font-size: medium;">Given the preferences lists, you need to write a program to figure out which candidate will win and in which round.</p>
<h3>Input</h3>
<p><span style="font-family: 'Times New Roman'; font-size: medium;">Your program will be tested on one or more test cases. The first line of the input will be a single integer&nbsp;</span><span style="font-family: 'Times New Roman'; font-size: medium;"><em>T</em></span><span style="font-family: 'Times New Roman'; font-size: medium;">, the number of test cases&nbsp;</span><span style="font-family: 'Times New Roman'; font-size: medium;">(1<img src="file://QovgN75o.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>T</em><img src="file://8zNwxKRy.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE">100)</span><span style="font-family: 'Times New Roman'; font-size: medium;">. Followed by the test cases, the first line of a test case contains two integers&nbsp;</span><span style="font-family: 'Times New Roman'; font-size: medium;"><em>C</em></span><span style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;and&nbsp;</span><span style="font-family: 'Times New Roman'; font-size: medium;"><em>V</em></span><span style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;separated by a single space.&nbsp;</span><span style="font-family: 'Times New Roman'; font-size: medium;"><em>C</em></span><span style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;and&nbsp;</span><span style="font-family: 'Times New Roman'; font-size: medium;"><em>V</em></span><span style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</span><span style="font-family: 'Times New Roman'; font-size: medium;">(1<img src="file://4PaPHlxM.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>C</em>,&nbsp;<em>V</em><img src="file://wlcLC1bJ.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE">100)</span><span style="font-family: 'Times New Roman'; font-size: medium;">represent the number of candidates and voters respectively, followed by&nbsp;</span><span style="font-family: 'Times New Roman'; font-size: medium;"><em>V</em></span><span style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;lines each line contains&nbsp;</span><span style="font-family: 'Times New Roman'; font-size: medium;"><em>C</em></span><span style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;integers separated by a single space, representing the preferences list for a single voter (the first is his most preferable candidate while the last is his least preferable one). Each integer from 1 to&nbsp;</span><span style="font-family: 'Times New Roman'; font-size: medium;"><em>C</em></span><span style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;will appear exactly once in each line.</span></p>
<h3>Output</h3>
<p><span style="font-family: 'Times New Roman'; font-size: medium;">For each test case, print on a single line two integers separated by a single space. The first integer is the ID of the winner candidate (a number from 1 to C), the second integer is cither 1 or 2 indicating whether this candidate will win in the first round or the second one respectively.</span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre>2 
2 3
2 1
1 2
2 1
3 5
1 2 3
1 2 3
2 1 3
2 3 1 
3 2 1</pre>
<strong>Output:</strong>
<pre>2 1
2 2</pre>
</pre>