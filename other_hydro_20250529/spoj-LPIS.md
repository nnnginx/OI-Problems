<p><span style="font-size: medium;">Dhrubo has a sequence of N integers. He is trying to find the longest perfect increasing subsequence of that sequence. But he is not very expert in finding longest perfect increasing subsequences. So he needs your help.</span></p>
<p><span style="font-size: medium;">&nbsp;A subsequence is a sequence that can be derived by another sequence by deleting elements without changing the order of the remaining elements. An increasing subsequence of a sequence is a subsequence where the elements are sorted in increasing order.</span></p>
<p><span style="font-size: medium;">Difference between an increasing subsequence and a perfect increasing subsequence is that in a perfect increasing subsequence the difference between any two consecutive elements is always 1.</span></p>
<p><span style="font-size: medium;">&nbsp;For example, let¡¯s consider a sequence S= {5, 2, 6, 3, 7, 8, 4}</span></p>
<p><span style="font-size: medium;">{5, 3, 4} is subsequence of sequence S but not an increasing subsequence.</span></p>
<p><span style="font-size: medium;">{5, 7, 8} is an increasing subsequence of sequence S, but not a perfect increasing subsequence.</span></p>
<p><span style="font-size: medium;">But {5, 6, 7, 8} is perfect increasing subsequence as the difference between any two consecutive elements is exactly 1.</span></p>
<p><span style="font-size: medium;">Note that, a single element will always be perfect increasing subsequence. So {5}, {2}, {7} are also perfect increasing subsequence of S.</span></p>
<p><strong><span style="text-decoration: underline;"><span style="font-size: medium;">INPUT:</span></span></strong></p>
<p><span style="font-size: medium;">First line of the input contains an integer N (1&lt;=N&lt;=10<sup>5</sup>) denoting the length of the sequence.</span></p>
<p><span style="font-size: medium;">Next line contains N integers separated by space which is the sequence.&nbsp; These integers will be greater than 0 and will not be greater than 10<sup>6</sup>.</span></p>
<p><strong><span style="text-decoration: underline;"><span style="font-size: medium;">OUTPUT:</span></span></strong></p>
<p><span style="font-size: medium;">A single integer in a line denoting the length of the longest perfect increasing subsequence.</span></p>
<p><strong><span style="text-decoration: underline;"><span style="font-size: medium;">Sample Input: #1</span></span></strong></p>
<p><span style="font-size: medium;">9</span></p>
<p><span style="font-size: medium;">5 1 5 6 2 3 8 7 4</span></p>
<p><span style="font-size: medium;">&nbsp;</span></p>
<p><strong><span style="text-decoration: underline;"><span style="font-size: medium;">Sample Output: #1</span></span></strong></p>
<p><span style="font-size: medium;">4</span></p>
<p><span style="font-size: medium;">&nbsp;</span></p>
<p><strong><span style="text-decoration: underline;"><span style="font-size: medium;">Sample Input: #2</span></span></strong></p>
<p><span style="font-size: medium;">8</span></p>
<p><span style="font-size: medium;">2 2 1 3 5 4 5 6</span></p>
<p><span style="font-size: medium;">&nbsp;</span></p>
<p><strong><span style="text-decoration: underline;"><span style="font-size: medium;">Sample Output: #2</span></span></strong></p>
<p><span style="font-size: medium;">5</span></p>
<p>&nbsp;</p>
<p>( set by : Nashir Ahmed )</p>