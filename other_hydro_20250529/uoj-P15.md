<p>石头剪刀布是常见的猜拳游戏:石头胜剪刀,剪刀胜布,布胜石头。如果两个人出拳一
样，则不分胜负。在《生活大爆炸》第二季第 8 集中出现了一种石头剪刀布的升级版游戏。</p>
<p>升级版游戏在传统的石头剪刀布游戏的基础上,增加了两个新手势:</p>
<p>斯波克:《星际迷航》主角之一。</p>
<p>蜥蜴人:《星际迷航》中的反面角色。</p>
<p>这五种手势的胜负关系如表一所示,表中列出的是<strong>甲对乙</strong>的游戏结果。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>甲\乙</th>
<th>剪刀</th>
<th>石头</th>
<th>布</th>
<th>蜥蜴人</th>
<th>斯波克</th>
</tr></thead><tbody><tr><td>剪刀</td><td>平</td><td>输</td><td>赢</td><td>赢</td><td>输</td></tr><tr><td>石头</td><td>×</td><td>平</td><td>输</td><td>赢</td><td>输</td></tr><tr><td>布</td><td>×</td><td>×</td><td>平</td><td>输</td><td>赢</td></tr><tr><td>蜥蜴人</td><td>×</td><td>×</td><td>×</td><td>平</td><td>赢</td></tr><tr><td>斯波克</td><td>×</td><td>×</td><td>×</td><td>×</td><td>平</td></tr></tbody></table></div>

<p>现在,小 A 和小 B 尝试玩这种升级版的猜拳游戏。已知他们的出拳都是有周期性规律的，但周期长度不一定相等。例如：如果小A以“石头-布-石头-剪刀-蜥蜴人-斯波克”长度为 $6$ 的周期出拳,那么他的出拳序列就是“石头-布-石头-剪刀-蜥蜴人-斯波克-石头-布-石头-剪刀-蜥蜴人-斯波克-......”,而如果小B以“剪刀-石头-布-斯波克-蜥蜴人”长度为 $5$ 的周期出拳,那么他出拳的序列就是“剪刀-石头-布-斯波克-蜥蜴人-剪刀-石头-布-斯波克-蜥蜴人-......”</p>
<p>已知小 A 和小 B 一共进行 $N$ 次猜拳。每一次赢的人得 $1$ 分，输的得 $0$ 分；平局两人都得 $0$ 分。现请你统计 $N$ 次猜拳结束之后两人的得分。</p>
<h2>输入格式</h2>
<p>第一行包含三个整数：$N,N_A,N_B$,分别表示共进行 $N$ 次猜拳、小 A 出拳的周期长度，小 B 出拳的周期长度。数与数之间以一个空格分隔。</p>
<p>第二行包含 $N_A$ 个整数,表示小 A 出拳的规律,第三行包含 $N_B$ 个整数,表示小 B 出拳的规律。其中，0 表示“剪刀”，1 表示“石头”，2 表示“布”，3 表示“蜥蜴人”，4 表示“斯波克”。数与数之间以一个空格分隔。</p>
<h2>输出格式</h2>
<p>输出一行，包含两个整数，以一个空格分隔，分别表示小 A、小 B 的得分。</p>


<pre><code class="language-input1">10 5 6
0 1 2 3 4
0 3 4 2 1 0
</code></pre>


<pre><code class="language-output1">6 2
</code></pre>



<pre><code class="language-input2">9 5 5
0 1 2 3 4
1 0 3 2 4
</code></pre>


<pre><code class="language-output2">4 4
</code></pre>

<h2>限制与约定</h2>
<p>$0 &lt; N \leq 200, 0 &lt; N_A \leq 200, 0 &lt; N_B \leq 200$</p>
<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>内存限制：</strong>$128\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20455/file/attachment.zip">样例数据下载</a></p>
