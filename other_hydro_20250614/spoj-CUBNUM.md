<p>For any positive integer n, n can be represented as sum of other positive cube numbers (n=a<sub>1</sub><sup>3</sup>+a<sub>2</sub><sup>3</sup>+...+a<sub>m</sub><sup>3</sup>). 
Your task is to print the smallest m, where m is number of cube numbers used to form n, such that n=a<sub>1</sub><sup>3</sup>+a<sub>2</sub><sup>3</sup>+...+a<sub>m</sub><sup>3</sup>.
For example: 
</p><ul>
<li>n=5,n=1<sup>3</sup>+1<sup>3</sup>+1<sup>3</sup>+1<sup>3</sup>+1<sup>3</sup> (m=5)</li>
<li>n=8,n=2<sup>3</sup> (m=1)</li>
<li>n=35,n=2<sup>3</sup>+3<sup>3</sup> (m=2)</li><p></p></ul>
<b>Note: My fastest time is 0.09s :). <br>Edit: My fastest time is 0.05s now lol<br> My Java solution is also accepted.</b>
<h3>Input</h3>
<p>Input consists of several test cases separated by new lines. Each test case consists of a positive integer, denoting the number of n (1 ¡Ü n ¡Ü 10<sup>5</sup>). Input is terminated by end of file (EOF).<br> It is guaranteed that total test case per input file is less than 10<sup>5</sup>.
<br><br> <b> Note: For c++ users, you can use 	while(scanf("%d",&amp;n)!=EOF); to read input until EOF.<br>Warning: large Input/Output data, be careful with certain languages!.</b>
</p>
<h3>Output</h3>
<p>For each case, print "Case #X: M", where X (1 ¡Ü X ¡Ü 10<sup>5</sup>) is the case number,and M is the minimum cube numbers used to form the integer n. There must be no trailing spaces at the end of printed lines, neither empty characters. Print a newline after each testcase. 

</p><h3>Example</h3>

<pre><b>Input:</b>
1
2
5
8
35

<b>Output:</b>
Case #1: 1
Case #2: 2
Case #3: 5
Case #4: 1
Case #5: 2

</pre>