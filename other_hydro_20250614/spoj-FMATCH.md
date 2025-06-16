<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/FMATCH/en/">English</a></td> 
<td width="50%"><a href="/problems/FMATCH/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>FJ has N (1 ¡Ü N ¡Ü 50,000) cows and M (1 ¡Ü M ¡Ü 50,000) bulls. Given a list of P (1 ¡Ü P ¡Ü 150,000) potential matches between a cow and a bull, compute the greatest number of pairs that can be matched. Of course, a cow can be matched to at most one bull, and vice versa.</p>

<h3>Input</h3>
<p>The first line contains three integers, N, M, and P. Each of the next P lines contains two integers A (1 ¡Ü A ¡Ü N) and B (1 ¡Ü B ¡Ü M), denoting that cow A can be matched with bull B.</p>

<h3>Output</h3>
<p>Print a single integer that is the maximum number of pairs that can be obtained.</p>

<h3>Example</h3>

<pre><b>Input:</b>
5 4 6
5 2
1 2
4 3
3 1
2 2
4 4


<b>Output:</b>
3

</pre>

<p>Cow 1 can be matched to bull 2, cow 3 to bull 1, and cow 4 to bull 3.</p>

<p>Original problem: <a href="https://www.spoj.com/problems/MATCHING/">https://www.spoj.com/problems/MATCHING/</a>.</p>