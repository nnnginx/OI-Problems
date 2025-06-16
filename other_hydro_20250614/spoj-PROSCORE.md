<p>Fegla, one of the ACM ICPC coaches, is very happy as one of his teams won the ACPC regional contest, and now he is preparing his team for the ACM ICPC World Final. He decided to establish a training camp for his team in the north coast, practicing on subset of problem sets from previous World Final contests to sharpen the team skills, but he needs to choose this subset wisely as World Final is soon.</p>
<p>After a long discussion with his team, they agreed on a certain criteria to choose the problem sets that will help in the training. Considering a problem set with N teams and P problems, a good problem set must satisfy the following conditions to be chosen:</p>
<ol>
<li>Any problem is solved by at least one team.</li>
<li>Minimum number of solved problems per team is one.</li>
<li>Maximum number of solved problems per team is less than p.</li>
</ol>
<p>&nbsp;</p>
<p>Although they are all programmers, these lazy guys would to ask for your help in writing a program to calculate that for them. We really doubt that they will do something in the World Finals with such behavior,&nbsp; so kindly help them, even if you are not from their school to state these 3 conditions for a given problem set. But, push them for some work, represent the true condition as 1 and the false condition as 0, and then convert the result to a decimal number to be the problem set score. Let the first condition to be the most left bit, the third condition to be the right most bit and the second condition to be middle bit. E.g. if a problem set matched only the first condition, it's represented as "100" and converted to 4.</p>
<p><strong>Input Specification:</strong></p>
<p>First line contains an integer T that represents the number of test cases, then follow T test cases, each in the following format: Line 1 contains two integers N and P, space separated, where 0 &lt; N, P ¡Ü&nbsp; 10. Then N lines each contains P integers are followed, where i-th line and j-th column represent (team=i, problem=j) state: 1 if problem is solved and 0 otherwise.</p>
<p><strong>Output Specification:</strong></p>
<p>For each test case, print on one line, ¡°Case K: score¡± where K is the Test Case number and score is the problem set score.</p>
<p><strong>Sample input:</strong></p>
<p>1<br>2 3<br>1 1 1<br>0 0 0</p>
<p><strong>Sample Output:</strong></p>
<p>Case 1: 4</p>