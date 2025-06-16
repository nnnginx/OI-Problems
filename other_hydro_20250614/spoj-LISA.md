<p>Young people spend a lot of money on things like  sweets, music CDs, mobile phones and so on.  But most young girls/boys have one problem:  Their pocket money is not enough for all these jolly things.  Little Lisa Listig is one of these poor girls with a small pocket money budget. Last month her pocket money lasted only one week. So she decided to enter into negotiations with her father. Her father Tomm - a mathematician - had an incredibly ingenious idea: He wrote down some fancy digits with operators (+,*) in between them on a sheet of paper and allowed Lisa to insert brackets.  Then he declared that the result of that arithmetic expression is Lisa's new pocket money.   Now it's Lisa's task to maximize her pocket money.  As her father was surprised what a huge sum of money Lisa got for her result, he decided to minimize the result of the expression for his son Manfred.  Now it's your task to calculate the results obtained by Lisa and her father.</p>

<h3>Input</h3>
<p>The first line of input contains the number of testcases k ( k&lt; 5000 ).  Each of the following k lines consists of an arithemtic expression. This expression consists of numbers (0-9) seperated by one of the two operators  '*' and '+'.  There are no spaces between the characters. Each line contains less than 100 characters.</p>

<h3>Output</h3>
<p>For each expression output the result obtained by Lisa and the result obtained by her father separated by one space. The results of the calculations are smaller than 2<sup>64</sup>.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
1
1+2*3+4*5

<strong>Output:</strong>
105 27</pre>

<p>Two possible expressions for the first testcase:</p>
<pre>105 = (1+2)*(3+4)*5
27  = 1+2*3+4*5
</pre>