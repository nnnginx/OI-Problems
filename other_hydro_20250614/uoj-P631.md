<p>为了恢复跳蚤国，跳蚤国王需要一支强大的军队，但他现在只是一个光杆司令。于是他来到了国富民强的蛐蛐国，希望能得到蛐蛐国王的支援。跳蚤国王向蛐蛐国王说明了来意。蛐蛐国王稍作思考，表示：“我们可以提供援军，但是需要先经过我的一个考验。”</p>
<p>蛐蛐国王的手下的禁卫军有 $\mathrm{limitn}$ 名士兵，士兵们在一个 $(10^9+1)\times (10^9+1)$ 的巨大网格上的格点处。每个格点的坐标可用数对 $(x,y)$ 表示，其中 $0 \le x \le 10^9$, $0 \le y \le 10^9$。任意时刻不能有两名士兵处在同一个位置。</p>
<p>对于一名士兵，如果与他所在位置 x 坐标相同的人数<strong>严格多于</strong>与他所在位置 y 坐标相同的人数，那么他就被编入第一组，否则被编入第二组。</p>
<p>一个调度过程是这样的。一开始你可以任意指定这 $\mathrm{limitn}$ 名士兵的位置，只要保证这些位置互不相同且在网格中。这时候每名士兵自动会被分入其中某一组。现在你可以指挥这些士兵进行至多 $\mathrm{limitm}$ 次移动，每次移动可以是将 x 坐标为 $a$ 的所有士兵的 x 坐标改为 $b$，或是将 y 坐标为 $a$ 的所有士兵 y 坐标改为 $b$。但每次移动后仍然要保证不能有两名士兵处在同一位置，且所有士兵位置仍在网格中。</p>
<p>显然，在每次移动后，有一部分（可能一个也没有）士兵所在的分组会改变。假设调度过程中共有 $m\leq \mathrm{limitm}$ 次移动，令第 $i$ 次移动后改变了分组的士兵个数为 $a_i$，则一个移动方式的总评价为 $S=\sum\limits_{i=1}^{m} a_i$。蛐蛐国王认为在调度过程中，最终得到的评价值 $S$ 越大说明指挥官能力越强。</p>
<p>现在蛐蛐国王的考验是：跳蚤国王需要证明他的指挥能力不比蛐蛐国王手下的将官差。于是他需要给出一个调度过程，使得最终得到的评价值 $S\geq \mathrm{minS}$，其中 $\mathrm{minS}$ 是蛐蛐国王手下给出的调度过程所得到的评价值。</p>
<p>跳蚤国王非常愤怒，觉得这个考验是在侮辱他的能力。但由于现在他是光杆司令，需要蛐蛐国的援助，因此他让作为计算机高手的你——伏特来帮他完成考验。</p>
<p>你设计的调度过程可以不用到全部 $\mathrm{limitn}$ 名士兵，即，你可以设定一个 $n\leq \mathrm{limitn}$ 作为士兵数量。</p>
<h2>输入格式</h2>
<p>一行三个正整数 $\mathrm{limitn},\mathrm{limitm}, \mathrm{minS}$，表示最大士兵数，最大移动次数和你要达到的最低评价值。</p>
<h2>输出格式</h2>
<p>第一行一个非负整数 $0\leq n\leq \mathrm{limitn}$ 表示你设计的调度过程中的士兵数。</p>
<p>接下来 $n$ 行，第 $i$ 行两个非负整数 $x_i,y_i$ 表示初始时第 $i$ 个士兵在 $(x_i,y_i)$ 位置，需要满足 $0 \leq x_i,y_i \leq 10^9$ 且 $(x_i,y_i)$ 互不相同。</p>
<p>接下来一行一个非负整数 $0\leq m\leq \mathrm{limitm}$ 表示你设计的调度过程中的移动次数。</p>
<p>接下来 $m$ 行每行三个非负整数 $\mathrm{type},a,b$，需要满足 $\mathrm{type} \in \{0,1\},0 \leq a,b \leq 10^9$，其中 $\mathrm{type}=0$ 表示将 x 坐标为 $a$ 的所有士兵 x 坐标改为 $b$，$\mathrm{type}=1$ 表示将 y 坐标为 $a$ 的所有士兵 y 坐标改为 $b$，注意每次移动后不能有两名士兵处在同一位置。</p>


