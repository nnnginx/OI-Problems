<p>在战前，蛐蛐国土地肥沃，农业发达，素有“沃野千里，天府之土”的美誉。农业是蛐蛐国的一大支柱产业。但在连年战乱后，蛐蛐国遭遇了严重水土流失，土质受到严重破坏，粮食和经济作物产量大大降低。振兴蛐蛐国农业，成为蛐蛐国的一大要务和难题。</p>
<p>伏特决定用跳蚤国的高新技术——金坷垃来解决这个难题。金坷垃是一种知名肥料，一袋能顶两袋撒，撒了小麦亩产一千八。即使面对蛐蛐国的恶劣土壤环境，金坷垃也可以极大提升作物产量。</p>
<p>但是金坷垃并不能单独使用，只能加入到一款其它的肥料中混合使用。同时金坷垃的作用有着极强的随机性：若一款原有的肥料肥力被量化为<strong>整数</strong> $x$ ，则将金坷垃掺入其中后，会带来一定的额外肥力，数值在 $[0,m]$ 间等概率随机，即，新的肥料肥力会变为 $[x,x+m]$ 之间的等概率随机<strong>实数</strong>，这里 $m$ 是一个给定的<strong>整数</strong>。</p>
<p>现在伏特想测试下金坷垃的性能，他从市面上买了 $n$ 款肥料，并将金坷垃分别掺入其中，不同肥料间掺入金坷垃后金坷垃带来的额外肥力互不相关。他希望你能告诉他，最终得到的肥料肥力中排序后第 $1\sim n$ 小的肥力期望值分别是多少。可以证明在题目的条件限制下，期望值是一个最简分数 $\frac{p}{q}$ ，且 $q$ 不是 $998244353$ 的倍数，你只需要输出 $p \cdot q^{-1} \bmod 998244353$ 的值即可。</p>
<h2>输入格式</h2>
<p>第一行两个正整数 $n,m$ ，分别表示肥料种类数和金坷垃的肥力上限。</p>
<p>接下来一行 $n$ 个正整数，第 $i$ 个正整数 $a_i$ 表示第 $i$ 款肥料的肥力。</p>
<h2>输出格式</h2>
<p>输出 $n$ 行，第 $i$ 行一个非负整数表示第 $i$ 小的肥力期望值对 $998244353$ 取模后的值。</p>


<pre><code class="language-input1">3 1
1 2 3
</code></pre>



<pre><code class="language-output1">499122178
499122179
499122180
</code></pre>



<p>三款肥料的肥力分别是 $a_1=1,a_2=2,a_3=3$ ，且 $m=1$ 。</p>
<p>容易发现不论金坷垃带来的额外肥力是多少，最终得到的三款肥料肥力 $b_i$ 仍然满足 $b_1\leq b_2\leq b_3$ 。因此第 $i$ 小肥料肥力期望值即为 $b_i$ 期望值 $\frac{3}{2},\frac{5}{2},\frac{7}{2}$ ，对 $998244353$ 取模后即得到样例输出。</p>


<pre><code class="language-input2">5 3
3 4 2 3 5
</code></pre>



<pre><code class="language-output2">505489582
791406484
246480092
249971894
702262855
</code></pre>


<h2>样例三</h2>
<p>见附加文件中 <code>ex_fertilizer3.in</code> 和 <code>ex_fertilizer3.out</code> 。</p>
<h2>样例四</h2>
<p>见附加文件中 <code>ex_fertilizer4.in</code> 和 <code>ex_fertilizer4.out</code> 。</p>
<h2>数据范围</h2>
<p>对于所有数据， $1\leq n\leq 2000,1\leq m,a_i\leq 10^8$ 。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n\leq$</th>
<th style="text-align:center;">特殊性质</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;" rowspan="2">$2000$</td>
<td style="text-align:center;">$\forall 1\leq i &lt; n,a_i+m\leq a_{i+1}$</td>
<td style="text-align:center;">$3$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$\forall 1\leq i &lt; n,a_i=a_{i+1}$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;" rowspan="5">无</td>
<td style="text-align:center;">$16$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$80$</td>
<td style="text-align:center;">$21$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$400$</td>
<td style="text-align:center;">$14$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$1500$</td>
<td style="text-align:center;">$23$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">$2000$</td>
<td style="text-align:center;">$8$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$4\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21013/file/attachment.zip">样例数据下载</a></p>
