<p>反攻正在进行中，按照套路，跳蚤国将会很快获得最终的胜利。跳蚤国的情报局也没闲下来，他们正打算派遣一批“菲克蚤”前往跳晚国窃取有关三星 note7 的资料。</p>
<p>Fake Yang 是这批“菲克蚤”的教练，他教会他们各种 Fake 的技术，以便更好混入敌方内部。共 $n$ 只菲克蚤，由 $1$ 到 $n$ 编号。Fake Yang 给每个菲克蚤都算了特征值 $a_1, \dots, a_n$，两个菲克蚤的相似度定义成这两个菲克蚤的特征值的差的绝对值，即第 $i$ 只菲克蚤与第 $j$ 只菲克蚤的相似度为 $\lvert a_i - a_j \rvert$。</p>
<p>现在这批菲克蚤排成一列在 Fake Yang 面前，Fake Yang 需要在其中选出一些菲克蚤合成一个行动小队。按照套路，他会选取连续一整段的菲克蚤 $a_l, a_{l + 1}, \dots, a_r$。很显然，这个行动小队越大越好，但是按照套路，小队内的跳蚤最好都各不相同，假如有两只跳蚤长得很像的话很可能会引起跳晚们的怀疑。为此 Fake Yang 将小队的相似度定义为小队中的跳蚤两两之间的最小的相似度，用 $s(l, r)$ 表示。</p>
<p>为保证安全，现在他想选取至少 $k$ 只跳蚤，且使得安全值最大。其中安全值定义如下：
\begin{equation}
s(l, r) \times (r - l)
\end{equation}</p>
<p>但是，他并不知道最优解是什么，于是按照套路你需要帮助他求得这个值。</p>
<h2>输入格式</h2>
<p>按照套路，第一行三个正整数 $n,m,k$。$k$ 的意义如前所述，$n$ 表示跳蚤的只数。</p>
<p>接下来一行 $n$ 个整数，按照套路依次表示 $n$ 只跳蚤的特征值 $a_1, \dots, a_n$，保证 $1 \le a_i \le m$。</p>
<h2>输出格式</h2>
<p>按照套路，一行一个整数，表示答案。</p>


<pre><code class="language-input1">10 10 2
1 4 2 6 1 9 6 8 10 3
</code></pre>


<pre><code class="language-output1">8
</code></pre>


<p>一种方案是选取区间 $[5, 6]$，相似度为 $8$，答案为$8 \times (6 - 5) = 8$。</p>
<h2>样例二</h2>
<p>按照套路，见样例数据下载。</p>
<h2>样例三</h2>
<p>按照套路，见样例数据下载。</p>
<h2>限制与约定</h2>
<p>由于一些原因，本题我们需要按照套路使用捆绑测试。每个子任务有若干个测试点，分为 $5$ 个子任务，你只有通过一个子任务的所有测试点才能按照套路得到这个子任务的分数。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>子任务</th>
<th>分值</th>
<th>$n$ 的规模</th>
<th>$m$ 的规模</th>
</tr></thead><tbody><tr><td>1</td><td>7</td><td>$n \le 100$</td><td rowspan="2">$m \le 50000$</td></tr><tr><td>2</td><td>13</td><td>$n \le 5000$</td></tr><tr><td>3</td><td>20</td><td rowspan="2">$n \le 50000$</td><td>$m \le 1000$</td></tr><tr><td>4</td><td>30</td><td>$m \le 50000$</td></tr><tr><td>5</td><td>30</td><td>$n \le 200000$</td><td>$m \le 200000$</td></tr></tbody></table></div>

<p>在所有数据中，满足 $2 \le n \le 200000$，$1 \le m \le 200000$，$2 \le k \le n$。</p>
<p><strong>时间限制：</strong>$2\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20686/file/attachment.zip">样例数据下载</a></p>
<h2>后记</h2>
<p>凭借着情报局的资料，跳蚤国很快研制出了高仿三星 note7，并加以改进，去掉了外面的手机外壳，暴露了其炸弹的本质，还在前端绑上了一个 Nokia1050，威力大增。</p>
<p>按照套路，失去了唯一优势的跳晚国很快败下阵来，跳蚤国获得最终的胜利！</p>
<p>然而谁都不曾思考过，为什么跳蚤大陆会出现这种新型科技——手机……</p>
