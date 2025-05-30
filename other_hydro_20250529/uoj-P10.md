<p>pyx喜欢出题给cyb做。为了增加难度，他有可能在cyb还没做完前面的题的时候就把新题目出给他。</p>
<p>假设pyx总共要给cyb出$n$道题，其中第$i$道题是在$t_i$时刻出给cyb的，cyb需要花$s_i$秒才能AC此题。</p>
<p>pyx比较高产，出题时刻可能相同（也就是pyx可能同一时刻丢出了动态仙人掌和可持久化带插入仙人掌路径k大值给cyb）。</p>
<p>按照cyb的个人喜好，他给$n$道题目标上了<strong>互不相同</strong>的优先级$p_i$。</p>
<p>cyb做题过程是这样的：</p>
<ul><li>cyb收到题目是瞬间的事情。</li>
<li>每次，cyb先收到所有pyx新出的题。</li>
<li>接着，cyb把现在所有待解决的题目按照优先级瞬间排序。（当然优先级是互不相同的）</li>
<li>然后，cyb会花恰好$1$秒钟时间在那个优先级最高的题，然后解决该题需要花的时间减少$1$秒。如此循环。</li>
</ul><p>由于是神犇之间的交流，十分有记录的意义，需要载入史册，这个光荣的任务就交给修电脑的oier们了。</p>
<p>现在给你$n$道题的$t_i, s_i, p_i$。然而不幸的是，由于奇怪的原因，你一不小心把<strong>某一道题</strong>的优先级弄丢了。</p>
<p>你为了掩饰自己的错误，通过不断打听，得知了cyb在时刻$T$时AC了这道优先级未知的题目。（即第$T$秒末，第$T$秒结束的时刻）</p>
<p>你想试着推测出优先级，然而很显然，方案可能不止一种。你决定编造这个题目的优先级，使得cyb仍会在时刻$T$ AC此题。</p>
<p>除此之外，你还要帮cyb算出所有题目被解决的时刻，以展示你是多么的负责。</p>
<p>也就是说，你要求出一个可行的优先级，并求出在这个优先级下，所有题目被解决掉的时刻。</p>
<h2>输入格式</h2>
<p>第一行输入一个正整数$n$。</p>
<p>接下来$n$行描述一个题目，第$i$行有三个整数分别是$t_i, s_i, p_i$，含义如前所述。有且仅有一个题目（我们不妨称其为题目$x$）的$p_x = -1$，表示该题的优先级未知。</p>
<p>最后一行包含一个整数$T$——任务$x$完成的时刻。</p>
<p>所有题目的优先级互不相同，但 $t_i$ 并不一定互不相同。</p>
<h2>输出格式</h2>
<p>在第一行输出一个正整数$p_x$——即题目$x$的优先级（请记住所有题目的优先级必须互不相同）。接下来输出$n$个数字，第$i$个数字表示第$i$个题目结束时的时间。</p>
<p>我们保证数据有解。如果有多解，输出任意一组解即可。</p>
<p><strong>输出的优先级必须在$[1, 10 ^ 9 + 1]$之内</strong>。</p>


<pre><code class="language-input1">3
4 3 -1
0 2 2
1 3 3
7
</code></pre>


<pre><code class="language-output1">4
7 8 4
</code></pre>



<pre><code class="language-input2">3
3 1 2
2 3 3
3 1 -1
4
</code></pre>


<pre><code class="language-output2">4
7 6 4
</code></pre>

<h2>样例三</h2>
<p>见样例数据下载</p>
<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th>
<th>$n$的大小</th>
<th>$t$的大小</th>
</tr></thead><tbody><tr><td>1</td><td>$n \le 5$</td><td>$t_i \le 5$</td>
</tr><tr><td>2</td><td>$n \le 10$</td><td>$t_i \le 10$</td>
</tr><tr><td>3</td><td>$n \le 50$</td><td>$t_i \le 50$</td>
</tr><tr><td>4~12</td><td>$n \le 100$</td><td>$t_i \le 10000$</td>
</tr><tr><td>13~14</td><td>$n \le 50000$</td><td>$t_i \le 50000$</td>
</tr><tr><td>15~18</td><td>$n \le 50000$</td><td>$t_i \le 1000000000$</td>
</tr><tr><td>19~20</td><td>$n \le 300000$</td><td>$t_i \le 1000000000$</td>
</tr></tbody></table></div>

<p>保证$0 \le t_i \le 10^9,1 \le s_i,p_i \le 10^9, 1 \le T \le 10^{15}$。（$p_x$例外，$p_x = -1$）</p>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20450/file/attachment.zip">样例数据下载</a></p>
