<p>We want to pick a certain number of people from a group of N people and make them play a game of&nbsp;tug of war!</p>
<p>Then, we would like to split these people into two teams.</p>
<p>Afterwards, an intense game of tug of war would start.</p>
<p>However, when the strength of each team is not equivalent, the game is not very fun.&nbsp;A team's strength is the sum of the strengths of the people in the team.</p>
<p>Since you want the game that is fun, it is necessary to determine if it is possible to pick some people and split them into two teams such that the two teams' strengths are equal.</p>
<h3>Input</h3>
<p>The input consists of a number of test cases.</p>
<p>The first line is the number of test case, T. (1&lt;=T&lt;=200)</p>
<p>Each case starts with N (1&lt;=N&lt;=100,000), the total&nbsp;number of people.</p>
<p>The next line consists of N integers, separated by a space. The ith integer indicates the strength of the ith person. These integers&nbsp;are less than 100, but larger than 0.&nbsp;</p>
<h3>Output</h3>
<p>For each test case, output "YES" if it is possible to pick some people from the group and separate into two teams of equal strengths. If not, output "NO". Refer to the&nbsp;sample test cases for further clarifications.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>4<br>10 20 30 40<br>3<br>10 18 15<br><br><br>
<strong>Output:</strong>
YES<br>NO </pre>
<pre>There are a number of ways to pick teams for the first test case. One example would be {10,20} and {30}.<br></pre>