<p>The problem is simple.</p>
<p>Find &nbsp;<strong>(a^b) % MOD</strong></p>
<p>where ,</p>
<p>a = Nth <strong>non-fibonacci</strong> number</p>
<p>b = (Nth <strong>fibonacci</strong> number)%MOD</p>
<p>MOD = 10^9+7</p>
<p>Consider fibonacci series as 1,1,2,3,....</p>
<p><strong>Note :</strong> It is guaranteed that Nth non-fibonacci number will always be less than MOD value for every value of N used.</p>
<h3>Input</h3>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">First line contains T , the number of test cases</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Each next T lines contains a &nbsp;number N.</div>
<p>First line contains <strong>T</strong> , the number of test cases.</p>
<p>Each next T lines contains a &nbsp;number <strong>N</strong>.</p>
<h3>Output</h3>
<p>Print T lines of output where each line corresponds to the required answer.&nbsp;</p>
<p><strong>Announcement: </strong>Constraints are updated. Sorry for inconvenience occurred.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>3
3
2
1</pre>
<pre><strong>Output:</strong></pre>
<pre>49
6
4
</pre>
<pre><strong>Explanation</strong></pre>
<pre>For N=3 : 3rd non fibo number =7, 3rd fibo number=2. ans= (7^2) %MOD =49</pre>
<pre>For N=2 : 2nd non fibo number =6, 2nd fibo number=1. ans=(6^1) %MOD=6</pre>
<pre>For N=1 : 1st non fibo number =4, 1st fibo number=1.  ans= (4^1) %MOD =4</pre>
<pre><strong>Constraints</strong></pre>
<pre>1&lt;=T&lt;=100000</pre>
<pre><strong>1&lt;=N&lt;=9*10^8</strong></pre>
<pre><strong>Note: Test cases have been updated and costraints are changed.  Those who get TLE or WA are suggested to resubmit. GOOD LUCK there.</strong></pre>