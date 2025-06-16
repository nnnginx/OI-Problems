<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Alice and Bob are participating in an exciting new Olympic event, the Team Slide Treasure Hunt Race! This event takes place on a slide with various treasures on it, which is up to 10m wide and 10km long. Yes, that's kilometers.</p>
<p>The slide can be represented as a grid of cells, with $N$ ($2 \leq N \leq 10^4$) rows and $M$ ($2 \leq M \leq 10$) columns. The rows are numbered $1, 2, \ldots, N$ from top to bottom, and the columns are numbered $1, 2, \ldots, M$ from left to right. The cell in row $i$ and column $j$ is referred to as cell ($i$, $j$), and contains a treasure with value $G_{i,j}$ ($1 \le G_{i,j} \le 10^5$).</p>
<p>The two friends will each get to travel once down the slide, one after another. First, Alice will slide from the top-left corner of the slide (cell ($1$, $1$)) down to the bottom-left corner (cell ($N$, $1$)). Then, Bob will slide from the top-right corner (cell ($1$, $M$)) down to the bottom-right corner (cell ($N$, $M$)). Whenever a person moves in the slide, they move from their current row to the next row down, and they can also guide themselves left or right by one column if desired. This means that they can go from cell ($i$, $j$) to either cell ($i+1$, $j-1$), ($i+1$, $j$), or ($i+1$, $j+1$), as long as they don't exit the slide. Throughout the race, both Alice and Bob collect the treasure in each cell they slide through - this includes their respective starting and ending cells. However, if Bob goes through any cell that Alice has already visited, he can't collect the treasure in it again.</p>
<p>Alice and Bob would like to determine a sliding plan to allow them to collect as much treasure as possible, and win the gold medal! They've asked you to determine the maximum total value of treasure that they can collect, out of all valid strategies.</p>
<h3>Input</h3>
<p>The first line of the input will contain two integers $N$ and $M$, separated by a space. Each of the next $N$ lines, for $i$ from $1$ to $N$, will contain the $M$ space-separated integers $G_{i,1} \,\,\, G_{i,2} \,\,\, \dots \,\,\, G_{i,M}$.</p>
<h3>Output</h3>
<p>Output one number on a line by itself: the maximum combined treasure value that Alice and Bob can collect.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">5 4<br>3 6 8 2<br>5 2 4 3<br>1 1 20 10<br>1 1 20 10<br>1 1 20 10</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">73</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The single optimal sliding plan involves Alice sliding down-right, down-right, down-left, and down-left, followed by Bob sliding down-left, down-right, down-left, and down-right. The treasures collected are shown in bold on the following grid:</p>
<p style="text-align: center;"><img src="../../../content/sourspinach:slide.bmp" alt=""></p>
<p>Alice collects a total treasure value of $3+2+20+1+1=27$, while Bob collects $2+4+10+20+10=46$. Their total is then $27+46=73$.</p>