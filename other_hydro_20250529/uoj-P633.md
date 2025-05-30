<p>在第三个游戏中赢下了小 L 后，跳跳将军放你离开了跳跳堡。</p>
<p>而在长时间围困跳跳堡后，跳蚤国王指挥部队发动了总攻。双方交战异常激烈，最终你立下了大功，利用潜入跳跳堡时得到的地图发现了突破口——一座无人防守的小门，于是潮水般的跳蚤和蛐蛐涌进了小门，跳蚤蛐蛐联军终于成功收复了跳跳堡，恢复了跳蚤国。</p>
<p>在庆功宴上，跳蚤乐队奏响了新谱的歌曲《你将如闪电般归来》，跳蚤国王心情大好，给在场的宾客们出了一个题，只要能做出这个题就可以获得他的大赏：</p>
<p>给定一棵节点被染有红色或绿色的有标号有根树，我们称之为“闪电树”当且仅当：</p>
<ol>
<li>每个节点 $i$ 的父亲编号 $p_i$ 比 $i$ 小，即 $p_i &lt; i$；</li>
<li>这棵树的每一层恰有一个红色节点；</li>
<li>对于任意一个节点，如果它不是根节点，那么它的父亲一定是红色；</li>
<li>任意一个红色节点的绿色孩子数量均为偶数个。</li>
</ol>
<p>“可以推出，闪电树中红色的节点形成了一条从根节点往下连到某个叶子节点的红色路径，就像一条红色的闪电，划开前方的艰难险阻……” 跳蚤国王形象地描述道。</p>
<p>给定 $k, n$，问节点数为 $n$ 层数为 $k$ 的闪电树的数量对 $998244353$ 取模的值。</p>
<p>这道题非常难，在场的其他宾客绞尽脑汁也不知道怎么完成，但你——伏特是一名计算机高手，发现这个题目可以用计算机轻松解决。只要解决了它，大赏就是你的了！</p>
<h2>输入格式</h2>
<p>一行两个正整数 $k,n$，表示树的层数和结点数。</p>
<h2>输出格式</h2>
<p>一行一个整数表示答案对 $998244353$ 取模的值。</p>


<pre><code class="language-input1">2 10
</code></pre>


<pre><code class="language-output1">9
</code></pre>


<p>容易发现树的形态一定只能是 $p_2=p_3=\ldots=p_{10}=1$，即第一层为节点 $1$，第二层为节点 $2\sim 10$。</p>
<p>而对于树的颜色，显然节点 $1$ 只能是红色，节点 $2\sim 10$ 中恰好有一个是红色，其余是绿色，因此共有 $9$ 种方案。</p>


<pre><code class="language-input2">3 7
</code></pre>


<pre><code class="language-output2">65
</code></pre>



<pre><code class="language-input3">8 14
</code></pre>


<pre><code class="language-output3">703179
</code></pre>



<pre><code class="language-input4">529 1453
</code></pre>


<pre><code class="language-output4">159030840
</code></pre>



<pre><code class="language-input5">1453 14530529
</code></pre>


<pre><code class="language-output5">443513052
</code></pre>



<pre><code class="language-input6">10 1000000000000000000
</code></pre>


<pre><code class="language-output6">384797525
</code></pre>

<h2>数据范围</h2>
<p>对于所有数据，$1\le k\le 10^7$，$k\le n\le 10^{18}$，$k\equiv n \pmod 2$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$k\le$</th>
<th style="text-align:center;">$n\le$</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;" rowspan="4">$n$</td>
<td style="text-align:center;">$100$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$3\times 10^3$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$10^5$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$10^7$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;" rowspan="4">$10^{18}$</td>
<td style="text-align:center;">$5$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$100$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">$10^3$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">$10^7$</td>
<td style="text-align:center;">$15$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$2\texttt{s}$</p>
<p><strong>空间限制</strong>：$1\texttt{GB}$</p>
<h2>下载</h2>
<p><a href="./21034/file/attachment.zip">样例数据下载</a></p>
