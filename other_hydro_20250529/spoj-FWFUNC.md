<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/FWFUNC/en/">English</a></td> 
<td width="50%"><a href="/problems/FWFUNC/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>Multiplicative functions are defined as functions such that f(m*n) = f(m) * f(n). Now, we put an extra constraint on multiplicative functions that if m and n are coprime , then f(m) and f(n) are also coprime. Additionally it is also provided that f(1)=1. f(x) is defined for positive integers and it returns positive integers.</p>
<p>
Now, you are provided with some x and corresponding f(x). Your task is to find out , if you can uniquely determine the value of f(y) given y and if yes, find the value. 
</p>

<h3>Input</h3>
<p>The first line of input contains a number representing the number of test cases. For each test case, the first line contains a number N representing the number of (x,f(x)) pairs to be provided. N Lines follow, each line containing a pair of space separated numbers : the first one corresponding to x and second one to f(x). Next line contains q, the number of queries. q lines follow, each containing a number y.</p>

<h3>Output</h3>
<p>For each test case output q lines, one corresponding to each query. The output should contain "YES f(y)" where f(y) is replaced by the integer denoting f(y) with no leading zeroes if given the data, we can uniquely determine f(y), or "NO" if the input data is inconsistent with the properties of the function or with the given information provided about the function, we can not uniquely determine f(y).</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
3
2 2
3 2
7 19
1
7
1
6 6
1
6
2
2 2
3 3
1
12

<b>Output:</b>
NO
YES 6
YES 12
</pre>

<h3>Constraints</h3>
<p>Dataset 1: The number of test cases are less than 20. N ¡Ü=50. x and f(x) ¡Ü 10^50 . x and f(x) do not have a prime factor greater than 100005.</p>
<p>The number of queries are less than or equal to 50. Each number in the query is less than 10^50. You are guaranteed that if the answer is unique, it contains less than 400 digits. Time limit: 12s</p>