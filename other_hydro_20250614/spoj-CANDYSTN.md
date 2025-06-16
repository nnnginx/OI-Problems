<table border="0">
<tbody>
<tr>
<td>
<p align="justify">Little Pratya loves collecting candies and she also likes playing games :).</p>
<p align="justify">Today Pratya is travelling in bus and she has a bag full of <strong>N</strong> candies. She looks outside the window and notices milestones with numbers written on them. She decides to play a game. She wants to select some initial <em>non-zero</em> number of candies from the bag and call it her collection of candies. When she sees a milestone on the way, she will add or remove some candies from her collection as following.</p>
Let the previous milestone number be <strong>a1</strong> and the current milestone number be <strong>a2</strong>.</td>
<td>
<p><img src="./21729/file/E1LPWOVP.png" border="0" alt="pratya1" width="142" height="165"></p>
</td>
</tr>
</tbody>
</table>
<p><strong>a2 &gt; a1 : </strong> Pratya adds ( a2 - a1 ) candies to her collection (thus, her bag of candies loses them). If the bag doesn't contain  at least ( a2 - a1 ) candies, she starts crying. <br><br></p>
<p><strong>a2 &lt; a1 : </strong> Pratya removes ( a1 - a2 ) candies from her collection (thus, her bag of candies gains them). If her collection doesn't contain  more than ( a1 - a2 ) candies, she starts crying.  <br><br></p>
<p><strong>a1 = a2 : </strong> Pratya is bored to see the same number again and so she eats one of the candies from her collection.</p>
<p align="justify">Moreover, Pratya always wants her candy collection to have at least one candy, otherwise she starts crying. Given the numbers written on all the milestones in order, find the minimum number of candies Pratya should select in the beginning so that she doesn't have to cry at all.  If it is not possible , print -1. Note that no change to the collection happens when she sees the first milestone.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contain the number of test cases <strong>T</strong>. Each test case has two lines. The first line specifies <strong>N</strong> and <strong>M</strong>. <strong>N</strong> is the number of candies in the bag and <strong>M</strong> is the total number of milestones. Second line contains <strong>M</strong> integers, the numbers written on the milestones, in the order Pratya sees them.</p>
<p>^ is used for power.</p>
<p>T &lt;= 150</p>
<p>1 &lt;= N &lt;= 10^7</p>
<p>2 &lt;= M &lt;= 10^4</p>
<p>Each milestone number will be between [-10^6,10^6].</p>
<h3>Output</h3>
<p>For each test case output the minimum number of candies that should be selected from the bag or -1 if its not possible</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3<br>10 5<br>1 5 1 -1 -2<br>2 5<br>1 5 1 -1 -2<br>100 3<br>1 2 3<br><br><strong>Output:</strong><br>4<br>-1<br>1<br></pre>
<p>Note : Large input, prefer using scanf / printf&nbsp; to&nbsp; cin / cout<br> <em>* There are multiple test sets, and the judge shows the <strong>sum</strong> of the time taken over all test sets of your submission, if Accepted.</em></p>