<p>&nbsp;</p>
<p>Arya is very fond of fibonacci numbers.He claimed he can solve any problem on fibonacci number.His clever friend golu gave him a challengeÂ</p>
<p>to prove his skills.He gave him a sequence which he called exponacci.The sequence is given by<br><strong>g(n)=2^f(n-1)</strong>for n&gt;0<br><strong>g(0)=1</strong>for n==0<br>f(n) denotes the nth fibonacci number where<br>f(0)=1<br>f(1)=1(Obviously golu is not as good as arya in fibonacci numbers so he believes f(0)=1,anyways we have chosen not to disturb him)<br>f(n)=f(n-1)+f(n-2)for n&gt;1<br>Help arya to find the nth exponacci number.Since the numbers can be very large take mod 10^9+7</p>
<p><strong>Input :</strong>Â <br>The first line of the input will be the number of test cases(T&lt;=2000). For each test case first line contains one integers n 0 &lt;= n &lt;= 10^15</p>
<p><strong>Output :</strong><br>The value of g(n)%(10^9+7)</p>
<p><strong><span style="text-decoration: underline;"><span style="color: red; font-size: large;">Warning: value of n won't fit in int,use long long int instead </span> </span> </strong></p>
<pre>Sample Cases :
Input:
2
3
5
 
Output:
4
32
</pre>