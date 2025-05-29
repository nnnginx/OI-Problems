<p>Given an array of n integers and a number x. Your task is very simple. You have to find the subarray (length&gt;0) whose xor is maximum with x. lets say the subarray as maxsubarray.You have to print the xor value of maxsubarray.</p>
<h3>Input</h3>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">first line of input consists of t test cases</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">second line of input contains two integers n and x.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">third line contains n space separated integers denoting the elements of array</div>
<p>first line of input consists of t test cases</p>
<p>second line of input contains two integers n and x.</p>
<p>third line contains n space separated integers denoting the elements of array</p>
<h3>Output</h3>
<p>first and only line of output is Xor value of maxsubarray.</p>
<h3>Constraints</h3>
<p>1&lt;=t&lt;=10</p>
<p>1&lt;=n&lt;=200000</p>
<p>1&lt;=x&lt;=2*10^9</p>
<p>1&lt;=arr[i]&lt;=2*10^9 where arr[i] is any integer of array</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
3 7
1 2 3

<strong>Output:</strong>
0</pre>
<pre>taking 1^2^3 is 0 when taken xor with 7 gives us the maxmimum xor value.</pre>