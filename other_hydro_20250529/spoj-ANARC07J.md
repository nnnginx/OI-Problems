<p>Johnny is on probation! He has failed so many math courses and the Department has forced him to register in a remedial math course. He must pass the course or he'd be expelled from the University. In an attempt to impress his professor, Johnny is typing all his assignments on the computer. The latest assignment is rather simple, Johnny was given a set of problems to solve. Each problem had a list of one or more numbers that Johnny was supposed to add. Johnny has worked all night on the assignment, neatly typing his solution to each problem using a word processor as seen here:</p>
<p>4+12+3=19</p>
<p>As usual, Johnny woke up late, he hardly had the time to print the assignment and rush to class. Only in the classroom did he discover that, due to a printer driver problem, non of the plus signs were printed. The above line was printed as:</p>
<p>4123=19</p>
<p>Write a program to figure out where the pluses are supposed to be. All what Johnny remembers is that all the numbers were positive; None of the numbers, other than possibly the sum, had more than 5 digits; And none of the numbers had a zero as the left-most digit.</p>
<p style="text-align: center;"><strong>Input</strong></p>
<p>The input consists of N ( N &lt;= 100 ) test cases. The number of them (N) is given on the first line of the input file. N lines follows each have an expression. No line will be longer than 256 characters.</p>
<p style="text-align: center;"><strong>Output</strong>&nbsp;<strong>&nbsp;</strong></p>
<p>For each expression in the input, your program must print a line of&nbsp;<em>result. result&nbsp;</em>is the expression with the necessary plus signs in place. There are no spaces in&nbsp;<em>result</em>&nbsp;. If there are more than one possible solution, print a solution that requires the least number of plus signs. Knowing how bad Johnny is in arithmetic, it is possible that there is no solution, in which case your program should print ``IMPOSSIBLE" as the&nbsp;<em>result</em>.</p>
<p style="text-align: center;"><strong>Example</strong></p>
<p><strong>Input:</strong></p>
<p>3<br> 4123=19<br> 15442147612367219875=472<br> 111=8</p>
<p><strong>Output:</strong></p>
<p>4+12+3=19<br> 15+44+21+47+61+23+67+21+98+75=472<br> IMPOSSIBLE</p>
<p>&nbsp;</p>
<pre><span><span style="font-family: 'Times New Roman'; white-space: normal; font-size: small;">
</span></span></pre>