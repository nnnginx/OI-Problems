<p>A technique used in early programming contest strategies involved partitioning the available intellectual capacity of a team into a number of members with each member having a fixed amount of intelligence, different members potentially having different amounts. The sum of the brightness of all members equals the total intellectual capacity of the team.</p>
<p>Given a set of problems, it was the task of the team to assign the problems to different team members, so that they could be solved concurrently. This was made difficult due to the fact that the solution time of a problem might depend on the amount of intelligence available to it. Every problem has a minimum intelligence requirement, but if assigned to a brighter member its solution time might increase or decrease.</p>
<p>In this task, you have to determine optimal assignments of problems to team members. Your program is given the intellectual capacities of the team members available for the solution of problems, and for each problem a description of how its solution time depends on the amount of intelligence available to it. Your program has to find the solution schedule of the problems that minimizes the average solution time for the problems. A solution schedule is an assignment of problems to team members and times, such that no two problems use the same member at the same time, and no problem is assigned to a team member with less brightness than its minimum requirement. The solution time of the problem is the difference between the time when the problem was submitted to be solved (which is the start of the contest at time zero for all problems in this task), and the time that the problem is solved.</p>
<h3>Input Specification</h3>
<p>The input data will contain multiple test cases. Each test case begins with a line containing a pair of integers <code>m</code> and <code>n</code>. The number <code>m</code> specifies the number of team members (<code>1 &lt;= m &lt;= 3</code>), and <code>n</code> specifies the number of problems to be solved (<code>1 &lt;= n &lt;= 10</code>).</p>
<p>The next line contains <code>m</code> positive integers giving the intelligence amounts of the <code>m</code> team members. Following this are <code>n</code> lines, describing the time-brightness tradeoffs for each of the <code>n</code> problems. Each line starts with a positive integer <code>k</code> (<code>k &lt;= 10</code>), followed by <code>k</code> pairs of positive integers <code>s<sub>1</sub>,t<sub>1</sub>,s<sub>2</sub>,t<sub>2</sub>,...,s<sub>k</sub>,t<sub>k</sub></code> that satisfy <code>s<sub>i</sub> &lt; s<sub>i+1</sub></code> for <code>1 &lt;= i &lt; k</code>. The minimum intelligence requirement of the problem is <code>s<sub>1</sub></code>, i.e. it cannot be solved by a member with less intellectual capacity than this number. If the problem is solved by a team member with brightness <code>s</code>, where <code>s<sub>i</sub> &lt;= s &lt; s<sub>i+1</sub></code> for some <code>i</code>, then its solution time will be <code>t<sub>i</sub></code>. Finally, if the problem is solved by a team member with intellectual capacity <code>s<sub>k</sub></code> or more, then its execution time will be <code>t<sub>k</sub></code>.</p>
<p>A pair of zeroes will follow the input for the last test case.</p>
<p>You may assume that each problem will be solved in exactly the time specified for the given brightness, regardless of the number of other problems being solved by other team members at the same time. No problem will have an intelligence requirement larger than that of the brightest team member.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Output Specification</h3>
<p>For each test case, first display the case number (starting with <code>1</code> and increasing sequentially). Then print the minimum average solution time for the set of problems with two digits to the right of the decimal point. Follow this by the description of a solution schedule that achieves this average solution time. Display one line for each problem, in the order they were given in the input, that identifies the problem number, the member used to solve it (numbered in the order given in the input), the time when the member started to solve the problem, and the time when the problem was solved. Follow the format shown in the sample output, and print a blank line after each test case.</p>
<h3>Sample Input</h3>
<p>&nbsp;</p>
<pre>2 4
40 60
1 35 4
1 20 3
1 40 10
1 60 7
3 5
10 20 30
2 10 50 12 30
2 10 100 20 25
1 25 19
1 19 41
2 10 18 30 42
0 0
</pre>
<h3>Sample Output</h3>
<p>&nbsp;</p>
<pre>Case 1
Average solution time = 7.75
Problem 1 is solved by member 2 from 0 to 4
Problem 2 is solved by member 1 from 0 to 3
Problem 3 is solved by member 1 from 3 to 13
Problem 4 is solved by member 2 from 4 to 11

Case 2
Average solution time = 35.40
Problem 1 is solved by member 3 from 19 to 49
Problem 2 is solved by member 2 from 0 to 25
Problem 3 is solved by member 3 from 0 to 19
Problem 4 is solved by member 2 from 25 to 66
Problem 5 is solved by member 1 from 0 to 18

</pre>