<p>为了让无法联网的跳蚤也能使用“跳找”发现新世界，你计划推动“跳找”搜索引擎接入卫星通信。</p>
<p>跳蚤王国共拥有 $n$ 颗通信卫星，每颗卫星的覆盖区域都是一个三角形。</p>
<p>若卫星 $R$ 的覆盖区域严格包含点 $p$，则称 $p$ 能连接 $R$，称点 $p$ 能连接的卫星集合为 $T_p$。</p>
<p>现在跳蚤国打算建立<strong>两处</strong>基站，设为点 $p_1,p_2$。若其满足 $T_{p_1} \cup T_{p_2}=S$，则能联系到到所有卫星，称这种建设方案为“完整的”。</p>
<p>第 $i$ 颗卫星的性能恰为第 $i$ <strong>弱</strong>，称一个卫星集合 $T$ 中性能最好的的卫星为“主星”。</p>
<p>你要求出有哪些卫星可能在“完整的”基站建设方案中成为某个基站的“主星”，以方便咨询管理调度事宜。</p>
<p>即：对于每颗通信卫星 $S_i$，判定是否存在“完整的”基站建设方案 $p_1,p_2$，使得 $S_i$ 是 $T_{p_1}$ 或 $T_{p_2}$ 的“主星”。</p>
<h2>输入格式</h2>
<p>第一行一个整数 $n$，表示卫星的个数。</p>
<p>后 $n$ 行，每行六个整数 $x_1,y_1,x_2,y_2,x_3,y_3$。</p>
<p>描述一个顶点分别为 $(x_1,y_1),(x_2,y_2),(x_3,y_3)$ 的三角形，即为第 $i$ 个卫星的覆盖区域。</p>
<h2>输出格式</h2>
<p>输出一行长度为 $n$ 的 0/1 串，其中第 $i$ 个字符为 $1$ 表示第 $i$ 个卫星可能作为“主星”，反之为 $0$。</p>


<pre><code class="language-input1">4
2 9 2 5 6 5
2 6 2 2 5 3
4 1 4 6 7 1
1 1 1 5 5 1
</code></pre>


<pre><code class="language-output1">0111
</code></pre>


<p>可构成答案的两种“完整的”基站建设方案如图。</p>
<p><img src="https://img.uoj.ac/problem/579/tri.png" alt="样例一" class="img-responsive center-block"></p>
<p>图中橙色点表示方案中包含的基站。紫色圈中的是“主星”。</p>


<pre><code class="language-input2">5
1 1 1 6 2 1
1 1 1 5 3 1
1 1 1 4 4 1
1 1 1 3 5 1
1 1 1 2 6 1
</code></pre>


<pre><code class="language-output2">11111
</code></pre>



<pre><code class="language-input3">16
44 82 17 23 48 13 
21 26 31 53 73 46 
37 4 59 44 24 84 
4 27 10 91 76 3 
73 53 58 62 11 20 
7 11 94 8 13 94 
93 41 10 20 81 19 
4 42 52 92 52 33 
12 92 59 14 24 55 
37 6 95 68 1 43 
30 28 92 4 27 59 
26 7 82 34 15 23 
47 98 26 23 70 50 
5 100 3 8 95 65 
14 26 82 41 2 62 
82 31 7 30 55 65
</code></pre>


<pre><code class="language-output3">0000000000010101
</code></pre>

<h2>限制与约定</h2>
<p>对于所有数据，$1\leq n\leq 550,1\leq x_1,y_1,x_2,y_2,x_3,y_3\leq 10^5$ 且均为<strong>整数</strong>。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n\leq$</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">1</td>
<td style="text-align:center;">$16$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">2</td>
<td style="text-align:center;">$50$</td>
<td style="text-align:center;">$25$</td>
</tr>
<tr>
<td style="text-align:center;">3</td>
<td style="text-align:center;">$160$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">4</td>
<td style="text-align:center;">$550$</td>
<td style="text-align:center;">$40$</td>
</tr>
</tbody>
</table>
</div>
<p>为了防止卡精度，保证将所有卫星覆盖区域的顶点任意移动不超过 $10^{-3}$ 单位后答案不变。</p>
<p><strong>时间限制</strong>：$6\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20983/file/attachment.zip">样例数据下载</a></p>