<pre><code class="language-input1">4 3 4
</code></pre>


<pre><code class="language-output1">4
0 0
1 1
2 2
3 3
3
0 0 1
1 2 1
1 0 3
</code></pre>


<p>这组样例 $\mathrm{limitn}=4,\mathrm{limitm}=3,\mathrm{minS}=4$，你选择了 $n=\mathrm{limitn}=4,m=\mathrm{limitm}=3$。</p>
<p>初始时，$4$ 名士兵分别在 $(0,0),(1,1),(2,2),(3,3)$ 位置，分组为 $(2,2,2,2)$。</p>
<p>第一次移动后，第 $1$ 名士兵移动到了 $(1,0)$，前两名士兵分组改变，现在分组为 $(1,1,2,2)$。</p>
<p>第二次移动后，第 $3$ 名士兵移动到了 $(2,1)$，第 $2$ 名士兵分组改变，现在分组为 $(1,2,2,2)$。</p>
<p>第三次移动后，第 $1$ 名士兵移动到了 $(1,3)$，第 $1$ 名士兵分组改变，现在分组为 $(2,2,2,2)$。</p>
<p>共改变 $S=2+1+1=4$ 次，满足 $S\geq \mathrm{minS}$，因此这是一个合法的调度过程。</p>
<p>注意这并不是在 $\mathrm{limitn}=4, \mathrm{limitm}=3$ 下 $S$ 最大的方案。 </p>
<h2>样例二</h2>
<p>见附加文件中 <code>ex_dispatch2.in</code>，这组样例限制与子任务 $1$ 相同，输出不下发但依然可以提交测试。</p>
<h2>数据范围</h2>
<p>本题是一道<strong>传统题</strong>，你需要提交一个输出方案的程序。</p>
<p>本题共有 $4$ 个子任务，每个子任务有且仅有一个测试点，且 $\mathrm{limitn},\mathrm{limitm},\mathrm{minS}$ 均按下表给定。对于一个子任务，只有你的输出合法，并且满足 $S\geq \mathrm{minS}$，你才能获得该子任务的分数。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$\mathrm{limitn}=$</th>
<th>$\mathrm{limitm}=$</th>
<th style="text-align:center;">$\mathrm{minS}=$</th>
<th>分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$10^3$</td>
<td>$10^3$</td>
<td style="text-align:center;">$10^3$</td>
<td>$40$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;" rowspan="3">$10^5$</td>
<td>$300$</td>
<td style="text-align:center;">$94500$</td>
<td>$20$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$5\times 10^4$</td>
<td>$13600000$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$10^5$</td>
<td>$21100000$</td>
<td style="text-align:center;">$20$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>校验器</h2>
<p>为了方便选手测试，附加文件中我们给出了名为 <code>checker.cpp</code> 的文件，选手可以编译该程序，并使用它校验自己的输出文件。但请注意它与最终评测时所使用的校验器并不完全一致，<strong>且它的效率可能不足够高</strong>。你也不需要关心其代码的具体内容。</p>
<p>编译命令为：<code>g++ -std=c++11 checker.cpp −o checker</code>。此外，附加文件中有还有名为 <code>testlib.h</code> 的文件，在编译时，请确保该文件与 <code>checker.cpp</code> 在同一子目录下。</p>
<p>在终端中，<code>checker</code> 的使用方式为：<code>checker &lt;输入文件名&gt; &lt;输出文件名&gt; &lt;输出文件名&gt;</code>。如果你的输入文件名为 <code>dispatch.in</code>，输出文件名为 <code>dispatch.out</code>，则正确的使用方式为 <code>checker dispatch.in dispatch.out dispatch.out</code>。</p>
<p>若你的方案正确，校验器会给出 <code>ok</code> 并输出你的调度过程的评价值，否则，该校验器会给出简要的错误信息。</p>
<h2>下载</h2>
<p><a href="./21032/file/attachment.zip">附加文件下载</a></p>
