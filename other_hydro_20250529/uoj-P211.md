<p>经过推理，人们终于找到那些投通过的异端，然而，投通过的人数远远没有达到 $51 \%$ 的比例。</p>
<p>这时有聪明的人跳出来，一拍大腿大喊一声 “我知道了！一定都是 UOJ 那个叫妹滋滋的管理员干的！”</p>
<p>人们仔细一想，觉得非常有道理，那些被抓到的犯人们更是叫的比谁都响，早早的把锅甩了出去，更不要说妹滋滋还是著名畅销丛书《MYSQL——从删库到跑路》的作者了。</p>
<p>舆论经过了几天的发酵，已经到了不可收拾的地步，几乎所有人都知道了所谓的 “妹滋滋的阴谋”，于是过街人人喊打的妹滋滋只能开始了她的逃亡之路。</p>
<p>现在妹滋滋在坐标为 $(0,0)$ 的位置，她每天可以往上下左右四个方向中的一个方向移动一个单位的距离。</p>
<p>为了躲避来自四面八方的堵截，妹滋滋觉得 “自己都不知道自己在哪” 的风骚走位是坠吼得，于是她决定每天随机一个方向走。</p>
<p>然而走每个方向的概率并不是相同的，四个方向分别有一个权值，上下左右方向的权值分别是$w_1,w_2,w_3,w_4$，走每个方向的概率和他的权值成正比。</p>
<p>在 $n$ 天后（走了 $n$ 步），厌倦了 “我是谁？我在哪？我要到哪里去” 的日常的妹滋滋开始思考新的问题：这 $n$ 天他经过的不同位置个数的方差 $V$ 是多少？</p>
<p>妹滋滋讨厌小数，所以她想要知道 $V \times (w_1+w_2+w_3+w_4)^n$ 对 $998244353$ 取模后的值。</p>
<p>方差即对于所有$(w_1+w_2+w_3+w_4)^n$种情况的不同位置个数的方差。</p>
<h2>输入格式</h2>
<p>输入第一行一个正整数$n$，表示天数。</p>
<p>第二行4个非负整数$w_1$，$w_2$，$w_3$，$w_4$。分别表示方向上下左右的权值</p>
<h2>输出格式</h2>
<p>一个非负整数，表示答案</p>


<pre><code class="language-input1">2
1 1 1 1
</code></pre>


<pre><code class="language-output1">48
</code></pre>

<h2>explanation</h2>
<p>一共有2天，四个方向的概率相同。总共16种方案，其中有4种只经过2个点，其他12种都经过3个点，平均经过点数为2.75。</p>
<p>于是$V=4*(2-2.75)^{2}+12*(3-2.75)^{2}=3$。</p>
<p>所以$V*(w_1+w_2+w_3+w_4)^{n}=48$。</p>


<pre><code class="language-input2">10
11 21 31 41
</code></pre>


<pre><code class="language-output2">291038161
</code></pre>



<pre><code class="language-input3">100
54 89 77 43
</code></pre>


<pre><code class="language-output3">118369836
</code></pre>

<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th>
<th>限制与约定</th>
</tr></thead><tbody><tr><td>1</td><td rowspan="2">$n \le 10$</td></tr><tr><td>2</td></tr><tr><td>3</td><td rowspan="2">$w_3=w_4=0$</td></tr><tr><td>4</td></tr><tr><td>5</td><td>$n \le 30$</td></tr><tr><td>6</td><td>$n \le 50$</td></tr><tr><td>7</td><td>$w_1=w_2=w_3=w_4$</td></tr><tr><td>8</td><td>$n \le 70$</td></tr><tr><td>9</td><td rowspan="2">$n \le 100$</td></tr><tr><td>10</td></tr></tbody></table></div>

<p>对于所有数据，$1\le n\le 100$，$0 \le w_1,w_2,w_3,w_4 \le 100$，$1\le w_1+w_2+w_3+w_4$</p>
<p><strong>时间限制：</strong>$3\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20651/file/attachment.zip">样例数据下载</a></p>
