<p>给定整数 $n,y$ 和一个长度为 $n$ 的整数序列 $A = \{a_1,a_2,\cdots,a_n\}$，<strong>保证序列 $A$ 单调不减或单调不增</strong>。</p>
<p>构建有向图 $G(V,E)$，其中 $V = \{1,2,\cdots,n\}$，$E = \{(i,j) \mid 1 \leq i,j \leq n, a_i \geq j\}$。注意图 $G$ 中可能包含自环。</p>
<p>定义边子集 $T \subseteq E$ <strong>合法</strong>当且仅当图 $G'(V,T)$ 中每个点的入度和出度不超过 $1$，自环对对应点的入度和出度均贡献 $1$。定义一个合法边子集 $T$ 的<strong>权值</strong>为 $y^{\mathrm{cycle}(T)}$，其中 $\mathrm{cycle}(T)$ 表示图 $G'(V,T)$ 的环数，自环是一个环。</p>
<p>特别地，本题认为 $0^0=1$。</p>
<p>对于所有整数 $0 \leq k \leq n$，求所有大小为 $k$ 的合法边子集的权值和，对 $998244353$ 取模。</p>
<h2>输入格式</h2>
<p>第一行两个整数 $n,y$，第二行 $n$ 个整数 $a_1,a_2,\cdots,a_n$ 描述序列 $A$。</p>
<h2>输出格式</h2>
<p>一行 $n+1$ 个整数，第 $i$ 个整数表示大小为 $i-1$ 的合法边子集的权值和，对 $998244353$ 取模。</p>


<pre><code class="language-input1">2 2
2 2
</code></pre>


<pre><code class="language-output1">1 6 6
</code></pre>


<p>图 $G$ 中有两个点和边 $\{(1,1),(1,2),(2,1),(2,2)\}$。</p>
<p>大小为 $0$ 的合法边子集仅有空集，其权值为 $1$，故大小为 $0$ 的合法边子集的权值和为 $1$；</p>
<p>大小为 $1$ 的合法边子集有 $\{(1,1)\},\{(2,2)\},\{(1,2)\},\{(2,1)\}$，它们的权值分别为 $2,2,1,1$，权值和为 $6$；</p>
<p>大小为 $2$ 的合法边子集有 $\{(1,1),(2,2)\},\{(1,2),(2,1)\}$，它们的权值分别为 $4,2$，权值和为 $6$。</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，$1 \leq n \leq 10^5 , 0 \leq y &lt; 998244353 , 0 \leq a_i \leq n$。保证序列 $A$ 是单调不减或单调不增序列。</p>
<p>前 $5$ 个子任务满足序列 $A$ 单调不减，特殊性质与分值如下表所示。</p>
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>子任务编号</th><th>$n \leq $</th><th>特殊性质</th><th>分值</th></tr></thead><tbody><tr><td>$1$</td><td>$8$</td><td>无</td><td>$1$</td></tr><tr><td>$2$</td><td>$15$</td><td>$y=0$</td><td>$9$</td></tr><tr><td>$3$</td><td>$2000$</td><td>无</td><td>$10$</td></tr><tr><td>$4$</td><td>$75000$</td><td>$y=1$</td><td>$15$</td></tr><tr><td>$5$</td><td>$10^5$</td><td>无</td><td>$15$</td></tr></tbody></table><p>后 $4$ 个子任务满足序列 $A$ 单调不增，设 $b_i = \sum_{j=1}^n [a_j \geq i]$，特殊性质与分值如下表所示。</p>
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>子任务编号</th><th>$n \leq $</th><th>特殊性质</th><th>分值</th></tr></thead><tbody><tr><td>$6$</td><td>$15$</td><td>$y=0$</td><td>$5$</td></tr><tr><td>$7$</td><td>$2000$</td><td>无</td><td>$10$</td></tr><tr><td>$8$</td><td>$75000$</td><td>对于所有满足 $a_i \geq i$ 的 $i$，$a_i \geq b_i$</td><td>$15$</td></tr><tr><td>$9$</td><td>$10^5$</td><td>无</td><td>$20$</td></tr></tbody></table><p><strong>请注意算法常数对运行时间带来的影响。</strong></p>
<p><strong>时间限制：$\texttt{3s}$</strong></p>
<p><strong>空间限制：$\texttt{512MB}$</strong></p>
<h2>下载</h2>
<p><a href="https://uoj.ac/download.php?type=problem&amp;id=597">样例数据下载</a></p>
