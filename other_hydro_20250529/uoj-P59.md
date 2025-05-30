<p>为了鼓励人们多参加运动，小Q所在的CD市的体育中心有一项长期的积分送礼活动。</p>
<p>体育中心有许多项运动，每项运动有一个固定的非负整数积分，每参加一次该项运动可以积累相应的一次积分。体育中心每个月都会推出一种新的礼品，当月积分大于等于当月的礼品积分时，就可以用相应的积分值换取一份礼品，每月的积分都只能在当月使用，不能积累到下一个月。</p>
<p>小Q是个运动达人，平时的爱好就是邀请一群朋友到体育中心参加各类体育项目。因为有朋友的帮助，小Q每月都可以换得很多的礼品。</p>
<p>新的一月快要到了，小Q又开始了对下一月运动的计划。可是，小Q发现他记录每项体育运动积分的表格不见了。这份表格可是小Q花了一年时间收集，记录了体育中心大大小小所有体育项目积分的表格。</p>
<p>万分沮丧的小Q突然想起他还有记录每个月参加每个项目次数的习惯。后来他又来到体育中心网站上查到了他每个月的剩余积分，也就是他当月的总积分扣除若干份礼物的所需要的积分后剩下的积分。至于每个月小Q领了多少份礼物，小Q自己也不记得了。</p>
<p>小Q想，用这些数据也许能求出每项运动的积分。经过推导，小Q发现如果某一个月的记录出错了，很有可能就会出现无解的情况。小Q每个月参加的体育项目很多，记错一两次也是很正常的。</p>
<p>最后小Q想了一个比较折中的办法：求每项运动的积分，使这个积分能满足尽量多月份的记录。</p>
<p>由于小Q还要去参加今天的体育运动，所以这个问题和众多的问题一样，要交给学信息学竞赛的你。</p>
<h2>输入格式</h2>
<p>该题为提交答案型试题，所有输入数据 sports1.in ~ sports10.in 见数据下载。</p>
<p>输入的第一行包含两个正整数 $n, m$，分别表示体育项目的个数和有记录的月份数。</p>
<p>接下来有 $m$ 行，每行有 $n + 2$ 个非负整数，表示一个月的记录。前 $n$ 个数中的第 $i$ 个数表示小Q在该月参加第 $i$ 个体育项目的次数，第 $n + 1$ 个数表示该月兑换一份礼物所需的积分，第 $n + 2$ 个数表示兑换了若干次礼物以后剩余的积分。</p>
<p>保证输入每个数均不超过 $2^{31} - 1$。</p>
<p>输入文件的末尾包含 $8$ 行，每行包含一个整数，为参数 $a_3, a_4, \dots, a_{10}$，意义见评分方法。</p>
<h2>输出格式</h2>
<p>针对给定的 10 个输入文件 sports1.in ~ sports10.in，你需要分别提交你的输出文件 sports1.out ~ sports10.out。</p>
<p>每个输出文件输出 $n$ 行，每行包含一个小于 $10^{10m}$（不超过 $10m$ 位）的非负整数。其中第 $i$ 行表示第 $i$ 个体育项目的积分。</p>


<pre><code class="language-input1">2 4
2 0 4 2
0 2 3 1
5 7 24 16
2 0 4 5
2
2
1
1
0
0
0
0
</code></pre>


<pre><code class="language-output1">7
11
</code></pre>


<p>第 1 条记录：$2 \times 7 + 0 \times 11 = 14$，兑换 $3$ 次奖品后剩余 $2$ 分；</p>
<p>第 2 条记录：$0 \times 7 + 2 \times 11 = 22$，兑换 $7$ 次奖品后剩余 $1$ 分；</p>
<p>第 3 条记录：$5 \times 7 + 7 \times 11 = 112$，兑换 $4$ 次奖品后剩余 $16$ 分；</p>
<p>第 4 条记录：无论如何设定每个体育项目的得分，都无法满足该条记录。</p>
<h2>评分方法</h2>
<p>对于每组数据，我们设置了 $8$ 个评分参数 $a_3, a_4, \dots, a_{10}$。如果选手的输出不合法，则得零分。否则，设在你的方案中，满足的月份个数为 $w_u$，我们给出的答案的月份个数为 $w_s$，你的分数将会由下表给出：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>得分</th><th>条件</th><th>得分</th><th>条件</th></tr></thead><tbody><tr><td>10</td><td>$w_s - w_u \leq a_{10}$</td><td>5</td><td>$w_s - w_u \leq a_5$</td></tr><tr><td>9</td><td>$w_s - w_u \leq a_9$</td><td>4</td><td>$w_s - w_u \leq a_4$</td></tr><tr><td>8</td><td>$w_s - w_u \leq a_8$</td><td>3</td><td>$w_s - w_u \leq a_3$</td></tr><tr><td>7</td><td>$w_s - w_u \leq a_7$</td><td>2</td><td>$w_u \geq 0$</td></tr><tr><td>6</td><td>$w_s - w_u \leq a_6$</td><td>1</td><td>$w_u \geq 0$</td></tr></tbody></table></div>

<p>如果有多项满足，则取满足条件中的最高得分。</p>
<h2>如何测试你的输出</h2>
<p>在终端中先切换到该试题的目录下：（windows用户请使用cmd）</p>
<p><code>cd sports</code></p>
<p>我们提供checker这个工具来测试你的输出文件是否是可接受的。使用这个工具的方法是，在终端中运行</p>
<p><code>./checker_linux64 &lt;case_no&gt;</code></p>
<p>其中<code>case_no</code>是测试数据的编号。例如</p>
<p><code>./checker_linux64 3</code></p>
<p>将测试sports3.out是否可以接受。（windows用户请使用<code>checker_win32 3</code>）（什么你是windows 64位？放心吧可以运行win32应用程序的。）</p>
<p>当然我们有对应的linux 32位版本：<code>checker_linux32</code>。如果linux用户发现无法运行程序，请尝试执行<code>chmod +x checker_linux64</code>或<code>chmod +x checker_linux32</code>后重试。</p>
<p>其它操作系统请安装 <a href="//nodejs.org/">node.js</a> 然后使用 <code>node checker.js &lt;case_no&gt;</code> 运行checker。</p>
<p>在你调用这个程序后，checker将根据你给出的输出文件给出测试的结果。</p>
<h2>下载</h2>
<p><a href="./20499/file/attachment.zip">输入数据及checker下载</a></p>
