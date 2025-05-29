<p>
LoadingTime has been given a task these days. He is required to write a tool called Text Generator. This software is widely used among the kids who are under seven. It generates an article with the size of a given number L for users. If an article contains at least one word which the users know, we consider it readable. Now, LoadingTime wants to know, how many readable articles can it generates, and he can improve his Text Generator. Could you help him?? </p>

<h3>Input</h3>

<p>The input contains multiple test cases.</p>
<p>The first
line of each test case contains two integer N (1 &lt;= N &lt;= 10), L
(1 &lt;= L &lt;= 1000000). The following N lines contain N words representing
the words knew by the users. All the words and the generated article only
contain uppercase letters, and the length of each word is not greater than 6. 
</p>

<h3>Output</h3>

<p>For each test case, your program should output a integer as LoadingTime
required. As the number could be quite large, you only need to print
the answer modulo 10007. 

</p><h3>Example</h3>
<pre><b>Input:</b>
2 2
A
B
2 10000
ABC
B

<b>Output:</b>
100
5960

</pre>