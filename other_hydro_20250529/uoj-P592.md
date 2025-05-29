<p><strong>这是一道交互题。</strong></p>
<p><strong> 由于某些原因本题仅支持 C++, C++11 语言的提交。 </strong></p>
<p>你通过你派遣到黑衣人中的卧底，知晓了神犇被黑衣人 $03$ 当做了坐骑，并取名为 <code>ak's cow</code>，并且它过几天就要被吃了。</p>
<p>为了救出神犇，你需要打探出黑衣人 $03$ 手下之间的关系，黑衣人 $03$ 有 $n$ 个手下，编号为 $0\sim n-1$，其中有 $m$ 对手下 $a_i$, $b_i$ 之间关系不佳。</p>
<p>你决定举办好多次聚会，每次聚会可以邀请一些黑衣人 $03$ 的手下，但是邀请的名单必须给每个人看，如果有人发现名单里存在和自己关系不佳的人，他就会拒绝来聚会，这次聚会就不能举办成功。</p>
<p>由于时间紧急，你最多举办聚会次数不能太多，由于资金有限，所有聚会的人数和不能太大，而你需要知道哪些手下之间关系不佳。</p>
<h2>任务</h2>
<p>你必须引用 <code>meeting.h</code> 头文件。</p>
<p>你需要实现下面的过程：</p>
<pre><code class="sh_cpp">std::vector&lt;std::pair&lt;int, int&gt;&gt; solve(int n);</code></pre>
<p>其中 $n$ 是黑衣人 $03$ 的手下数量，而关系不佳的手下对数你并不知道，你需要返回关系不佳的手下，顺序任意。</p>
<p>你可以调用以下过程和交互库进行交互：</p>
<pre><code class="sh_cpp">bool meeting(std::vector&lt;int&gt; set);</code></pre>
<p>该函数表示你就将举办一场聚会，其中 <code>set</code> 是一个包含要邀请的人的编号的 vector。当聚会能正常举办时返回值为 <code>true</code>，否则为 <code>false</code>。你必须保证所有编号在合法范围内且互不相同，不然你会获得 $0$ 分。</p>
<h2>评测方式</h2>
<p>样例评测库将读入如下格式的输入数据：</p>
<p>第一行包括两个正整数 $n$ 和 $m$，表示黑衣人 $03$ 的手下个数，与关系不佳的手下对数。</p>
<p>接下来 $m$ 行，每行两个整数 $x_i, y_i$，表示手下 $x_i$ 与 $y_i$ 关系不佳，一对关系不佳的手下只会被读入一次，且没有手下和自己关系不佳。</p>
<p><strong>在最终测试中，关系不佳的手下是确定的，不会因为你的询问而改变。</strong></p>
<p>样例评测库将输出如下格式的输出数据：</p>
<p>如果程序正常运行，则输出两个整数 $cnt, size$，表示举办聚会个数与总人数，否则会输出错误信息。</p>


<pre><code class="language-input1">2 1
0 1
</code></pre>


<pre><code class="language-output1">1 2
</code></pre>


<p>我们可以直接调用 <code>meeting([0, 1])</code> 来检验唯一一对可能关系不佳的手下，我们发现它们关系不佳于是可以返回 <code>[(0, 1)]</code>。</p>
<h2>样例二</h2>
<p>见下载文件中的 <code>ex_meeting2.in</code> 与 <code>ex_meeting2.out</code>。</p>
<h2>限制与约定</h2>
<p>对于所有数据，$1 \leq n \leq 1000, 1 \leq m \leq 2000$。</p>
<p>对于所有测试点，我们会根据以下方式计分：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">编号</th>
<th style="text-align:center;">聚会个数上限</th>
<th style="text-align:center;">聚会总人数上限</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$499500$</td>
<td style="text-align:center;">$10^7$</td>
<td style="text-align:center;">$25$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$50000$</td>
<td style="text-align:center;">$10^7$</td>
<td style="text-align:center;">$35$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$50000$</td>
<td style="text-align:center;">$10^6$</td>
<td style="text-align:center;">$40$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>对每个部分，你满足其要求就可以获得其分数。</strong></p>
<p>若聚会个数不超过 $500000$，且聚会总人数不超过 $10^7$，交互库运行时间不会超过 $2\texttt{s}$。</p>
<p>若聚会个数不超过 $50000$，交互库运行时间不会超过 $200\texttt{ms}$。</p>
<p>保证交互库使用空间不超过 $4 \texttt{MB}$。</p>
<p><strong>时间限制</strong>：$3\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="https://uoj.ac/download.php?type=problem&amp;id=592">样例数据与样例评测库下载</a></p>
