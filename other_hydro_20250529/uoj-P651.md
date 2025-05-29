<p>对于一个用六边形无限平铺的平面，Pak Dengklek 站在其中一个格子上，并称该格子为初始格子。如果六边形平铺中的两个格子有公共边，则称它们是相邻的格子。对于一步移动，Pak Dengklek 可以从一个格子向六个可能的方向（从 $1$ 到 $6$ 编号，如下图所示）移动到与其相邻的格子上。</p>
<p><img src="https://img.uoj.ac/problem/651/651_hexagon_p1.png" alt="放图" class="img-responsive center-block"></p>
<p>于某个由 $N$ 次行动构成的行动序列，Pak Dengklek 可以用其产生的路径（对应一个按序访问的格子序列）构造一个领域。其中第 $i$ 次行动由移动方向 $D[i]$ 和在该方向上的移动步数 $L[i]$ 组成，并且该路径应有如下性质：</p>
<ul>
<li>路径是 封闭 的，这意味着在格子序列中，起点格子与终点格子（即初始格子）相同。</li>
<li>路径是 简单 的，这意味着在格子序列中，除了初始格子访问过恰好两次（起点和终点分别访问一 次），其他格子只能被访问至多一次。</li>
<li>路径是 暴露 的，这意味着在格子序列中，每个格子与至少一个不在序列中出现过的非 内部格子 相邻。<ul>
<li>如果一个格子不在格子序列中出现过，并且从它出发，在不经过格子序列中任何格子的情况下，（通过若干步移动） 只能访问到有限个格子，我们就称该格子是 内部格子 。</li>
</ul>
</li>
</ul>
<p>下图是一个符合上述条件的路径例子。其中：</p>
<ul>
<li>$1$ 号格子（粉色）是初始格子。</li>
<li>被编号的格子（淡蓝色）组成格子序列，编号代表它被访问的顺序。</li>
<li>被标上叉号的格子（深蓝色）是内部格子。</li>
</ul>
<p><img src="https://img.uoj.ac/problem/651/651_hexagon_p2.png" alt="放图" class="img-responsive center-block"></p>
<p>构造出的领域只包含所有路径上的格子和内部格子。领域中格子 $c$ 的距离定义为：在只经过领域中包含格子的情况下，从初始格子出发到达 $c$ 所需要的最少移动步数。领域中一个格子的分数定义为 $A+d \times B$，其中 $A$ 和 $B$ 是 Pak Dengklek 给定的常数，$d$ 是该格子在领域中的距离。下图给出了用上示路径构成的领域中每个格子的距离。</p>
<p><img src="https://img.uoj.ac/problem/651/651_hexagon_p3.png" alt="放图" class="img-responsive center-block"></p>
<p>请帮助 Pak Dengklek 计算，用给出的行动序列构成的领域中，所有格子的分数之和。由于总分数值可能很大，最终结果对 $10^9+7$ 取模。</p>
<h2>实现细节</h2>
<p>你需要实现下列函数：</p>
<pre><code class="sh_cpp">int draw_territory(int N, int A, int B, int[] D, int[] L)</code></pre>
<ul>
<li>$N$：行动序列中行动的次数。</li>
<li>$A,B$：分数计算中的常数。</li>
<li>$D$：大小为 $N$ 的数组，其中 $D[i]$ 表示第 $i$ 次行动的方向。</li>
<li>$L$：大小为 $N$ 的数组，其中 $L[i]$ 表示第 $i$ 次行动的移动步数。</li>
<li>函数应该返回用给出的行动序列所构成的领域中，所有格子的分数总和对 $10^9+7$ 取模后的值。</li>
<li>该函数将被调用恰好一次。</li>
</ul>
<h2>例子</h2>
<p>考虑下列调用：</p>
<pre>draw_territory(17, 2, 3,
               [1, 2, 3, 4, 5, 4, 3, 2, 1, 6, 2, 3, 4, 5, 6, 6, 1],
               [1, 2, 2, 1, 1, 1, 1, 2, 3, 2, 3, 1, 6, 3, 3, 2, 1])

</pre>

