<p>In a galaxy far far away, there exists a silicon based form of life, who call themselves stabards. Unlike humans, the stabards are multi-gendered. Therefore, when two stabards form a partnership (known as mating in earth parlance), one stabard would be the donor of genetic material and the other would be the combinator of the genetic material. Of course, the combinator had the tougher task, to combine the genetic material and create a new stabard.
<br><br>
Early on, the wise stabards realized that due to the increased number of genders, every stabard was likely to waste his time trying to find a suitable partner. After that, due to the tremendous opportunity, every stabard would waste some more time trying to cheat on his partner by forming more partnerships (especially the donors since they had nothing much to do). Therefore, the wise ones made the following rules about partnerships:
</p><ol>
<li> Each stabard can form at most two partnerships.</li>
<li>In order to maintain a sense of balance, a stabard cannot play the same role (donor/combinator) in both partnerships.</li>
<li>The partnerships shall be formed such that the total number of them is maximized.</li>
</ol>

<p>To ensure all rules are being followed, the wise ones send the stabard data every year to earth and wish to know the maximum number of partnerships that can be formed.

</p><h3>Input</h3>
<p>For each test case, two integers M (the number of stabard genders) and N (the total number of stabards) are given on the first line. M lines follow, each consisting of M characters. The j-th character on the i-th line denotes what would happen if a stabard of gender i formed a partnership with a stabard of gender j. It will be either
<br><br>
'X' �C such a partnership is forbidden.
<br><br>
'D' �C stabard of gender i would be the donor.
<br><br>
'C' �C stabard of gender i would be the combinator.
<br><br>
After the M lines, N space separated integers are given on a single line. The i-th integer gives the gender of the i-th stabard.
<br><br>
The end of the test cases is given by a line with M and N both being 0. This test case should not be processed. The total number of test cases will be &lt;= 100.

</p><h3>Constraints</h3>
<p>0 &lt; M &lt;= 100
<br><br>
0 &lt; N &lt;= 100
<br><br>
The gender data for stabards will be symmetric and consistent. (i.e. character i on line j will not conflict with character j on line i). Two stabards of the same gender can never partner each other. (The wise ones fear this will pollute the gene pool. Moreover, big fights would break out as who would be the donor.) The gender given for each stabard will be between 0 and M-1 inclusive.

</p><h3>Output</h3>
<p>For each test case, a single integer giving the total number of partnerships. Each integer must be on its own line.

</p><h3>Example</h3>

<pre><b>Input:</b>
2 4
XD
CX
0 0 1 1
3 3
XDC
CXD
DCX
0 1 2
0 0

<b>Output:</b>
2
3
</pre>