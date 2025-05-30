<p>这是一道模板题。</p>
<p><del>（这个题现在标程挂了。。哪位哥哥愿意提供一下靠谱的标程呀？）</del> <del>现在的新标程有没有问题啊？</del> 现在的新标程有没有问题啊？</p>
<p><strong>已将所有ex tests的t改成1。现在的checker会先判解是否合法，再判和标准答案的误差。如果发现有std优的合法解，请联系管理员。</strong></p>
<p>本题中你需要求解一个标准型线性规划：</p>
<p>有 $n$ 个实数变量 $x_1,x_2,\dots,x_n$ 和 $m$ 条约束，其中第 $i$ 条约束形如 $\sum_{j=1}^n a_{ij}x_j \le b_i$。</p>
<p>此外这 $n$ 个变量需要满足非负性限制，即 $x_j\ge 0$。</p>
<p>在满足上述所有条件的情况下，你需要指定每个变量 $x_j$ 的取值，使得目标函数 $F=\sum_{j=1}^n c_j x_j$ 的值最大。</p>
<h2>输入格式</h2>
<p>第一行三个正整数 $n,m,t$。其中 $t \in \{0,1\}$。</p>
<p>第二行有 $n$ 个整数 $c_1,c_2,\cdots,c_n$，整数间均用一个空格分隔。</p>
<p>接下来 $m$ 行，每行代表一条约束，其中第 $i$ 行有 $n+1$ 个整数 $a_{i1},a_{i2},\cdots,a_{in}, b_i$，整数间均用一个空格分隔。</p>
<h2>输出格式</h2>
<p>如果不存在满足所有约束的解，仅输出一行 "<samp>Infeasible</samp>"。</p>
<p>如果对于任意的 $M$，都存在一组解使得目标函数的值大于 $M$，仅输出一行"<samp>Unbounded</samp>"。</p>
<p>否则，第一行输出一个实数，表示目标函数的最大值 $F$。当第一行与标准答案的相对误差或绝对误差不超过 $10^{-6}$，你的答案被判为正确。</p>
<p>如果 $t=1$，那么你还需要输出第二行，用空格隔开的 $n$ 个非负实数，表示此时 $x_1,x_2,\dots,x_n$ 的取值，如有多组方案请任意输出其中一个。</p>
<p>判断第二行是否合法时，我们首先检验 $F-\sum_{j=1}^n c_j x_j$ 是否为 $0$，再对于所有 $i$，检验 $\min\{ 0,b_i-\sum_{j=1}^n a_{ij}x_j \}$ 是否为 $0$。检验时我们会将其中大于 $0$ 的项和不大于 $0$ 的项的绝对值分别相加得到 $S_+$ 和 $S_-$，如果 $S_+$ 和 $S_-$ 的相对误差或绝对误差不超过 $10^{-6}$，则判为正确。</p>
<p>如果 $t=0$，或者出现 <samp>Infeasible</samp> 或 <samp>Unbounded</samp> 时，不需要输出第二行。</p>


<pre><code class="language-input1">2 2 1
1 1
2 1 6
-1 2 3
</code></pre>


<pre><code class="language-output1">4.2
1.8 2.4
</code></pre>


<p>两条约束分别为 $2x_1+x_2\le 6,-x_1+2x_2\le 3$。</p>
<p>当 $x_1=1.8,x_2=2.4$ 时目标函数 $x_1+x_2$ 取到最大值 $4.2$。</p>


<pre><code class="language-input2">2 2 1
1 -1
1 1 4
-1 -2 -2
</code></pre>


<pre><code class="language-output2">4.0
4.0 0.0
</code></pre>


<p>注意 $x_j\ge 0$ 的限制。</p>


<pre><code class="language-input3">3 3 1
0 0 1
-2 1 0 -4
1 1 0 4
1 -2 0 -4
</code></pre>


<pre><code class="language-output3">Infeasible
</code></pre>



<pre><code class="language-input4">2 1 1
0 1
1 0 1
</code></pre>


<pre><code class="language-output4">Unbounded
</code></pre>

<h2>限制与约定</h2>
<p>对于所有数据，$1\leq n,m \leq 20$，$0 \leq |a_{ij}|,|b_i|,|c_j|\leq 100$，$t \in \{0,1\}$。</p>
<p>本题包含 4 个子任务，每个 25 分。</p>
<p>子任务 1,3 满足 $b_i\ge 0$。</p>
<p>子任务 2,4 没有特殊限制。</p>
<p>子任务 1,2 中 $t=0$。</p>
<p>子任务 3,4 中 $t=1$。</p>
<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20619/file/attachment.zip">样例数据下载</a></p>
