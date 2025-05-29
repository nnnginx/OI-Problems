<p>The Kazooba tribe contains N men, who want to gather for a tribe council. The men are all descendants of a single one, who is the chief of the tribe. Since the people of this tribe are quite long lived, every person's ancestors, including the chief, are alive and will be attending the council.
</p><p>The men arrive at the council in some particular order and they are seated as they arrive. The men sit in a row of parallel tables. The first table is at the base of the Holy Mountain and the row extends indefinitely to the West (away from the Mountain). Unfortunately, each man doesn't get along with his father and his sons, so he doesn't want to sit at the same table with any of them. On the other hand, each man wants to be as close to divinity as possible, so, when he arrives at the council, he goes to the table closest to the Holy Mountain, where none of his children or father is already seated.
</p><p>As usual, the Gods of the tribe have a certain inclination for grandeur. Therefore, they would like to command the men to arrive in such an order, as to maximize the number of tables that are occupied. Unfortunately, they do not have any inclination for programming, so they have ordered you to write a program for that.
</p><p>Write a program that determines the maximum number of tables that can end up being occupied.

</p><h3>Input</h3>
<p>The first line of the input file contains an integer N, representing the number of men in the tribe. All men are numbered from 1 to N; the chief is number 1. Each of the following lines describe a father�Cson relation and
contains two integers A B separated by a blank, meaning that person number A is the father of the person number
B. The relations described in the file are correct (for instance, there are no "cycles" and each person is a
descendent of the chief).


</p><h3>Output</h3>
<p>The output file should contain a single line with the maximum number of tables that can be occupied.

</p><h3>Example</h3>

<pre><b>Input:</b>
5
1 4
3 2
1 3
3 5

<b>Output:</b>
3


<b>Explanation:</b> 
If men arrive in the order 2 4 1 5 3, the following happens:
<ul><li>2 goes to the first table</li><li>4 goes to the first table</li><li>1 has a son (4) at the first table, so he goes to the second table</li><li>5 goes to the first table</li><li>3 has two sons at the first table (2 and 5) and his father (1) is at
the second table, so he goes to the third table</li>
</ul></pre>

<h3>Constraints</h3>
<ul><li>1 &lt; N &lt;= 100 000</li>
<li>Any table has unlimited capacity.</li></ul>

<b>Note</b>: The problem statement and test data was updated on 22-11-2008. I'm sorry for the inconvenience.