<p>该行动序列和上述题面中给出的例子相同。下表列出了该领域中所有可能的距离值所对应的分数。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th>距离值</th>
<th>格子数</th>
<th>每个格子分数</th>
<th>总分数</th>
</tr>
</thead>
<tbody>
<tr>
<td>$0 $</td>
<td>$1$</td>
<td>$2+0×3=2$</td>
<td>$1×2=2$</td>
</tr>
<tr>
<td>$1 $</td>
<td>$4$</td>
<td>$2+1×3=5$</td>
<td>$4×5=20$</td>
</tr>
<tr>
<td>$2 $</td>
<td>$5$</td>
<td>$2+2×3=8$</td>
<td>$5×8=40$</td>
</tr>
<tr>
<td>$3 $</td>
<td>$6$</td>
<td>$2+3×3=11$</td>
<td>$6×11=66$</td>
</tr>
<tr>
<td>$4 $</td>
<td>$4$</td>
<td>$2+4×3=14$</td>
<td>$4×14=56$</td>
</tr>
<tr>
<td>$5 $</td>
<td>$3$</td>
<td>$2+5×3=17$</td>
<td>$3×17=51$</td>
</tr>
<tr>
<td>$6 $</td>
<td>$4$</td>
<td>$2+6×3=20$</td>
<td>$4×20=80$</td>
</tr>
<tr>
<td>$7 $</td>
<td>$4$</td>
<td>$2+7×3=23$</td>
<td>$4×23=92$</td>
</tr>
<tr>
<td>$8 $</td>
<td>$5$</td>
<td>$2+8×3=26$</td>
<td>$5×26=130$</td>
</tr>
<tr>
<td>$9 $</td>
<td>$3$</td>
<td>$2+9×3=29$</td>
<td>$3×29=87$</td>
</tr>
<tr>
<td>$10$</td>
<td>$4$</td>
<td>$2+10×3=32$</td>
<td>$4×32=128$</td>
</tr>
<tr>
<td>$11$</td>
<td>$5$</td>
<td>$2+11×3=35$</td>
<td>$5×35=175$</td>
</tr>
<tr>
<td>$12$</td>
<td>$2$</td>
<td>$2+12×3=38$</td>
<td>$2×38=76$</td>
</tr>
</tbody>
</table>
</div>
<p>总分数值为 $2+20+40+66+56+51+80+92+130+87+128+175+76=1003$。</p>
<p>因此，<code>draw_territory</code> 应该返回 $1003$。</p>
<h2>输入格式</h2>
<p>示例测试程序将按以下格式读取输入数据：</p>
<ul>
<li>第 $1$ 行：$N, A, B$</li>
<li>第 $2 + i(0 \le i \le N-1)$ 行：$D[i], L[i]$</li>
</ul>
<h2>输出格式</h2>
<p>示例测试程序将按以下格式输出你的答案：
- 第 $1$ 行，<code>draw_territory</code> 的返回值。</p>
<h2>限制与约定</h2>
<ul>
<li>$3 \leq N \leq 200\ 000$</li>
<li>$0 \leq A,B \leq 10^9$</li>
<li>$1 \leq D[i] \leq 6(0 \leq i \leq N-1)$</li>
<li>$1 \leq L[i] (0 \leq i \leq N-1)$</li>
<li>$L$ 中的元素之和不超过 $10^9$。</li>
<li>给出的行动序列所对应的路径一定是 <em>封闭、简单</em> 和 <em>暴露</em> 的。</li>
</ul>
<p>子任务：</p>
<p><strong> 实际测试中，前 12 个 subtask 为数据包，后 8 个 subtask 为 8 个子任务。 </strong></p>
<ol>
<li>($3$ 分) $N=3,B=0$</li>
<li>($6$ 分) $N=3$</li>
<li>($11$ 分) $L$ 中的元素之和不超过 $2000$</li>
<li>($12$ 分) $B = 0,L$ 中的元素之和不超过 $200\ 000$</li>
<li>($15$ 分) $B = 0$</li>
<li>($19$ 分) $L$ 中的元素之和不超过 $200\ 000$</li>
<li>($18$ 分) $L[i] = L[i + 1] (0 \leq i \leq N-2)$</li>
<li>($16$ 分) 无附加限制</li>
</ol>
<p><strong>时间限制</strong>：$2\texttt{s}$</p>
<p><strong>空间限制</strong>：$1\texttt{GB}$</p>
<h2>下载</h2>
<p><a href="./21052/file/attachment.zip">样例数据下载</a></p>
