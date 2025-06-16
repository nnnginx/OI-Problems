<p>跳蚤国王在地图中为你选出了一片 $n\times n$ 的方形荒漠，这里坐落着一座太阳能发电站，这将会作为“跳找”实验室的专用能源。</p>
<p>为了保证能源供给稳定，防止机房断电惨案，你被委派为发电站对接和监测工作的负责人。</p>
<p>你本以为只需要在数字化控制中心逛一逛就能完成任务，驾车来到电站之后，才发现问题有本质的不同。</p>
<p>电站年久失修，不仅控制系统无迹可寻，旧的线路也已经全部湮没于黄沙之中。幸运地是，所有光伏元件仍然保持完好——现在，要重新排布和连接这些光伏元件使其恢复运转。</p>
<p>给出 $n\times n$ 的 0/1 矩阵 $A$，其中 $A_{i, j}=1$ 表示位置 $(i,j)$ 有光伏元件，而 $0$ 表示没有元件。</p>
<p>受新的布线方案的限制，对光伏元件的分布有下列要求：</p>
<p>设第 $i$ 行的元件个数为 $c_{0,i}$ ，第 $i$ 列的元件个数为 $c_{1,i}$。</p>
<p>对于每个 $i$ ,给出 $dl_i, dr_i, k_i$ ,要求 $\left\lvert c_{0,i}-c_{1,i} \right\rvert \leq k$ 且 $c_{0,i}, c_{1,i} \in\left[dl_i,dr_i\right]$。即：要求第 $i$ 行和第 $i$ 列的元件个数在 $\left[dl_i, dr_i\right]$ 之间，且相差不超过 $k_i$。</p>
<p>给出 $n\times n$ 的矩阵 $C$，以 $C_{i, j}$ 表示<strong>改变</strong>位置 $(i,j)$ 上元件有/无状态的代价；特别地，若 $C_{i, j} = -1$，则表示 $(i,j)$ 位置的状态不可改变。</p>
<p>你深知：干活的进度一目了然，咕掉的空洞深不见底，而 deadline 总是比想象中近。于是，你计划尽快找到一组光伏元件的排布方案，在满足要求的前提下，使得总费用最小。</p>
<p>数据保证至少存在一组解。</p>
<h2>输入格式</h2>
<p>第一行一个正整数 $n$ 表示矩阵的大小。</p>
<p>下面 $n$ 行，每行 $n$ 个整数 $A_{i, j}$ 表示 0/1 矩阵 $A$。</p>
<p>下面 $n$ 行，每行 $n$ 个整数 $C_{i, j}$ 表示矩阵 $C$。</p>
<p>下面 $n$ 行，每行 $3$ 个整数 $dl_i, dr_i, k_i$。</p>
<h2>输出格式</h2>
<p>输出一行一个整数，表示最小所需的费用。</p>
<p>下面 $n$ 行，每行 $n$ 个数，描述 0/1 矩阵 $R$。第 $i$ 行第 $j$ 列的数表示 $R_{i, j}$。</p>
<p>矩阵 $R$ 即为你给出的对光伏元件分布方案。</p>
<p>如有多种方案，请输出任意一种即可。</p>


<pre><code class="language-input1">4
0 1 0 0
1 1 0 0
1 0 1 0
1 0 1 1
171 -1 445 270
665 464 1204 885
-1 515 1156 893
636 455 1189 890
1 2 1
2 4 1
1 3 1
1 3 0
</code></pre>


<pre><code class="language-output1">906
0 1 0 1
1 1 0 0
1 0 1 0
0 0 1 1
</code></pre>

<h2>样例二</h2>
<p>见下载文件中的 <code>ex_elec2.in</code> 与 <code>ex_elec2.out</code>。</p>
<p>该样例输入文件满足 $C_{i, j} \leq 0$。</p>
<h2>样例三</h2>
<p>见下载文件中的 <code>ex_elec3.in</code> 与 <code>ex_elec3.out</code>。</p>
<p>该样例输入文件满足 $k_i = 0$。</p>
<h2>样例四</h2>
<p>见下载文件中的 <code>ex_elec4.in</code> 与 <code>ex_elec4.out</code>。</p>
<p>该样例没有特殊性质。</p>
<h2>限制与约定</h2>
<p>对于所有的数据, $1\leq n\leq 100,\ 0\leq dl_i\leq dr_i\leq n,\ 0 \leq k_i \leq n,\ C_{i,j} \geq -1,\ \sum \lvert C_{i, j} \rvert \leq 2\times 10^9$。</p>
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr><th>子任务编号</th><th>$n \leq$</th><th>特殊性质</th><th>分值</th></tr>
</thead>
<tbody>
<tr><td> $1$ </td><td> $4$ </td> <td> 无 </td><td>$20$</td> </tr>
<tr><td> $2$ </td><td rowspan="4"> $50$ </td> <td> $C_{i, j} \leq 0, k_i = 0$ </td> <td>$10$</td> </tr>
<tr><td> $3$ </td><td> $C_{i, j} \leq 0$ </td> <td>$10$</td></tr>
<tr><td> $4$ </td><td> $k_i = 0$ </td> <td>$10$</td></tr>
<tr><td> $5$ </td><td> 无 </td> <td>$10$</td></tr>
<tr><td> $6$ </td><td rowspan="3"> $100$ </td><td> $C_{i, j} \leq 0$ </td> <td>$10$</td></tr>
<tr><td> $7$ </td><td> $k_i = 0$ </td> <td>$10$</td></tr>
<tr><td> $8$ </td><td> 无 </td> <td> $20$ </td> </tr>
</tbody>
</table>

<p>特殊性质一栏留空表示没有特殊性质。</p>
<p><strong>时间限制</strong>：$6\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20979/file/attachment.zip">样例数据下载</a></p>
