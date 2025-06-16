<p>从前一个和谐的班级，有 $n_l$ 个是男生，有 $n_r$ 个是女生。编号分别为 $1, \dots, n_l$ 和 $1, \dots, n_r$。</p>
<p>有若干个这样的条件：第 $v$ 个男生和第 $u$ 个女生愿意结为配偶，且结为配偶后幸福程度为 $w$。</p>
<p>请问这个班级里幸福程度之和最大是多少？</p>
<h2>输入格式</h2>
<p>第一行三个正整数，$n_l, n_r, m$。</p>
<p>接下来 $m$ 行，每行三个整数 $v, u, w$ 表示第 $v$ 个男生和第 $u$ 个女生愿意结为配偶，且幸福程度为 $w$。保证 $1 \leq v \leq n_l$，$1 \leq u \leq n_r$，保证同一对 $v, u$ 不会出现两次。</p>
<h2>输出格式</h2>
<p>第一行一个整数，表示幸福程度之和的最大值。</p>
<p>接下来一行 $n_l$ 个整数，描述一组最优方案。第 $v$ 个整数表示 $v$ 号男生的配偶的编号。如果 $v$ 号男生没配偶请输出 $0$。</p>


<pre><code class="language-input1">2 2 3
1 1 100
1 2 1
2 1 1
</code></pre>


<pre><code class="language-output1">100
1 0
</code></pre>

<h2>限制与约定</h2>
<p>$1 \leq n_l, n_r \leq 400$，$1 \leq m \leq 160000$，$1 \leq w  \leq 10^9$。</p>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20520/file/attachment.zip">样例数据下载</a></p>
