<h3>Problem</h3>
<p align="justify">
Suppose you are given a 2<sup>a</sup>x2<sup>b</sup> array. It is stored sequentially in memory in the usual way, first values in the first row, then values in the second one and so on. You would like to transpose it, but you don't have any additional memory. The only operation that you can perform is swapping contents of two memory cells. What is the minimal number of such operations required for transpostion?
</p>
<h3>Input</h3>
<p align="justify">
The first line of input contains the number of test cases c (1&lt;=c&lt;=100). Each test case consists of two integers a,b (0&lt;=a+b&lt;=500000).
</p>
<h3>Output</h3>
<p align="justify">
For each test case output the minimal number of swaps required to transpose an 2<sup>a</sup>x2<sup>b</sup> array. As it can be quite large, you have to output its remainder when divided by 1000003 (yes, it's a prime number :).
</p>
<h3>Example</h3>
<pre>Input:
3
1 1
2 2
5 7

Output:
1
6
3744

</pre>