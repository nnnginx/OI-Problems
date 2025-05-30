<p>小U最近锅多如狗，因为有一堆的人要找他调代码。一共有$n$ 个人要找他办事 。他们做了一道国家集训队的一道神题<del>，要用到可持久化 Top cactus 等算法</del>，但是他们都没有把代码调出来。他们分别编号为 $1, 2, \ldots, n$，且编号从小到大排成一列。</p>
<p>小U想把他们按编号分成各批，然后<strong>从前往后（即编号从小到大）</strong>分批调代码。其中<strong>每一批人的编号是连续的一段</strong>。第 $i$ 个人调出代码需要 $t_i$ 个单位时间。而每一批蒟蒻需要把代码都调好，才能出来。也就是说，他们占用教室的时间为<strong>每个人调代码所需时间的最大值</strong>。</p>
<p>由于同学Gayfriends之间容易互相影响，每一批蒟蒻内编号最大的人，设编号为 $i$，不能与编号为 $l_i$ 的人在同一批，否则这一批的代码会调不出来。如果 $l_i = 0$，就意味着没有这个限制这位同学是个纯洁的好孩子。</p>
<p>而每位蒟蒻都会有不耐烦指数。第 $i$ 位蒟蒻每等待一个单位时间，他的不耐烦程度就会增加 $w_i$。等待时间指的是从他们排好队到这个蒟蒻进教室为止的这段时间，也就是排在他前面的每一批蒟蒻占用教室时间之和。</p>
<p>现在小U想让他们成功调出这道神题，并且不耐烦程度的和最小。可是他忙着帮助他们，就把这个任务交给了你。</p>
<h2>输入格式</h2>
<p>第一行一个正整数 $n$，表示人数。</p>
<p>接下来 $n$ 行每行三个非负整数 $l_i, t_i, w_i​$，意义如题面所述。</p>
<p>保证 $0 \leq l_i \lt i$。</p>
<h2>输出格式</h2>
<p>仅一行，表示$n$个人的最小不耐烦程度之和。</p>


<pre><code class="language-input1"><code>1
0 2426 8707</code>
</code></pre>

<pre><code class="language-output1"><code>0</code>
</code></pre>


<pre><code class="language-input2"><code>4
0 1929 401
1 7233 960
1 3564 9106
2 4746 182</code>
</code></pre>

<pre><code class="language-output2"><code>21084798</code>
</code></pre>
<h2>限制与约定</h2>
<p>本题有 5 个子任务。对于所有数据，有 $0 \leq t_i, w_i \leq 10^9$，且最终答案不大于 $10^{18}$。</p>
<p>Subtask 1 (9 pts): $1 \leq n \leq 10$；  </p>
<p>Subtask 2 (10 pts): $1 \leq n \leq 2\,000$；  </p>
<p>Subtask 3 (18 pts): $1 \leq n \leq 100\,000$ 且 $w_i$，$t_i$ 均为一定范围内等概率随机生成；  </p>
<p>Subtask 4 (12 pts): $1 \leq n \leq 100\,000$ 且 $t_i \leq t_{i+1}$；</p>
<p>Subtask 5 (51 pts): $1 \leq n \leq 100\,000$。</p>
<p><strong>时间限制：</strong>$3\mathtt{s}$</p>
<p><strong>空间限制：</strong>$512\mathtt{MB}$</p>
<h2>下载</h2>
<p><a href="./20835/file/attachment.zip">样例数据下载</a></p>
