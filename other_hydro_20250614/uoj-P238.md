<p>按数目填色是个有名的智力游戏。我们现在考虑的是这个游戏的一维版本。在这个游戏中，玩家会有一行 $n$ 个方格。这些方格从左到右分别编号为 $0$ 至 $n - 1$。玩家必须要为这些方格填上黑色或白色，我们用 <samp>'X'</samp> 代表填上黑色的方格并用 <samp>'_'</samp> 来代表填上白色的方格。</p>
<p>系统将会给玩家一个提示，这个提示是一个含有 $k$ 个正整数的序列 $c = [c_0, \ldots, c_{k - 1}]$。而玩家必须要根据提示为方格填色，填色的要求是在这行上，填上黑色的方格必须组成 $k$ 个连续的区间，而且，在由左开始的第 $i$ (由 $0$ 开始) 个区间上必须含有 $c_i$ 个黑色方格。例如，若提示为 $c = [3, 4]$，则该游戏的正确填色方法是必须含有两个由连续黑色格位组成的区间，这两个区间的长度分别是 $3$ 和 $4$。因此，若 $n = 10$ 且 $c = [3, 4]$ 的话，则满足提示的一个正确的填色方法是 <samp>'_XXX__XXXX'</samp>。要注意的是 <samp>'XXXX_XXX__'</samp> 并不满足提示，因为黑色的区间的长度顺序不正确。同时 <samp>'__XXXXXXX_'</samp> 也不满足提示，因为它只含有一个黑色区间而非两个分开的黑色区间。</p>
<p>你将获得一个部分方格已填好颜色的游戏行格，即，你知道 $n$ 及 $c$ 的值，并且你也知道有些方格一定是黑色和有些方格一定是白色。你的工作是从中推算出更详细的方格的信息。</p>
<p>更加详细来说，一个正确的游戏解应该满足提示，并且和已经知道颜色的方格的颜色一致。你的程序必须找出在所有正确的游戏解中都会填上黑色的方格和在所有正确的游戏解中都会填上白色的方格。</p>
<p>你可以假设每个输入一定存在至少一个正确的游戏解。</p>
<h2>实现细节</h2>
<p>你必须编写程序以实现以下的函数（或方法）：</p>
<ul><li><code>std::string solve_puzzle(std::string s, std::vector&lt;int&gt; c)</code>，<ul><li><code>s</code>: 一个含有 $n$ 个字符的字符串。而对于每个 $i$ ($0 \le i \le n - 1$)，字符 $i$ 将会是以下其中一个：<ul><li><samp>'X'</samp>, 表示方格 $i$ 必须要填上黑色，</li>
<li><samp>'_'</samp>, 表示方格 $i$ 必须要填上白色，</li>
<li><samp>'.'</samp>, 表示方格 $i$ 没有任何信息。</li>
</ul></li>
<li><code>c</code>: 是一个长度为 $k$ 的数组，它的内容是上面叙述中所讲的提示，</li>
<li>这函数必须要返回一个长度为 $n$ 的数组。对于每个 $i$ ($0 \le i \le n - 1$) 而言，输出字符串的第 $i$ 个字符应该是以下其中一个：<ul><li><samp>'X'</samp>, 表示在所有游戏解中，第 $i$ 个方格都是填上黑色，</li>
<li><samp>'_'</samp>, 表示在所有游戏解中，第 $i$ 个方格都是填上白色，</li>
<li><samp>'?'</samp>, 表示其他情况（即该游戏中存在两个正确的游戏解，且其中一个解该方格是填上黑色，但在另一个解中该方格是填上白色）。</li>
</ul></li>
</ul></li>
</ul><h2>样例一</h2>
<p><code>solve_puzzle("..........", [3, 4])</code></p>
<p>以下是这次游戏的所有正确的解：</p>
<ul><li><samp>"XXX_XXXX__"</samp>,</li>
<li><samp>"XXX__XXXX_"</samp>,</li>
<li><samp>"XXX___XXXX"</samp>,</li>
<li><samp>"_XXX_XXXX_"</samp>,</li>
<li><samp>"_XXX__XXXX"</samp>,</li>
<li><samp>"__XXX_XXXX"</samp>.</li>
</ul><p>你可以观察到下标为 $2, 6,$ 和 $7$ (从 $0$ 开始) 的方格在所有正确的解中都是黑色，而其他的所有方格可能但不一定是黑色的。所以正确的答案应该是 <samp>??X???XX??</samp>。</p>
<h2>样例二</h2>
<p><code>solve_puzzle("........", [3, 4])</code></p>
<p>在这个样例中，正确的填色方法只有一种，即 <samp>"XXX_XXXX"</samp>。</p>
<h2>样例三</h2>
<p><code>solve_puzzle("..._._....", [3])</code></p>
<p>在这个样例中，我们可以推出方格 $4$ 一定是白色，因为在白色的方格 $3$ 和方格 $5$ 之间根本不可能容纳 $3$ 个连续的方格，因此正确的答案应该是 <samp>"???___????"</samp>。</p>
<h2>样例四</h2>
<p><code>solve_puzzle(".X........", [3])</code></p>
<p>只有两个正确解符合上述描述：</p>
<ul><li><samp>"XXX_______"</samp>,</li>
<li><samp>"_XXX______"</samp>.</li>
</ul><p>因此正确的答案应该是 <samp>"?XX?______"</samp>。</p>
<h2>子任务</h2>
<p>在所有的子任务中 $1 \le k \le n, 1 \le c_i \le n$ (对于每个 $0 \le i \le k - 1$)。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>子任务</th>
<th>分数</th>
<th>$n \le $</th>
<th>$k \le $</th>
<th>对 `s` 的限制</th>
</tr></thead><tbody><tr><td>1</td><td>7</td><td>$20$</td><td>$k=1$</td><td>`s` 只含有字符 <samp>'.'</samp> (即是空白的游戏行格)</td></tr><tr><td>2</td><td>3</td><td>$20$</td><td>无</td><td>`s` 只含有字符 <samp>'.'</samp></td></tr><tr><td>3</td><td>22</td><td>$100$</td><td>无</td><td>`s` 只含有字符 <samp>'.'</samp></td></tr><tr><td>4</td><td>27</td><td>$100$</td><td>无</td><td>`s` 只含有字符 <samp>'.'</samp> 及 <samp>'_'</samp> (只有关于填上了白色的方格信息)</td></tr><tr><td>5</td><td>21</td><td>$100$</td><td>无</td><td>无</td></tr><tr><td>6</td><td>10</td><td>$5000$</td><td>$100$</td><td>无</td></tr><tr><td>7</td><td>10</td><td>$200000$</td><td>$100$</td><td>无</td></tr></tbody></table></div>

<h2>评测方式</h2>
<p>评测程序将会按照下列格式读取输入数据：</p>
<ul><li>第一行：字符串 <code>s</code>，</li>
<li>第二行：整数 $k$，随后有 $k$ 个整数 $c_0, \ldots, c_{k - 1}$。</li>
</ul><p><a href="/faq">交互式类型的题目怎么本地测试</a></p>
<p><strong>时间限制：</strong>$2\texttt{s}$</p>
<p><strong>空间限制：</strong>$2\texttt{GB}$</p>
<h2>下载</h2>
<p><a href="./20678/file/attachment.zip">样例及测评库下载</a></p>
