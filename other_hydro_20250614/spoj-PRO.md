<p>A large Bytelandian supermarket chain has asked you to write a program for the simulating costs of a promotion being prepared. 

</p><p>The promotion has to follow the following rules: 

</p><ul>
<li>A customer who wants to participate in the promotion, writes on the receipt, paid by himself, his personal details and throws it into a special ballot box. 
</li><li>At the end of every day of the promotion, two bills are taken out from the ballot box: 
<ul>
<li> first, the receipt amounting to the largest sum is chosen, 
</li><li> then the receipt amounting to the smallest sum is chosen; 
</li></ul>
The customer who has paid the largest sum gets a money prize equal to the difference between the sum on his bill and the sum on the bill amounting to the smallest sum. 
</li><li>
To avoid multiple prizes for one purchase, both bills selected according to the above rules are not returned to the ballot box, but all remaining bills still participate in the promotion. 
</li></ul>
<p> The turnover of the supermarket is very big, thus an assumption can be made, that at the end of every day, before taking out receipts amounting to the largest and the smallest sum, there are at least 2 receipts in the ballot box. 

</p><p> Your task is to compute (on the basis of information about prices on receipts thrown into the ballot box on each day of promotion) what the total cost of prizes during the whole promotion will be. 
</p><p>
Write a program, which: reads from the standard input a list of prices on receipts thrown into the ballot box on each day of the promotion, computes the total cost of prizes paid in consecutive days of promotion, then writes the result to the standard output. 

</p><h3>Input</h3>
<p>The first line of the input contains one positive integer n (1 &lt;= n &lt;= 5000), which is the duration of promotion in days. 

Each of the next n lines consists of a sequence of non-negative integers separated by single spaces. Numbers in the (i+1)-th line of the file represent prices on receipts thrown into the ballot box on the i-th day of promotion. The first integer in the line is k, 0 &lt;= k &lt;= 10^5, the number of receipts on the day, and the next k numbers are positive integers standing for the sums on receipts; none of these numbers is larger than 10^6. 
</p><p>
The total number of bills thrown into the ballot box during the whole promotion does not exceed 10^6. 

</p><h3>Output</h3>
<p>The output should contain exactly one integer, equal to the total cost of prizes paid during the whole promotion. 

</p><h3>Example</h3>

<pre><b>Input:</b>
5
3 1 2 3
2 1 1
4 10 5 5 1
0
1 2

<b>Output:</b>
19
</pre>