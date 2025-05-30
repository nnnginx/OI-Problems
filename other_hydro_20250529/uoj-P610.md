<p>Bitaro 将要参加一场特技飞行比赛。在这场比赛中，他将会驾驶一架飞机。这架飞机将会保持一个确定的海拔高度，并从上空经过检查点。<br>我们不妨假定这架飞机飞过的区域是一个平面直角坐标系。其中有 $N$ 个检查点，以 $1$ 到 $N$ 编号。第 $i$（$1 \le i \le N$）个检查点的坐标为 $(X_i, Y_i)$。</p>
<p>在比赛的过程中，他的飞机必须恰好经过每个检查点一次。具体地，他必须以以下方式飞行：</p>
<ol>
<li><p>首先，Bitaro 选择一个检查点作为起点，并且从这个检查点开始飞行。</p>
</li>
<li><p>重复以下过程 $N-1$ 次：<br>  Bitaro 在所有还没有被选择过的检查点中选择一个检查点作为下一个目标，然后从当前检查点直线飞行到这个检查点。</p>
</li>
<li><p>当飞机到达最后一个检查点时，此次飞行结束。</p>
</li>
</ol>
<p>在第 $2$ 步中，我们认为起点是已经被选择过的。他的飞机必须以直线从一个检查点飞到下一个检查点。虽然这是特技飞行，但是他被禁止在途中画弧线或转弯。</p>
<p>显然，他的飞行路线是一条折线。在飞行的过程中，他的飞机最多会更改 $N-2$ 次他的飞行方向。如果折线中以某个检查点为顶点的角非常小，那么 Bitaro 将会大幅度改换他的飞行方向；并且由于 Bitaro 技艺不精，这很可能会发生事故导致比赛被淘汰。</p>
<p>因此，Bitaro 希望最大化他的折线中最小角（除去起点和终点）的角度。</p>
<p>给定检查点的坐标，请您寻找一个经过检查点的排列顺序使得折线中最小角最大。</p>
<h2>输入格式</h2>
<p>第一行两个整数 $N, Z_0$。其中 $Z_0$ 是一个供评分器使用的参数。  </p>
<p>接下来 $N$ 行，每行两个整数 $X_i,Y_i$。</p>
<h2>输出格式</h2>
<p>输出包含 $N$ 行。其中第 $k$（$1 \le k \le N$）行包含一个整数 $P_k$（$1 \le P_k \le N$），即您给出的路线中第 $k$ 个检查点的编号。这里，起点即为 $P_1$。</p>
<h2>限制与约定</h2>
<p>对于所有的数据，满足</p>
<ul>
<li><p>$3 \le N \le 1\,000$。  </p>
</li>
<li><p>$\sqrt{X_i^2+Y_i^2} \le 10\,000\,000\ (1 \le i \le N)$。</p>
</li>
<li><p>$(X_i,Y_i) \ne (X_j,Y_j)\ (1 \le i &lt; j \le N)$。</p>
</li>
<li><p>$1 \le Z_0 \le 179$。</p>
</li>
</ul>
<h2>库</h2>
<p>在这道题中，你可以调用一个库，它包含计算三个点确定的角的角度的函数。这个库在压缩包中的 $\texttt{aerobatics.h}$ 文件中。调用规范如下：</p>
<ul>
<li>$\texttt{double GetAngle(int xa, int ya, int xb, int yb, int xc, int yc)}$<br>这个函数计算 $\angle BAC$ 的角度。它返回一个实数，保证误差足够小。<br><strong>注意确保参数的顺序正确。</strong><ul>
<li>关于点 $A$，参数 $\texttt{xa}$ 是 $A$ 的 $x$ 坐标，参数 $\texttt{ya}$ 是 $A$ 的 $y$ 坐标。</li>
<li>关于点 $B$，参数 $\texttt{xb}$ 是 $B$ 的 $x$ 坐标，参数 $\texttt{yb}$ 是 $B$ 的 $y$ 坐标。</li>
<li>关于点 $C$，参数 $\texttt{xc}$ 是 $C$ 的 $x$ 坐标，参数 $\texttt{yc}$ 是 $C$ 的 $y$ 坐标。</li>
<li>如果 $A,B$ 或 $A,C$ 的坐标相等，那么将会得到不可预料的结果。</li>
</ul>
</li>
</ul>
<p>在你的程序中，你可以使用该库中的 $\texttt{GetAngle}$。当然，你也可以修改这个函数。<br>不过评分器同样也使用库中的 $\texttt{GetAngle}$ 函数。</p>


<pre><code class="language-input1">7 90
3 1
2 5
0 2
-1 6
-3 1
-1 -4
4 -2
</code></pre>


<pre><code class="language-output1">5
3
1
7
6
4
2
</code></pre>



<h2>限制与约定</h2>
<p>对于每个输出文件，您的分数将以以下方式计算。<br>如果您的输出是错误的，您的分数为 $0$。例如，如果您给出的序列 $P_1,P_2,\dots,P_N$ 不是 $1,2,\dots,N$ 的排列或您的输出格式有误，您将会悲惨地得到 $0$ 分。<br>如果您的输出是正确的，则令 $Z$ 为折线中的最小角，您的分数将以以下公式计算：</p>
<ul>
<li><p>若 $Z \ge Z_0$，您的分数为 $S$。</p>
</li>
<li><p>若 $Z &lt; Z_0$，您的分数为 $S \times \dfrac{f(Z/180)}{f(Z_0/180)}$。</p>
</li>
</ul>
<p>其中函数 $f(\alpha)$（$0 \le \alpha \le 1$）定义为</p>
<p>$$ f(\alpha) = 4\alpha^4 + \alpha $$</p>
<p>您此题的分数为您在 $6$ 个输入文件得到的分数之和，四舍五入到最近的整数。</p>
<p>对于每组输入数据，$N,Z_0$ 的值及分数如下表：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">输入文件名</th>
<th style="text-align:center;">$N$</th>
<th style="text-align:center;">$Z_0$</th>
<th style="text-align:center;">分数</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$\texttt{input_01.txt}$</td>
<td style="text-align:center;">$15$</td>
<td style="text-align:center;">$100$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$\texttt{input_02.txt}$</td>
<td style="text-align:center;">$200$</td>
<td style="text-align:center;">$143$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$\texttt{input_03.txt}$</td>
<td style="text-align:center;">$200$</td>
<td style="text-align:center;">$134$</td>
<td style="text-align:center;">$15 $</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$\texttt{input_04.txt}$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">$156$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$\texttt{input_05.txt}$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">$150$</td>
<td style="text-align:center;">$20 $</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$\texttt{input_06.txt}$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">$153$</td>
<td style="text-align:center;">$20$</td>
</tr>
</tbody>
</table>
</div>
<h2>下载</h2>
<p><a href="./21014/file/attachment.zip">样例数据下载</a></p>
