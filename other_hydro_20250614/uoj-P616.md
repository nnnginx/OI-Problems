<p>Anna 和 Bruno 是考古学家。他们在挖掘 IOI 王国的遗迹。在遗迹 A 中，Anna 发现了一个古老机器的设计图。在遗迹 B 中，Bruno 发现了一台真实的机器。</p>
<p>这个机器包含 $N$ 个装置。装置排成一行连接到一根电线上。有三种类型的装置分别为 $X$、$Y$ 和 $Z$。从左边开始，每个装置的编号依次为 $0$ 至 $N-1$。装置 $i$ （$0\leq i\leq N-1$）的类型为 $S_i$，即 $S_i$ 为 $X$、$Y$ 或 $Z$ 之一。</p>
<p>因为机器太大，Bruno 决定一个一个从机器中移除装置。然而因为装置之间互相通过电线连接，他必须非常小心移除时的顺序。</p>
<p>考虑一种从机器中将装置移除的方法，我们有如下定义：</p>
<ul>
<li>假设装置 $x,y,z$ （$0\leq x\lt y\lt z\leq N-1$）还没有被移除，且 $S_x=X$，$S_y=Y$，$S_z=Z$。此外，假设对于每个 $x\lt j\lt y$，装置 $j$ 已被移除，且对于每个 $y\lt k\lt z$，装置 $k$ 也已被移除。如果所有这些条件都满足且我们将装置 $y$ 从机器中移除，那么这被称为一个<strong>好的移除</strong>。</li>
<li>任何其他将装置从机器中移除的方法都不是好的移除。</li>
</ul>
<p>Bruno 需要将所有 $N$ 个装置从机器中移除且<strong>好的移除</strong>的次数最大。然而，因为三种类型的装置看起来很相似，他不能分辨装置的类型。</p>
<p>而因为 Anna 有机器的设计图，她知道附在机器上的装置的类型。因此她可以通过无线电发射器来帮助 Bruno。通过无线电发射器，她能够传送一个序列，该序列中的每个字符都是 $0$ 或 $1$。</p>
<p>写一个程序来实现 Anna 的规划和 Bruno 的规划使得<strong>好的移除</strong>的次数最大。在该任务中 Anna 传送给 Bruno 的字符越短你的得分越高。</p>
<h2>实现细节</h2>
<p>你需要提交两个文件。</p>
<p>第一个文件为 <code>Anna.cpp</code>。需要实现 Anna 的规划。具体的，它需要实现以下函数且程序需要使用 <code>#include</code> 包含 <code>Anna.h</code> 头文件。</p>
<ul>
<li><code>void Anna(int N, std::vector&lt;char&gt; S)</code> 对于每个测试用例，这个函数会在开始时被调用恰好一次。<ul>
<li>参数 <code>N</code> 为装置的数量 $N$。</li>
<li>参数 <code>S</code> 为一个 $N$ 长数组。这意味着 <code>S[i]</code> 为装置 $i$（$0\leq i\leq N-1$）的类型 $S_i$。因此字符 <code>S[i]</code> 为 <code>X</code>、<code>Y</code> 或 <code>Z</code> 之一。</li>
</ul>
</li>
</ul>
<p>你的程序可以调用以下函数：</p>
<ul>
<li><code>void Send(int a)</code> 使用该函数，Anna 将传送一个字符 $0$ 或 $1$ 给 Bruno。<ul>
<li>参数 <code>a</code> 为传给 Bruno 的信息。它应该为 $0$ 或 $1$。如果不满足该条件，你的程序将会被判断为 <strong>Wrong Answer [1]</strong>。</li>
<li>该函数 <code>Send</code> 不应被调用超过 $200000$ 次，否则你的程序将会被判断为 <strong>Wrong Answer [2]</strong>。</li>
</ul>
</li>
</ul>
<hr>
<p>第二个文件是 <code>Bruno.cpp</code>。需要实现 Bruno 的规划。它需要包含以下函数且该程序需要使用 <code>#include</code> 包含 <code>Bruno.h</code> 头文件。</p>
<ul>
<li><code>void Bruno(int N, int L, std::vector&lt;int&gt; A)</code> 在函数 <code>Anna</code> 被调用后，该函数会被调用一次。<ul>
<li>参数 <code>N</code> 为装置的数量 $N$。</li>
<li>参数 <code>L</code> 为 Anna 发送的字符（$0$ 或 $1$）的数量。</li>
<li>参数 <code>A</code> 为一个 $L$ 长数组。它意味着 Anna 发送了一个序列 <code>A[0],A[1],...,A[L-1]</code> 以这样的顺序给 Bruno。序列中的每个字符为 $0$ 或 $1$。</li>
</ul>
</li>
</ul>
<p>你的程序可以调用以下函数：</p>
<ul>
<li><code>void Remove(int d)</code> 你的程序调用该函数来回答如何移除装置。<ul>
<li>参数 <code>d</code> 为装置的索引。意味着 Bruno 移除了装置 $d$。</li>
<li>必须满足 $0\leq d\leq N-1$，否则你的程序将会被判断为 <strong>Wrong Answer [3]</strong>。</li>
<li>不允许使用相同的参数 $d$ 来调用该函数超过一次，否则你的程序将会被判断为 <strong>Wrong Answer [4]</strong>。</li>
<li>函数 <code>Remove</code> 需要被调用恰好 $N$ 次。当函数 <code>Bruno</code> 终止时，如果调用 <code>Remove</code> 的次数不为 $N$ 次，你的程序将会被判断为 <strong>Wrong Answer [5]</strong>。</li>
<li>在所有 $N$ 个装置被移除后，好的移除的次数需要为可能的最大值，否则你的程序将会被判断为 <strong>Wrong Answer [6]</strong>。</li>
</ul>
</li>
</ul>
<h2>注意事项</h2>
<ul>
<li>你的程序可以实现其他的函数来内部使用，或者使用全局变量。提交的文件将会被与 grader 一起编译成一个可执行文件。所有全局变量和内部函数应该在一个匿名的命名空间内声明来避免与其他文件的冲突。它将被作为两个进程执行，分别为 Anna 和 Bruno。Anna 的进程和 Bruno 的进程间无法共享全局变量。</li>
<li>你的程序不允许使用标准输入输出，也不能与其他文件通过任何方式交互。但是你的程序可以通过标准错误流来输出 debug 信息。</li>
</ul>
<p>你可以在这里（可能需要补一个链接）下载一个包含样例 grader 的存档文件来测试你的程序。存档文件也包含了一个你的程序的样例。</p>
<p>样例 grader 为 <code>grader.cpp</code> 文件。为了测试你的程序，将 <code>grader.cpp</code>、<code>Anna.cpp</code>、<code>Bruno.cpp</code>、<code>Anna.h</code>、<code>Bruno.h</code> 放在同一个目录下并使用下列编译命令</p>
<p><code>g++ -std=gnu++17 -O2 -fsigned-char -o grader grader.cpp Anna.cpp Bruno.cpp</code></p>
<p>当编译成功时会生成可执行文件 <code>grader</code>。</p>
<p>注意实际的 grader 与样例 grader 不同。样例 grader 将会使用单进程且从标准输入读入数据并将结果写到标准输出。</p>
<p>实际测试中，您的程序会被运行两次，两次的时间限制均为 $2$ 秒。</p>
<h2>输入格式</h2>
<p>样例 grader 从标准输入读入以下数据：</p>
<p>$N$</p>
<p>$S_0\space S_1\space \cdots \space S_{N-1}$</p>
<p>这里 $S_i$ 与 $S_{i+1}$（$0\leq i\leq N-2$）之间使用一个空格分隔。</p>
<h2>输出格式</h2>
<p>当程序成功停止时，样例 grader 会在标准输出写入下列信息。</p>
<ul>
<li>如果你的答案被判定为 Wrong Answer [1]、[2]、[3]、[4]、[5] 之一，它会输出类型如 <code>Wrong Answer [1]</code>。</li>
<li>否则它会输出 <code>Send</code> 函数被调用的次数 $L$ 和好的移除的次数 $D$ 如 <code>Accepted: L D</code>。注意样例 grader 与实际 grader 不同，样例 grader 不会检查你的程序是否被判定为 Wrong Answer [6]。</li>
</ul>
<p>如果你的程序被判定为 Wrong Answer [1]、[2]、[3]、[4]、[5] 之中的多种类型，样例 grader 将只会报告其中一个。</p>
<h2>样例交互</h2>
<p>这里是一个输入的样例和样例 grader 与对应的函数调用。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th>Sample Input 1</th>
<th>Sample Function Calls</th>
<th>Sample Function Calls</th>
</tr>
</thead>
<tbody>
<tr>
<td>$ $</td>
<td>Call</td>
<td>Call</td>
</tr>
<tr>
<td><code>4 X Y X Z</code></td>
<td><code>Anna(4, {X, Y, X, Z})</code></td>
<td>$ $</td>
</tr>
<tr>
<td>$ $</td>
<td>$ $</td>
<td><code>Send(0)</code></td>
</tr>
<tr>
<td>$ $</td>
<td>$ $</td>
<td><code>Send(1)</code></td>
</tr>
<tr>
<td>$ $</td>
<td><code>Bruno(4, 2, {0, 1})</code></td>
<td>$ $</td>
</tr>
<tr>
<td>$ $</td>
<td>$ $</td>
<td><code>Remove(2)</code></td>
</tr>
<tr>
<td>$ $</td>
<td>$ $</td>
<td><code>Remove(1)</code></td>
</tr>
<tr>
<td>$ $</td>
<td>$ $</td>
<td><code>Remove(0)</code></td>
</tr>
<tr>
<td>$ $</td>
<td>$ $</td>
<td><code>Remove(3)</code></td>
</tr>
</tbody>
</table>
</div>
<p>在样例的函数调用中，四个装置将被以如下方式移除。</p>
<ol>
<li>在开始时，四个装置为 <code>X Y X Z</code>。</li>
<li>Bruno 移除了装置 2（注意这里为索引，而非第二个）。剩余的装置变为 <code>X Y - Z</code>。这里 <code>-</code> 意味着原先在这个位置的装置已被移除。</li>
<li>Bruno 移除了装置 1。剩余的装置变为 <code>X - - Z</code>。因为 $(x,y,z)=(0,1,3)$ 满足条件，这次是好的移除。</li>
<li>Bruno 移除了装置 0。剩余的装置变为 <code>- - - Z</code>。</li>
<li>最后 Bruno 移除了装置 3.剩余的装置变为 <code>- - - -</code>。</li>
</ol>
<p>好的移除的次数为一次，在这个样例中，好的移除的次数不可能大于一。</p>
<h2>限制与约定</h2>
<ul>
<li>$3\leq N\leq 100000$。</li>
<li><p>$S_i$ 为 <code>X</code>、<code>Y</code> 或 <code>Z</code> 之一（$0\leq i\leq N-1$）。</p>
</li>
<li><p>（5 分）$N\leq 18$。</p>
</li>
<li>（95 分）无额外约束。在该子任务中，你的分数将会使用以下方式计算。<ul>
<li>令 $L$ 为该子任务中每个测试用例中调用 <code>Send</code> 函数的次数的最大值，你的分数将按照下面方法计算：<ul>
<li>当 $160000\lt L\leq 200000$ 时，你的分数为 $\displaystyle 25+\left\lfloor 10\times \frac{200000-L}{40000}\right\rfloor$ 分。</li>
<li>当 $100000\lt L\leq 160000$ 时，你的分数为 $\displaystyle 35+\left\lfloor 30\times \frac{160000-L}{60000}\right\rfloor$ 分。</li>
<li>当 $70000\lt L\leq 100000$ 时，你的分数为 $\displaystyle 65+\left\lfloor 30\times \left(\frac{100000-L}{30000}\right)^2\right\rfloor$ 分。</li>
<li>当 $L\leq 70000$ 时，你的分数为 95 分。</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>这里 $\lfloor x\rfloor$ 为不超过 $x$ 的最大整数。</p>
<p><strong>时间限制</strong>：$2\texttt{s}$</p>
<p><strong>空间限制</strong>：$256\texttt{MB}$</p>
