<p>你有没有听说过奇异物品公司(Just Odd Inventions, Ltd.)?这家物品以生产奇异物品闻名，我们在题目中称之为 JOI 公司。</p>
<p>JOI 公司举办了一个新年晚会。员工正在巨大的烤盘上烤制 $N$ 块汉堡肉。烤盘大小为$10^9 \times 10^9$，方便起见，我们称左起第$x$列，下起第$y$行的格子为$(x,y)$。</p>
<p>汉堡肉从$1$至$N$编号，第$i$块汉堡肉被看成是左下角为$(L_i,D_i)$，右上角为$(R_i,U_i)$的一块矩形。汉堡肉可能相交。</p>
<p>你是JOI公司的一名新员工，你的任务是选择烤盘上的$K$个位置，并且在每个位置上插入一根竹签。这样你就可以判断每个被插入竹签的汉堡肉有没有熟。一个位置可以插入多个竹签。</p>
<p>形式化的，你需要找到一个$K$元组$(x_1,y_1),\cdots,(x_K,y_K)$满足如下条件：</p>
<ul><li>对于所有$1 \le i \le N$,存在$1 \le j \le K$同时满足$L_i \le x_j \le R_i,D_i \le y_j \le U_i$。</li>
<li>对于所有$1 \le j \le K$，满足$1 \le x_j,y_j \le 10^9$。</li>
</ul><p>数据保证有解。</p>
<h2>输入格式</h2>
<p>第一行两个空格分隔的整数 $N,K$。</p>
<p>接下来 $N$ 行每行四个整数 $L_i,D_i,R_i,U_i$，描述一块汉堡肉。</p>
<h2>输出格式</h2>
<p>$K$ 行，一行两个数字$x_i,y_i$，表示一根竹签。</p>
<p>若有多解，输出任意一组即可。</p>


<pre><code class="language-input1"><code class="sh_plain">4 2
2 1 3 3 
1 2 4 3 
6 1 7 4
5 3 7 5</code>
</code></pre>

<pre><code class="language-output1"><code class="sh_plain">2 2
7 4</code>
</code></pre>

<p>$(2,2)$处的竹签可以确定汉堡肉 $1,2$ 是否熟了。</p>
<p>$(7,4)$处的竹签可以确定汉堡肉 $3,4$ 是否熟了。</p>
<p>注意$(3,3),(6,4)$也是一组合法解。</p>


<pre><code class="language-input2"><code class="sh_plain">3 3
1 1 1 1
1 2 1 2
1 3 1 3</code>
</code></pre>

<pre><code class="language-output2"><code class="sh_plain">1 1
1 2
1 3</code>
</code></pre>
<h2>数据范围</h2>
<p>子任务1($1$分):$N \le 2000,K=1$</p>
<p>子任务2($1$分):$N \le 2000,K=2$</p>
<p>子任务3($3$分):$N \le 2000,K=3$</p>
<p>子任务4($6$分):$N \le 2000,K=4$</p>
<p>子任务5($1$分):$K=1$</p>
<p>子任务6($3$分):$K=2$</p>
<p>子任务7($6$分):$K=3$</p>
<p>子任务8($79$分):$K=4$</p>
<p>对于所有测试数据，满足$1 \le N \le 200000,1 \le K \le 4,1 \le L_i \le R_i \le 10^9,1 \le D_i \le U_i \le 10^9$。</p>
<p>时间限制:$\texttt{4S}$</p>
<p>空间限制:$\texttt{1GB}$</p>
<p><strong>如果std挂了请私信zyy。</strong></p>
