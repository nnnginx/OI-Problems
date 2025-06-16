<p><strong>这是一道交互题。</strong></p>
<p><strong>由于某些原因本题仅支持 C++, C++11 语言的提交。</strong></p>
<p>作为文化课大师，skip 蚤被跳蚤大学邀请参加跳蚤大学举办的跳蚤营。</p>
<p>在跳蚤营中，skip 蚤顺利的通过了考试，进入了面试。在面试中，面试考官给了 skip 蚤一个困难的问题。skip 蚤需要猜出面试官心中所想的 $3$ 个非负整数 $a,b,c$ 。面试官在最开始给了 skip 蚤一个正整数 $n$ ，表示 $a,b,c$ 都在区间 $[0,n]$ 中。skip 蚤每次可以告诉面试官三个非负整数 $x,y,z$ 满足 $0\leq x,y,z\leq n$ ，面试官会回答他 $|a+b-x-y|+|b+c-y-z|+|c+a-z-x|$ 的值。现在 skip 蚤想要通过尽量少的询问得到面试官所想的那 $3$ 个数。面试官为了确保 skip 蚤不是瞎蒙蒙对的，他会想多组 $a,b,c$ 让 skip 蚤去猜。</p>
<h2>任务</h2>
<p>你必须引用 <code>head.h</code> 头文件。</p>
<p>你需要实现下面的过程：</p>
<pre><code class="sh_cpp">void work(int N,int tp,int &amp;a,int &amp;b,int &amp;c);</code></pre>
<p>其中 $N$ 是面试官给出的 $n$ 的值， $tp$ 代表数据点是哪一类数据（你可能不需要用到它），你需要将最后猜的三个数分别写入 $a,b,c$ 中。</p>
<p>你可以调用以下过程和交互库进行交互：</p>
<pre><code class="sh_cpp">int query(int x,int y,int z);</code></pre>
<p>其中 $x,y,z$ 是向面试官提问所包含的三个非负整数，返回 $|a+b-x-y|+|b+c-y-z|+|c+a-z-x|$ 的值。你必须保证 $0\leq x,y,z\leq n$ ，不然交互库会返回 $-1$ 且你这次猜测会被视为失败。</p>
<h2>评测方式</h2>
<p>样例评测库将读入如下格式的输入数据：</p>
<p>第一行包括两个正整数 $T$ 和 $tp$，表示面试官让 skip 蚤猜的次数，与数据点是哪一类数据（样例为 $0$ ）。</p>
<p>接下来 $T$ 行，每行五个整数 $N_i,a_i,b_i,c_i,Q_i$ ，分别代表 $n$ 的大小，面试官心中所想的 $3$ 个数，和 skip 蚤最多询问多少次。</p>
<p><strong>在最终测试中，面试官心中所想的 $a,b,c$ 是确定的，不会因为你的询问而改变。</strong></p>
<p>样例评测库将输出如下格式的输出数据：</p>
<p>对于每一组数据，如果你正确给出了 $a,b,c$ 的值且询问次数没有超过限制次数，会输出一行一个数 $1$ ，否则会输出一行一个数 $0$ 。</p>


<pre><code class="language-input1">1 0
4 1 2 3 3
</code></pre>


<pre><code class="language-output1">1
</code></pre>

<h2>数据范围</h2>
<p>对于 $100\%$ 的数据， $1\leq T\leq 10^5,1\leq n\leq 10^8,3\leq Q\leq 1000$ 。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$tp=$</th>
<th>$T=$</th>
<th>$n$</th>
<th>$Q=$</th>
<th>特殊性质</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1\sim 2$</td>
<td style="text-align:center;">$1$</td>
<td>$100$</td>
<td>$=9$</td>
<td>$1000$</td>
<td rowspan="3">无</td>
</tr>
<tr>
<td style="text-align:center;">$3\sim 5$</td>
<td style="text-align:center;">$2$</td>
<td>$100000$</td>
<td>$\leq 10^8$</td>
<td>$4$</td>
</tr>
<tr>
<td style="text-align:center;">$6\sim 9$</td>
<td style="text-align:center;">$3$</td>
<td>$100000$</td>
<td>$=4$</td>
<td>$3$</td>
</tr>
<tr>
<td style="text-align:center;">$10\sim 13$</td>
<td style="text-align:center;">$4$</td>
<td>$100000$</td>
<td>$\leq 10^8$</td>
<td>$3$</td>
<td>$A$</td>
</tr>
<tr>
<td style="text-align:center;">$14\sim 20$</td>
<td style="text-align:center;">$5$</td>
<td>$100000$</td>
<td>$\leq 10^8$</td>
<td>$3$</td>
<td>无</td>
</tr>
</tbody>
</table>
</div>
<p>$A$ ：保证 $a,b,c$ 在 $[0,n]$ 内均匀随机，且只要在所有面试官想的次数中猜对其中至少 $40\%$ 即可得分。</p>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$1\texttt{GB}$</p>
<h2>下载</h2>
<p><a href="./21010/file/attachment.zip">样例数据下载</a></p>
