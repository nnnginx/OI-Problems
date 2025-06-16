<p>There are two tables. These tables are filled with numeric data. Each column of each table has a unique name. You need to implement JOIN operation for those tables. JOIN creates a new result table by combining column values of the two tables based upon the join-predicate. The query compares each row of the first table with each row of the second to find all pairs of rows which satisfy the join-predicate. When the join-predicate is satisfied, column values for each matched pair of rows of the table are combined into a result row. The result of the join can be defined as the outcome of first taking the Cartesian product of all records in the tables (combining every record in the first table with every record in the second table) - then return all the records which satisfy the join predicate. After that needed column are picked and printed as the result. Moreover the resulting rows should be output in the lexicographic order.

</p><h3>Input</h3>
<p>The input starts with the description of the first table. The first line consists of k<sub>1</sub> names of the columns of the table separated with spaces. All the names contain only small latin letters and digits. Next line contain number n<sub>1</sub> ¨C the amount of records in the table. In each of the next n<sub>1</sub> lines there are k<sub>1</sub> integers ¨C data written in the table. The description of the second table in the same format follows. Next line is number q ¨C the amount of queries. The description of each query follows in the following format:</p><p>
</p><pre>SELECT &lt;list of the names of columns&gt;
JOIN ON &lt;a name of the column from the first table&gt;=&lt;a name of the column of the second table&gt;
</pre>

<h3>Constraints</h3>
<p>2 &lt;= k<sub>1</sub>, k<sub>2</sub> &lt;= 10<br>
1 &lt;= n<sub>1</sub>, n<sub>2</sub> &lt;= 50000<br>
All the integers in the tables are positive and less than 100000.<br>
1 &lt;= q &lt;= 10

</p><h3>Output</h3>
<p>For each query print the result of JOIN operation. You should print only the columns given in the query and in the appropriate order. The rows should be ordered lexicographically. The result of each query won't contain more than 50000 records. Print blank line after the answer for each query. See the example for more information.

</p><h3>Example</h3>

<pre><b>Input:</b>
id1 a b
4
1 2 3
2 2 3
3 2 4
2 4 4
id2 c d
3
3 3 3
5 2 1
1 3 4
3
SELECT a,b,c
JOIN ON id1=d
SELECT id1,d
JOIN ON a=c
SELECT id2,id1,d
JOIN ON b=c

<b>Output:</b>
a b c
2 3 2
2 4 3

id1 d
1 1
2 1
3 1

id2 id1 d
1 1 4
1 2 4
3 1 3
3 2 3

</pre>