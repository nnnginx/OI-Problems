<p>
Jasio is a little boy - he is only three years old and enjoys playing with toy cars very much. Jasio has n different cars. They are kept on a shelf so high, that Jasio cannot reach it by himself. As there is little space in his room, at no moment may there be more than k toy cars on the floor. 

Jasio plays with one of the cars on the floor. Jasio's mother remains in the room with her son all the time. When Jasio wants to play with another car that is on the floor, he reaches it by himself. But when the toy is on the shelf, his mummy has to hand it to him. When she gives Jasio one car, she can at the same time pick any car from the floor and put it back on the shelf (so that there remains sufficient space on the floor).

The mother knows her child very well and therefore can predict perfectly which cars Jasio will want to play with. Having this knowledge, she wants to minimize the number of times she has to hand Jasio a toy from the shelf. Keeping that in mind, she has to put the toys off on the shelf extremely thoughtfully.
</p><p>
<b>Task</b>
</p><p>
Write a programme that:
</p><p>
<b>1.</b>reads from the standard input the sequence of toy cars in order in which Jasio will want to play with them,
</p><p>
<b>2.</b>calculates the minimal number of times the mother has to pick cars from the shelf,
</p><p>
<b>3.</b>writes the result to the standard output. 

</p><h3>Input</h3>
<p>
In the first line of the standard input is H- the number of test case (H &lt;= 16). For each test case follow contains some lines, start with three integers: n, k, p (1 &lt;= k &lt;= n &lt;= 100000, 1 &lt;= p &lt;= 500000), separated by single spaces. These denote respectively: the total number of cars, the number of cars that can remain on the floor at once and the length of the sequence of cars which Jasio will want to play with. Each of the following p lines contains one integer. These integers are the numbers of cars Jasio will want to play with (the cars are numbered from 1 to n ). 

</p><h3>Output</h3>
<p>
For each test case, you should write only one integer - the minimal number of times his mother has to pick a car from the shelf. 

</p><h3>Example</h3>
<pre><b>Input:</b>
1
3 2 7
1
2
3
1
3
1
2

<b>Output:</b>
4
</pre>