<p>这是一道模板题。</p>
<p>读入一个长度为 $n$ 的由小写英文字母组成的字符串，请把这个字符串的所有非空后缀按字典序从小到大排序，然后按顺序输出后缀的第一个字符在原串中的位置。位置编号为 $1$ 到 $n$。</p>
<p>除此之外为了进一步证明你确实有给后缀排序的超能力，请另外输出 $n - 1$ 个整数分别表示排序后相邻后缀的最长公共前缀的长度。</p>
<h2>输入格式</h2>
<p>一行一个长度为 $n$ 的仅包含小写英文字母的字符串。</p>
<h2>输出格式</h2>
<p>第一行 $n$ 个整数，第 $i$ 个整数表示排名为 $i$ 的后缀的第一个字符在原串中的位置。</p>
<p>第二行 $n - 1$ 个整数，第 $i$ 个整数表示排名为 $i$ 和排名为 $i + 1$ 的后缀的最长公共前缀的长度。</p>


<pre><code class="language-input1">ababa
</code></pre>


<pre><code class="language-output1">5 3 1 4 2
1 3 0 2
</code></pre>


<p>排序后结果为：</p>
<ol><li><samp>a</samp></li>
<li><samp>aba</samp></li>
<li><samp>ababa</samp></li>
<li><samp>ba</samp></li>
<li><samp>baba</samp></li>
</ol><h2>限制与约定</h2>
<p>$1 \leq n \leq 10^5$</p>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20475/file/attachment.zip">样例数据下载</a></p>
