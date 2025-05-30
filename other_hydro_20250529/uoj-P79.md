<p>从前一个和谐的班级，所有人都是搞OI的。有 $n$ 个是男生，有 $0$ 个是女生。男生编号分别为 $1, \dots, n$。</p>
<p>现在老师想把他们分成若干个两人小组写动态仙人掌，一个人负责搬砖另一个人负责吐槽。每个人至多属于一个小组。</p>
<p>有若干个这样的条件：第 $v$ 个男生和第 $u$ 个男生愿意组成小组。</p>
<p>请问这个班级里最多产生多少个小组？</p>
<h2>输入格式</h2>
<p>第一行两个正整数，$n, m$。保证 $n \geq 2$。</p>
<p>接下来 $m$ 行，每行两个整数 $v, u$ 表示第 $v$ 个男生和第 $u$ 个男生愿意组成小组。保证 $1 \leq v, u \leq n$，保证 $v \neq u$，保证同一个条件不会出现两次。</p>
<h2>输出格式</h2>
<p>第一行一个整数，表示最多产生多少个小组。</p>
<p>接下来一行 $n$ 个整数，描述一组最优方案。第 $v$ 个整数表示 $v$ 号男生所在小组的另一个男生的编号。如果 $v$ 号男生没有小组请输出 $0$。</p>


<pre><code class="language-input1">10 20
9 2
7 6
10 8
3 9
1 10
7 1
10 9
8 6
8 2
8 1
3 1
7 5
4 7
5 9
7 8
10 4
9 1
4 8
6 3
2 5
</code></pre>


<pre><code class="language-output1">5
9 5 6 10 2 3 8 7 1 4
</code></pre>



<pre><code class="language-input2">5 4
1 5
4 2
2 1
4 3
</code></pre>


<pre><code class="language-output2">2
2 1 4 3 0
</code></pre>

<h2>限制与约定</h2>
<p>$1 \leq n \leq 500$，$1 \leq m \leq 124750$。</p>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20519/file/attachment.zip">样例数据下载</a></p>
