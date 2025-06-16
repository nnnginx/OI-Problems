<p>Divisiblity by 3 rule is pretty simple rule: Given a number sum the&nbsp;digits of number and check if sum is divisible by 3.If divisible then it is&nbsp;divisible by 3 else not divisible.Seems pretty simple but what if we want to extend this rule in binary&nbsp;representation!! </p>
<p>Given a binary representation we can again find if it is&nbsp;divisible by 3 or not.&nbsp;Making it little bit interesting what if only length of binary&nbsp;representation of a number is given say n.</p>
<p>Now can we find how many numbers&nbsp;exist in decimal form (base 10) such that when converted into binary (base 2) form has n&nbsp;length and is divisible by 3 ?? (1 &lt;= n &lt; 2*10^18)</p>

<h3>Input</h3>
<p>Length of binary form: n</p>

<h3>Output</h3>
<p>Print in new line the answer modulo 1000000007.</p>

<h3>Example</h3>
<h4>Input</h4>
<pre>1
2</pre>

<h4>Output</h4>
<pre>1
2</pre>

<p><strong>Explanation: </strong>For n=2 there are only 2 numbers divisible by 3 viz.0 (00) and 3 (11) and having length 2 in binary form.</p>
<p><strong>NOTE: </strong>There are multiple testfiles containing many testcases each so read till EOF.</p>
<p><strong>Warnings: </strong>Leading zeros are allowed in binary representation and slower languages might require fast i/o. Take care.</p>