<p>
Before the ACM-ACPC regional contest, the site director and the volunteers were very busy preparing for the contest. One of their tasks is to assign a table for each team such that no two teams from&nbsp;the same university are adjacent to each other. The site director decided not to waste his time doing this task and asked the judges to do it. The judges thought this could be a good problem to be used in&nbsp;the contest problems set. As they were very busy preparing for the contest, the judges decided to solve part of the problem and ask the contestants to solve the rest.
</p>

<p>
The judges will generate a number of layouts for the teams assignment to the tables and will ask the contestants to write a program to check whether each of these layouts is valid or not. If a layout is not valid the program should count how many different universities have at least two of their teams sitting adjacent to each other. "Well, you may use those solutions for the next year's contest",&nbsp;said by the chief judge&nbsp;<em>Ahmed Aly</em>&nbsp;to the site director.
</p>

<p>
The contest hall can be represented as a 2D grid of&nbsp;<strong>N</strong>&nbsp;rows with&nbsp;<strong>M</strong>&nbsp;cells in each row. Each cell in the grid is either occupied by a team or empty. There could be up to 8 teams adjacent to a single team.&nbsp;A team may have less than 8 adjacent teams if it is seated next to a hall edge or some of its adjacent cells are empty.
</p>

<p>
For example, in the layout shown in the following figure, team E has 7 adjacent teams, named A, B, C, D, F, G and H, while the adjacent teams to team A are B, D and E.
</p>

<center>
<img src="./21926/file/cixJQMTs.png" border="0" width="254" height="254">
</center>

<h3>Input</h3>
<p>
Your program will be tested on one or more test cases. The first line of the input will be a single integer&nbsp;<strong>T</strong>, the number of test cases&nbsp;(1 ¡Ü <strong>T</strong> ¡Ü 100). Followed by the test cases, each one starts with a line containing 2 integers separated by a single space&nbsp;<strong>N</strong>&nbsp;and&nbsp;<strong>M</strong>&nbsp;(1 ¡Ü <strong>N</strong>,&nbsp;<strong>M</strong> ¡Ü 100)&nbsp;representing the dimensions of the hall, followed by&nbsp;<strong>N</strong>&nbsp;lines each line contains&nbsp;<strong>M</strong>&nbsp;integers separated by a single space, representing the tables assignment in this row. Each integer represents the university ID of the team assigned to this table or '<tt>-1</tt>' if it is empty. All universities IDs are positive integers not greater than 100.</p>

<h3>Output</h3>
<p>
For each test case, print on a single line integer, the number of different universities having at least two of their teams adjacent to each other.
</p>

<h3>Example</h3>
<pre><strong>Sample Input</strong>
3
3 3
1 2 3
2 2 2 
1 1 1
3 3 
1 2 3 
3 -1 1 
2 -1 2 
3 3 
1 2 3 
-1 1 5 
1 2 4

<strong>Sample Output</strong>
2 
0 
1</pre>