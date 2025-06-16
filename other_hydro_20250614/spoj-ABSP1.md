<p>Recently Mr. Kopa Samsu is learning programming. On a very renowned online judge, he found a problem:</p>
<p>You are given an array of N numbers in non-decreasing order. You have to answer the summation of the absolute difference of all distinct pairs in the given array.</p>
<p>Do you know what distinct pair means? Suppose you have an array of 3 elements: 3 5 6</p>
<p>Then all the distinct pairs are:</p>
<p>
3 5<br>
3 6<br>
5 6
</p>

<p>For this problem, Mr. Kopa Samsu implemented an algorithm to find the summation of the absolute difference of all distinct pairs. His algorithm was:</p>
<pre>int ABS(int a[], int n)
{
&nbsp; &nbsp; int sum = 0;
&nbsp; &nbsp; for (int i = 1; i &lt;= n ;i++)
&nbsp; &nbsp; {
&nbsp; &nbsp; &nbsp; &nbsp; for (int j = i + 1; j &lt;= n; j++)
&nbsp; &nbsp; &nbsp; &nbsp; {
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; sum += abs(a[i] - a[j]);
&nbsp; &nbsp; &nbsp; &nbsp; }
&nbsp; &nbsp; }
}</pre>

<p>
After a great hard work, he finished the code. But alas!!! Frustration came around him when he submitted his code, the judge gave the verdict ¡°TLE¡± (Time Limit Exit). ¡°How can I get rid of TLE?¡± he thought a lot but couldn't find any way. Then suddenly, he remembered about you that you (his friend) is very good at programming. So, he came to you seeking your help. Can you help him solving this problem?</p>

<h3>Input</h3>
<p>The input data set starts with an integer T (T &lt;= 1000), the number of test cases. Then every test case starts with a integer N (N &lt;= 10000), the number of elements in the array. After that, the next line contains N integers A[i], where 1 &lt;= i &lt;= N and 1 &lt;= A[i] &lt;= 1000000000 &amp; A[i] &lt;= A[i+1].</p>

<h3>Output</h3>
<p>Every test case should output an integer ¡°X¡±, where X is the summation of the absolute difference of all the distinct pair.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
3
1 2 3
3
1 4 5
3
2 4 6

<strong>Output:</strong>
4
8
8</pre>

<pre>Problem Set: S.M. Shaheen Sha, Raihat Zaman Neloy
Data Set &amp; Solution: Raihat Zamane Neloy</pre>