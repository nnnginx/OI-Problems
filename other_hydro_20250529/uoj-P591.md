<p>根据各路消息打听，你得知神牪被黑衣人 $02$ 关押在了一间密码房，而明天神牪就会被抓走吃掉。</p>
<p>你通过你强大的本领，知道了黑衣人 $02$ 的老巢，你发现这关押神牪的地点名字叫做 <code>le's home</code>，并且大门有一把十分强大的密码锁。你经过大量实验，发现你不能像某些主角一样马上破解它，于是你开始想办法。</p>
<p>具体而言这把密码锁的情况是这样的：</p>
<p>第一部分是密码锁部分，你通过严密的论证，发现你不会破解这一部分。</p>
<p>而对于第二部分，就是暴力拆锁。锁形状是一棵树，树上有很多铁链，每个铁链覆盖了树某个点 $u_i$ 到另外一个点 $v_i$ 的路径，并且你若要拆解它，你还需要耗费 $w_i$ 的体力。</p>
<p>黑衣人 $02$ 使用了强力 $250$ 胶水，在每个节点把经过这个点的所有铁链粘在了一起。而你想要蛮力破解这把锁的话，你需要先暴力拆解几条铁链，直到剩下存在两条铁链不直接或间接粘在一起（铁链 $a$ 与 $b$ 间接粘在一起，当且仅当 $a$ 和 $b$ 粘在一起或者存在铁链 $c$，使得 $a$ 与 $c$ 间接粘在一起且 $b$ 与 $c$ 间接粘在一起）。</p>
<p>经过不停的打探，你发现了越来越多的铁链，每知晓一条新的铁链，你想知道若只有这些铁链，完成任务所需要消耗体力的最小值。当然有可能这是一个不可能完成的任务，此时你需要输出 <code>-1</code>。</p>
<h2>输入格式</h2>
<p>第一行两个正整数 $n, q$，表示树中的节点数，依次知道的铁链数量。</p>
<p>下面 $n - 1$ 行，每行两个正整数 $x_i, y_i$ 表示树上这两个节点直接存在边。</p>
<p>下面 $q$ 行，每行三个正整数 $u_i, v_i, w_i$，表示新知道一条，覆盖了 $u_i$ 到 $v_i$ 的路径，需要消耗 $w_i$ 体力拆除的铁链。</p>
<h2>输出格式</h2>
<p>一共 $q$ 行，每行一个整数表示答案。</p>


<pre><code class="language-input1">5 5
1 2
2 3
2 4
1 5
2 4 511332337
1 4 919238353
5 1 597538394
2 1 170644152
5 2 848575637
</code></pre>


<pre><code class="language-output1">-1
-1
919238353
1089882505
1938458142
</code></pre>

<h2>样例二</h2>
<p>见下载文件中的 <code>ex_lock2.in</code> 与 <code>ex_lock2.out</code>，该样例符合子任务 $3$ 的限制。</p>
<h2>样例三</h2>
<p>见下载文件中的 <code>ex_lock3.in</code> 与 <code>ex_lock3.out</code>，该样例符合子任务 $4$ 的限制。</p>
<h2>限制与约定</h2>
<p>对于所有测试点，$1 \leq n, q \leq 2 \times 10^5, 1 \leq u_i, v_i, x_i, y_i \leq n, u_i \neq v_i, 1\leq w_i \leq 10^9$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n, q \le $</th>
<th style="text-align:center;">特殊性质</th>
<th style="text-align:center;">分值</th>
</tr></thead><tbody><tr><td style="text-align:center;">$1$</td>
<td style="text-align:center;">$16$</td>
<td style="text-align:center;" rowspan="3">无</td>
<td style="text-align:center;">$16$</td>
</tr><tr><td style="text-align:center;">$2$</td>
<td style="text-align:center;">$300$</td>
<td style="text-align:center;">$13$</td>
</tr><tr><td style="text-align:center;">$3$</td>
<td style="text-align:center;">$3000$</td>
<td style="text-align:center;">$19$</td>
</tr><tr><td style="text-align:center;">$4$</td>
<td style="text-align:center;" rowspan="2">$200000$</td>
<td style="text-align:center;">$x_i = y_i - 1$</td>
<td style="text-align:center;">$23$</td>
</tr><tr><td style="text-align:center;">$5$</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">$29$</td>
</tr></tbody></table></div>
<p><strong>时间限制</strong>：$3\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="https://uoj.ac/download.php?type=problem&amp;id=591">样例数据下载</a></p>
