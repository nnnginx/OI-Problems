<p>DCE Coders mentors got fed up by making problems, they are deciding upon the toughest problem for contest. Everybody started to tease Ankur sir that he can¡¯t make a single tough problem for juniors. He got very angry, now you only handle Ankur sir¡¯s anger (Beware: All the tough number theory problems given to you as assignments are like 2+2=4 for Ankur sir). Here is the problem given by him (Say thanks to Jyoti ma¡¯am that she softens the problem slightly.. ;)). You are given an integer n.&nbsp; There will be 2 different numbers K1 and K2, such that K1*K2 = n.</p>
<p>Both of which satisfies the equation &nbsp;(Totient(K!) &nbsp;mod K) !=0. &nbsp;</p>
<p>You are also given value of a function, F(n) = Sum of squares&nbsp; of factor of n. (example F(20) = 546)</p>
<p>Now you have to calculate the value of x and y which satisfies the equation K1x + K2y = m. Where m is given. Since there are many roots you have to find a single pair (x,y) which satisfies the equation having minimum absolute value of (x +y). If no pair is possible output -1. Else output <strong>(abs(x+y)^m)%mod</strong></p>
<h3>Input</h3>
<p>First line contains T(1&lt;=T&lt;=10000) number of test cases. Each test case consist of single line containing 3 integers n, F(n) and m.&nbsp;</p>
<h3>Output</h3>
<p>Output &nbsp;T lines , each line contains a single integer ((x+y)^m)%mod.</p>
<h3>Constraints</h3>
<p>T&lt;=10000</p>
<p>N&lt;=10^8</p>
<p>F(n)&lt;=10^18</p>
<p>M&lt;=100</p>
<p>mod=10000000000283</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1</pre>
<pre>6 50 3

<strong>Output:</strong>
0 </pre>