<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/katex.min.css" integrity="sha384-wITovz90syo1dJWVh32uuETPVEtGigN07tkttEqPv+uR2SE/mbQcG7ATL28aI9H0" crossorigin="anonymous">
<script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/katex.min.js" integrity="sha384-/y1Nn9+QQAipbNQWU65krzJralCnuOasHncUFXGkdwntGeSvQicrYkiUBwsgUqc1" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/contrib/auto-render.min.js"></script>
<script>// <![CDATA[
document.addEventListener("DOMContentLoaded", function(){
  renderMathInElement(
    document.body,{
      delimiters: [
        {left: "$$", right: "$$", display: true},
        {left: "$", right: "$", display: false}]})});
// ]]></script>

<p></p>
<p>You are given an array of size $N$ containing the integers $1, 2, \ldots, N$ in some order.</p>
<p>A <em>move</em> consists of swapping the integers $k$ and $k+1$ for some $1 \le k \lt N$.  In other words, you may swap any pair of integers that has a difference of one.</p>
<p>Find the minimum number of moves required to sort the given array in ascending order.</p>
<h3>Input</h3>
<p>The first line contains $T$ ($1 \le T \le 1000$), the number of test cases.</p>
<p>Each test case contains $N$ ($2 \le N \le 10^5$) followed by $N$ distinct integers ($1 \le x_i \le N$).</p>
<p>The sum of $N$ over all test cases will not exceed $10^5$.</p>
<h3>Output</h3>
<p>For each test case, output the number of moves required to sort the array.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
2 1 2
2 2 1
3 3 2 1
4 4 2 3 1
6 2 1 4 3 6 5

<strong>Output:</strong>
0
1
3
5
3
</pre>
<h3>Note</h3>
<p>Below is one optimal sequence of moves that sorts [4,2,3,1].</p>
<ul>
<li>Swap 1 and 2: [4,<b>2</b>,3,<b>1</b>] ¡ú [4,<b>1</b>,3,<b>2</b>].</li>
<li>Swap 2 and 3: [4,1,<b>3</b>,<b>2</b>] ¡ú [4,1,<b>2</b>,<b>3</b>].</li>
<li>Swap 3 and 4: [<b>4</b>,1,2,<b>3</b>] ¡ú [<b>3</b>,1,2,<b>4</b>].</li>
<li>Swap 2 and 3: [<b>3</b>,1,<b>2</b>,4] ¡ú [<b>2</b>,1,<b>3</b>,4].</li>
<li>Swap 1 and 2: [<b>2</b>,<b>1</b>,3,4] ¡ú [<b>1</b>,<b>2</b>,3,4].</li>
</ul>