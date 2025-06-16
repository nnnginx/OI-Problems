<p>Once upon a time in a kingdom far far away, the royal treasury started getting emptier and emptier. The king decided to change the situation and he invented a new system of cooperation with in the office of the royal treasurer. The clerks of the office are supposed to form pairs (in order to avoid being bribed) in such away that each pair is formed by a clerk and his/her direct subordinate. Your task is to compute, given the structure of the office of the treasurer, the maximum number of pairs that can be formed this way and in how many 
different ways this is possible.<br>  
<br>
The office of the treasurer is led by George Skinflint. Each clerk has zero, one or more subordinates and is a subordinate of a single clerk (except for George Skinflint who is responsible only to the king himself). The number of clerks does not exceed 1000. Your task is to compute the maximum number of pairs that can be formed by clerks in such a way that every pair is formed by a clerk and his/her direct subordinate. In 
addition, you should also compute the number of ways such pairs can be formed. Note that some clerks need not be contained in a pair.  

</p><h3>Input</h3>
<p><b>The input contains multiple testcases.</b></p> 

<p>The first line of each testcase contains a single number N that represents the number of clerks 1 &lt;= N &lt;= 1000. The clerks are assigned unique ID numbers from the range between 1 and N. The ID number of the treasurer (Skinflint) is 1. Each of the following N lines corresponds to one of the clerks: it contains his/her ID number, the number K of his/her subordinates, 0 &lt;= K &lt;= 999, and the ID numbers of his/her K subordinates separated by single spaces. You can assume that the line corresponding to a clerk never appears before the line corresponding to his/her supervisor.</p>   

<h3>Output</h3>
<p>The output for each testcase should consist of two lines. The first line of the output should contain a single number that represents the maximum number M of pairs that the clerks can form. The second line should contain the number of  
different ways in which the clerks can form M pairs obeying the rules given by the king.   

</p><h3>Example</h3>

<pre><b>Input:</b>
7
1 3 2 4 7
2 1 3
4 1 6
3 0
7 1 5
5 0
6 0

<b>Output:</b>
3
4
</pre>