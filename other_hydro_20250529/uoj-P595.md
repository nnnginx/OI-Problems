<p>太阳神为了体察凡间人情，化名 <span class="uoj-username" data-rating="1797">EntropyIncreaser</span> 下凡。<span class="uoj-username" data-rating="1797">EntropyIncreaser</span>，也就是 EI，合起来写就是日，意思是太阳神。</p>
<p>今天，<span class="uoj-username" data-rating="1797">EntropyIncreaser</span> 召集了粉丝群里的 $n$ 名群员来参与他的盛宴。宴会上，他和群员们玩起了益智游戏，以展示自己无量的智慧。</p>
<p>游戏的一方是 <span class="uoj-username" data-rating="1797">EntropyIncreaser</span>；另一方是 $n$ 名群员，他们排成了一行，依次编号为 $1, 2, \ldots, n$。字符集是前 $k$ 个英文字母集合 $\Sigma$，也就是说，游戏中所有字符串均由 $\Sigma$ 的元素构成。</p>
<p>游戏一开始，<span class="uoj-username" data-rating="1797">EntropyIncreaser</span> 给每个群员都发了一个字符串，第 $i$ 个群员的字符串是 $S_i$。随后，每个群员都任意地从收到的字符串 $S_i$ 中挑选一个子串 $T_i$（子串必须连续，但可以为空串）。群员们把各自所挑选的子串 $T_i$ 输入打字机，它们按照顺序没有间隔地接成了一个完整的字符串 $T=T_1T_2\cdots T_n$。<span class="uoj-username" data-rating="1797">EntropyIncreaser</span> 只能知道 $T$，而不知道每个字符是哪位群员输入的。游戏的规则是，只要解出一组可能的 $T_1, T_2, \ldots, T_n$，就能获得胜利。</p>
<p><span class="uoj-username" data-rating="1797">EntropyIncreaser</span> 看到字符串 $T$，不假思索，将它划分成 $n$ 个字符串 $T'_1T'_2\cdots T'_n$（同样可以为空）。群员们惊奇地发现，$T'_i$ 确实是他们所收到的串 $S_i$ 的子串！</p>
<p><span class="uoj-username" data-rating="1797">EntropyIncreaser</span> 笑笑：『这是一道大水题，没什么难的。我们来加大一点儿难度。』</p>
<p>这时月亮女神玲雨提出了游戏的加强版。</p>
<p>现在第 $i$ 位群员仍然取出了子串 $T_i$。在每位群员输入前，键盘的键位都会被秘密打乱，而群员仍然照常输入，也就是每位群员现在分配了一个 $\Sigma$ 上的置换 $f_i$，$T_i$ 的第 $j$ 个字符 $T_{ij}$ 输入时将变成 $f_i(T_{ij})$，所有输入的字符连接起来构成了 $T$。<span class="uoj-username" data-rating="1797">EntropyIncreaser</span> 的目标仍然是解出一组可能的 $T_1, T_2, \ldots, T_n$。</p>
<p><span class="uoj-username" data-rating="1797">EntropyIncreaser</span> 仔细端详，再次将 $T$ 分成了 $n$ 个字符串 $T'_1, T'_2, \ldots, T'_n$，群员们沸腾了：确实存在置换 $f_i$，使得 $S_i$ 的一个子串经过 $f_i$ 的作用得到 $T'_i$！</p>
<p>宴会从清晨进行到夜晚。在宴会的尾声，<span class="uoj-username" data-rating="1797">EntropyIncreaser</span> 宣布：『神将赐予群友数学的智慧，但是要先经过三道考验。』</p>
<p>现在，来自计数之神大加强的第一道考验摆在了你面前——请你来数一数，在最后一个游戏中，有多少个字符串 $T$ 有至少一组解？答案可能很大，所以对 $998244353$ 取模。</p>
<h2>输入格式</h2>
<p>第一行两个正整数 $n, k$。</p>
<p>接下来 $n$ 行，每行一个字符串，依次表示 $S_1, S_2, \ldots, S_n$。</p>
<h2>输出格式</h2>
<p>输出有解的字符串的数量，对 $998244353$ 取模。</p>


<pre><code class="language-input1">2 2
aa
a
</code></pre>


<pre><code class="language-output1">11
</code></pre>


<p>用 $\epsilon$ 指代空串。</p>
<p>$S_1$ 的子串有 $\epsilon$, <code>a</code>, <code>aa</code>，打乱键位后可获得 $\epsilon$, <code>a</code>, <code>b</code>, <code>aa</code>, <code>bb</code>。</p>
<p>$S_2$ 的子串有 $\epsilon$, <code>a</code>，打乱键位后可获得 $\epsilon$, <code>a</code>, <code>b</code>。</p>
<p>连接起来，有解的串有：$\epsilon$, <code>a</code>, <code>b</code>, <code>aa</code>, <code>ab</code>, <code>ba</code>, <code>bb</code>, <code>aaa</code>, <code>aab</code>, <code>bba</code>, <code>bbb</code>。</p>


<pre><code class="language-input2">2 2
aa
ab
</code></pre>


<pre><code class="language-output2">17
</code></pre>

<h2>限制与约定</h2>
<p>简记 $L=\sum_{i=1}^n|S_i|$。</p>
<p>保证 $2 \le k \le 26$，$S_i$ 非空，$L \le 10^6$。</p>
<p>子任务一（2分）：$n=1$，$k=2$，$L \le 1000$。</p>
<p>子任务二（7分）：$n=1$，$L \le 1000$。</p>
<p>子任务三（11分）：$n=1$，$L \le 10^5$。</p>
<p>子任务四（13分）：$k=2$，$L \le 1000$。</p>
<p>子任务五（17分）：$L \le 1000$。</p>
<p>子任务六（31分）：$k \le 5$。</p>
<p>子任务七（19分）：无特殊限制。</p>
<p><strong>时间限制</strong>：$3\texttt{s}$</p>
<p><strong>空间限制</strong>：$2048\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="https://uoj.ac/download.php?type=problem&amp;id=595">样例数据下载</a></p>
