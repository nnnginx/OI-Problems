<p style="text-align: center;"><strong>Problem B</strong></p>
<p style="text-align: center;"><strong>&nbsp;Esperanto Lessons</strong></p>
<p>In a Latin American high school the directors had decided to implement esperanto lessons, because they have observed many of their students started studying the universal language on their own. Because of this, all kids have really different levels before the courses are implemented. The directors decided to implement two levels: basic and advanced. Because of bureaucracy, they cannot put students of different divisions in the same English course. Also, to be fair, the basic and advanced levels have to be equal among all divisions of the school.</p>
<p>Therefore, each division will be partitioned in two subgroups, one for the basic level and one for the advanced level (note that it is possible that a division does not contain any students in one of the levels). To determine the levels, an Esperanto test has been taken by all students of all division, each getting a grade between 0 and 1000, inclusive. To accomplish their mentioned goals, the directors have decided that all students with a score greater than or equal to T will be assigned the advanced level and all students with a score less than T will be assigned the basic level.</p>
<p>However, they cannot decide on the best value of T. They decided to choose the value that better splits all divisions. For this, they have come up with a metric: They want the value of T that minimizes the accumulated difference. That is, the sum of the difference of the number of students in the two groups (basic and advanced) within each division.<strong></strong></p>
<p><strong>Input</strong></p>
<p>Each test case will be given in several lines. The first line contains a single integer N (1&lt;= N&lt;= 10<sup>6</sup>), the number of divisions in the school. 2N lines follow, with each division being described in 2 consecutive lines. The first line of each group of two contain a single integer K (1&lt;=K&lt;=10<sup>6</sup>) the number of people on the division. The second line contains K integers separated by single spaces with the scores of each of the students in the division. The scores will all be between 0 and 1000, inclusive. Total number of students within each test case (that is, the sum of the values of all K lines) will not be greater than 10<sup>6</sup>.<strong></strong></p>
<p><strong>Output</strong></p>
<p>For each test case, output a single line with a single integer representing the value of the accumulated difference if T is chosen optimally.<strong></strong></p>
<p><strong>Sample Input</strong></p>
<p>2</p>
<p>2</p>
<p>1 2</p>
<p>2</p>
<p>3 4</p>
<p>2</p>
<p>2</p>
<p>1 4</p>
<p>2</p>
<p>2 3</p>
<p>3</p>
<p>4</p>
<p>1 10 100 1000</p>
<p>3</p>
<p>5 55 555</p>
<p>5</p>
<p>4 16 64 256 1000</p>
<p>1</p>
<p>4</p>
<p>500 500 500 500</p>
<p>-1<strong></strong></p>
<p><strong>Sample Output</strong></p>
<p>2</p>
<p>0</p>
<p>2</p>
<p>4</p>