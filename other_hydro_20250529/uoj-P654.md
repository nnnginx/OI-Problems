<p>为了打倒邪恶管理员 Skip 蚤，跳蚤国王决定“以其人之道还治其人之身”。</p>
<p>跳蚤国王事先在 Skip 蚤的电脑中留下了后门。跳蚤国王计划通过后门攻破管理员 skip 蚤。</p>
<p>一个后门可以用一个非空序列$A$表示，攻破这个后门需要花费的时间为 $S(A)$。</p>
<p>对于长度为 $n$ 的序列 $A=\{A_0,A_1,\cdots,A_{n-1}\}$，定义 ${\rm scr}_{k,c}(A)$ 为将下标模 $k$ 等于 $c$ 的位置抽出组成的序列，保证 $c\leq k-1\leq n-1$，即 ${\rm scr}_{k,c}(A)=\{A_c\ ,A_{k+c}\ ,A_{2k+c}\ ,\cdots\}$。</p>
<p>对于任意一个序列 $A$ 定义权值函数 $S(A)$：</p>
<p>$$
     S(A) = \left\{\begin{array}{lr}
        A_0, &amp; \text{for } |A|=1,\\
        \sum_{d=2}^{|A|}\sum_{c=0}^{d-1}S\left({\mathrm {scr}}_{d,c}(A)\right), &amp; \text{otherwise.}
        \end{array}\right.
$$</p>
<p>现在，你已经知道了 Skip 蚤的电脑的后门，和表示它的长为 $n$ 的序列 $A$。</p>
<p>求出攻破它花费的时间 $S(A)$ 的值，答案对 $2^{32}$ 取模。</p>
<p>由于本题中 $n$ 较大，为避免文件操作占用过多时间，序列 $A$ 将由随机数生成器生成。本题的标准解法不依赖该随机性。</p>
<h2>输入格式</h2>
<p>一行，两个整数，分别为 $n,seed$。</p>
<p>随机数生成器的 <code>C++</code> 代码如下 ：</p>
<pre><code class="sh_cpp">namespace GenHelper
{
    unsigned z1,z2,z3,z4,b;
    unsigned read()
    {
        b=((z1&lt;&lt;6)^z1)&gt;&gt;13;
        z1=((z1&amp;4294967294U)&lt;&lt;18)^b;
        b=((z2&lt;&lt;2)^z2)&gt;&gt;27;
        z2=((z2&amp;4294967288U)&lt;&lt;2)^b;
        b=((z3&lt;&lt;13)^z3)&gt;&gt;21;
        z3=((z3&amp;4294967280U)&lt;&lt;7)^b;
        b=((z4&lt;&lt;3)^z4)&gt;&gt;12;
        z4=((z4&amp;4294967168U)&lt;&lt;13)^b;
        return (z1^z2^z3^z4);
    }
    void srand(int x)
    {
        z1=x;
        z2=(~x)^0x233333333U;
        z3=x^0x1234598766U;
        z4=(~x)+51;
    }
}
using namespace GenHelper;</code></pre>
<p>您要首先调用一次 <code>srand(seed)</code> ，然后连续调用 $n$ 次 <code>read()</code> ，第 $i$ 次的返回值即为 $A_{i-1}$。在 $0\sim 2^{32-1}$ 的范围内。</p>
<h2>输出格式</h2>
<p>输出一行一个整数，表示 $S(A)\bmod 2^{32}$。</p>


<pre><code class="language-input1">3 1
</code></pre>


<pre><code class="language-output1">1484747852
</code></pre>


<p>生成的序列为 $\{535855898,2903825961,3745143011\}$</p>


<pre><code class="language-input2">5 2
</code></pre>


<pre><code class="language-output2">16835609
</code></pre>



<pre><code class="language-input3">100 3
</code></pre>


<pre><code class="language-output3">2637589059
</code></pre>

<h2>限制与约定</h2>
<p>对于所有数据， $1\leq n\leq 2\times 10^6,1\leq seed\leq 10^8$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n\leq$</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">1</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">2</td>
<td style="text-align:center;">$800$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">3</td>
<td style="text-align:center;">$8\times 10^4$</td>
<td style="text-align:center;">$35$</td>
</tr>
<tr>
<td style="text-align:center;">4</td>
<td style="text-align:center;">$2\times 10^6$</td>
<td style="text-align:center;">$35$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong> : $1\texttt{s}$。</p>
<p><strong>空间限制</strong> : $256\texttt{MB}$。</p>
<h2>下载</h2>
<p><a href="./21055/file/attachment.zip">样例数据下载</a></p>
