<p>在某个诡异的地方，有一座智慧之城，那里的人民平均智商为 192，智商低于 150 的人都被称为弱智。智慧之城的市长名叫卡常（Karp-de-Chant），他 12 岁时在智慧之城中心大学 Cross Institute 获得博士学位，两年后发明了一种数列 —— 卡常数（Karp-de-Chant Number），该数列可用来解决或优化数论、图论等领域的多种经典难题。后来，卡常数被 Trajan（智慧之城的副市长）用 spaly 树进行扩展后，威力大大增加，可以在线性时间内解决各种网络流问题和其它一些难题。卡常和 Trajan 因此分别被选为正、副市长，他们和智慧之城内的另一些智者一起，领导人民共同建设人类智慧，发挥创造和改进的能力。</p>
<p>然而某一天，智慧之城突然受到了反人类智慧者的袭击，反人类智慧者在城内设置了 $N$ 个摄像头（由于他们的智商很低，只会用摄像头这种垃圾玩意），企图监视城内的人们。卡常、Trajan 决定找到这些摄像头并摧毁它们。</p>
<p>智慧之城里有一个用扩展卡常数原理设计的发射器，将其放在合适位置并设置半径以后，所有位于球心为这个发射器的位置、半径为指定值的球面上的目标都能被发现。在卡常、Trajan 的带领下，智慧之城的人们用这个发射器进行了若干次实验，并发现了一些摄像头的位置。比较囧的是，每次发射都能且仅能发现一个摄像头，但是，反馈回来的结果貌似有些不对劲……</p>
<p>后来人们终于找到了这 $N$ 个摄像头的位置，并发现在他们用发射器进行实验的过程中，某些摄像头被移位——这就是导致反馈结果不对劲的原因。但是，在对实验结果进行分析的时候，人们却肿么也回忆不起每次实验发现的摄像头是哪个了（可能是遭遇了灵异事件导致脑抽），只知道每次实验时发射器的位置和半径。你的任务就是，根据实验数据（为了防止被反人类智慧者窃取，已经进行了加密）找出每次实验时被发射器找到的摄像头的编号。</p>
<h2>输入格式</h2>
<p>第一行两个正整数 $N$、$M$，表示摄像头数量（摄像头以 $1$ 到 $N$ 编号）和事件数量。</p>
<p>第二行两个实数 $a$、$b$，表示加密参数。</p>
<p>接下来 $N$ 行，每行三个实数 $(x, y, z)$，表示 $1$ 到 $N$ 号摄像头的初始位置坐标。</p>
<p>接下来 $M$ 行，每行描述一个事件，有两种可能的事件（保证其中实数的精度充分高）：</p>
<ol><li>$0$ $i$ $x$ $y$ $z$，表示将编号为 $i$ 的摄像头的坐标改为 $(x, y, z)$；</li>
<li>$1$ $x$ $y$ $z$ $r$，表示进行一次实验，将发射器放在 $(x, y, z)$ 处并设置半径为 $r$，数据保证每次实验能且仅能发现一个摄像头；</li>
</ol><p>加密方式：设函数 $f(x)=ax-b \sin x$，对于所有事件中的参数（$i$、$x$、$y$、$z$、$r$），均加密成 $f(\text{last_res} \times 原值 + 1)$，其中 $\text{last_res}$ 为上一个实验事件的返回值（即发现的摄像头编号），若之前未进行过实验则 $\text{last_res} = 0.1$。</p>
<h2>输出格式</h2>
<p>对于每个实验事件，输出发现的摄像头编号，一个一行。</p>


<pre><code class="language-input1">6 10
1 0
-3.6 7.2 3.6
9.7 0.4 0.5
8.8 -4.7 0.5
9.6 8.2 -5.7
0.3 -9.9 1.5
0.5 -5.7 -1.0
0 1.3 1.92 0.13 1.85
1 1.98 1.55 1.2 2.360183811
1 8.2 0.9 2.1 9.981091248
1 -7.4 -44.0 11.2 83.061927835
1 20.8 -9.6 -11.8 31.598039153
0 10.0 11.2 -19.73 -19.1
0 13.0 7.3 28.6 22.6
0 4.0 22.3 -17.6 1.3
1 -3.2 -14.0 16.6 30.9549661993
0 7.0 -3.1 5.8 -0.9
</code></pre>


<pre><code class="language-output1">1
6
2
3
1
</code></pre>

<h2>样例二</h2>
<p>见样例数据下载。</p>
<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th>
<th>$n$</th>
<th>$m$</th>
<th>附加信息</th>
</tr></thead><tbody><tr><td>1</td><td>$1024$</td><td>$1024$</td><td rowspan="2">无</td></tr><tr><td>2</td><td>$2048$</td><td>$2048$</td></tr><tr><td>3</td><td>$32768$</td><td>$32768$</td><td rowspan="3">没有摄像头移位事件</td></tr><tr><td>4</td><td>$32768$</td><td>$65536$</td></tr><tr><td>5</td><td>$65536$</td><td>$65536$</td></tr><tr><td>6</td><td>$32768$</td><td>$32768$</td><td rowspan="5">无</td></tr><tr><td>7</td><td>$32768$</td><td>$65536$</td></tr><tr><td>8</td><td>$65536$</td><td>$32768$</td></tr><tr><td>9</td><td>$65536$</td><td>$65536$</td></tr><tr><td>10</td><td>$65536$</td><td>$65536$</td></tr></tbody></table></div>

<p>所有的测试点满足 $0 \leq b &lt; a &lt; 5$，坐标的绝对值均不超过 $100$，所有坐标均为随机生成且至少精确到 $10^{-5}$。</p>
<p>为尽可能减小精度误差，建议 C/C++ 使用long double类型、Pascal 使用 EXTENDED 类型存储实数。</p>
<p><strong>时间限制</strong>：$5\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>来源</h2>
<p>中国国家队清华集训2014~2015 Day 2 - By 梁泽宇</p>
<h2>下载</h2>
<p><a href="./20480/file/attachment.zip">样例数据下载</a></p>
