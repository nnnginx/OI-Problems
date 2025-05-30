<p>小 Z 正在自学量子计算机相关知识，最近他在研究量子通信章节，并遇到了一个有趣的问题。在该问题中，Alice 和 Bob 正在进行量子通信，它们的通信语言是一个大小为 $n$ 的字典 $S$，在该字典中，每一个单词 $s_i$（$1 \le i \le n$）都可以用一个 $\boldsymbol{256}$ <strong>位的</strong> $\boldsymbol{01}$ <strong>串</strong>来表示。在本题中 $s_i$ 可以通过调用函数 <code>gen</code> 来生成，选手可以在题目目录下的 <code>gen.cpp</code> 中查看，该函数的参数 <code>n</code>、<code>a1</code>、<code>a2</code> 将由输入数据给出。</p>
<p>Alice 和 Bob 接下来要进行 $m$ 次通信，每次通信由 Alice 向 Bob 传输<strong>恰好一个</strong>字典中的单词。然而，两人使用的通信信道并不可靠，会受到噪音的干扰。更具体地，对于第 $i$ 次传输，记 Alice 传输的原单词为 $x_i$，该 $01$ 串会受噪音干扰而<strong>翻转最多</strong> $\boldsymbol{k_i}$ <strong>位</strong>。换句话说，记 Bob 这次收到的 $01$ 串为 $y_i$，它与 $x_i$ 相比，可能有最多 $k_i$ 位是不同的，并且 $y_i$ 可能不在字典 $S$ 中出现。</p>
<p>与此同时，Bob 得知坏人 Eve 也潜入了两人的通信信道，并准备干扰两人的通信。他的干扰方式是将 Bob 收到的 $01$ 串变为任意的 $256$ 位 $01$ 串，并且这个串可能不在字典 $S$ 中出现。Eve 非常狡猾，他<strong>不一定</strong>会对每次通信都进行干扰。</p>
<p>现在 Bob 找来了你帮忙，对于接下来的每次通信，你需要根据 Bob 最终收到的 $01$ 串以及这次通信的噪音干扰阈值 $k_i$（$0 \le k_i \le 15$），判断这次通信是否有可能没有受到 Eve 的干扰（即 Bob 收到的 $01$ 串可以由字典中的某个单词翻转至多 $k_i$ 位后得到）。本次通信如果有可能没受到 Eve 干扰，请你输出 $1$，否则输出 $0$。Bob 很信任你的能力，所以你需要<strong>在线地回答结果，具体要求见输入格式</strong>。</p>
<p>为了降低读入用时， Bob 收到的串将用<strong>长度为</strong> $\boldsymbol{64}$ <strong>的</strong> $\boldsymbol{16}$ <strong>进制串</strong>给出，$16$ 进制串中包含数字字符 $\texttt{0} \sim \texttt{9}$ 与大写英文字母 $\texttt{A} \sim \texttt{F}$，其中字符 $\texttt{A} \sim \texttt{F}$ 依次表示数值 $10 \sim 15$。</p>
<p>$16$ 进制串可以逐位转化为 $01$ 串，例如：<code>5</code> 对应 <code>0101</code>，<code>A</code> 对应 <code>1010</code>，<code>C</code> 对应 <code>1100</code></p>
<p>注：$16$ 进制串 <code>AB</code> 对应的 $01$ 串是 <code>10101011</code>，其中第 $1$（下标从 $0$ 开始）个字符为 <code>0</code>。</p>
<h2>输入格式</h2>
<p>输入数据第一行包含四个非负整数 $n, m, a_1, a_2$，分别表示字典大小，通信次数，以及 <code>gen</code> 函数中参数 <code>a1</code> 和 <code>a2</code> 的初始值。</p>
<p>选手需要在自己的程序中调用题目描述中提到的 <code>gen</code> 函数生成单词表，选手可以复制并使用 <code>gen.cpp</code> 中的代码，程序中的布尔数组 <code>s[N+1][256]</code> 即为所有的单词。</p>
<p>接下来 $m$ 行，每行包含一个长度为 $64$ 的 $16$ 进制串和一个非负整数 $k_i$，分别表示第 $i$ 次通信 Bob 最终收到的 $01$ 串和噪音干扰阈值。</p>
<p>为了强制选手<strong>在线地回答询问</strong>，选手根据 $16$ 进制串还原出 $256$ 位 $01$ 串后，将 $01$ 串每一位异或上 ${\mathit{lastans}}$ 才能得到这次通信中 Bob 收到的真实 $01$ 串，其中 ${\mathit{lastans}} \in \{ 0, 1 \}$ 表示上一次询问的答案，第一个询问前 ${\mathit{lastans}}$ 初始值为 0。</p>
<p>注意：使用 <code>scanf</code> 和 <code>printf</code> 函数读入或输出 <code>unsigned long long</code> 类型变量时，对应的占位符为 <code>llu</code>。</p>
<h2>输出格式</h2>
<p>输出共 $m$ 行，每行一个整数 $0$ 或 $1$ 表示当前询问的答案。</p>
<h2>示例</h2>
<p>为了方便解释题意，我们使用了直接给出字典中单词、缩小单词长度为 $4$、允许离线地回答询问等方式，对简化的情况举例。</p>
<p>考虑字典大小为 $n = 2$，单词有 <code>1010</code> 和 <code>0111</code>。</p>
<p>对于询问 <code>B = 1011</code> 和 $k_1 = 1$，回答应该是 $1$，通过翻转 <code>1010</code> 的第 $4$ 位（从高位到低位，下同）得到。</p>
<p>对于询问 <code>1 = 0001</code> 和 $k_2 = 2$，回答应该是 $1$，通过翻转 <code>0111</code> 的第 $2$、$3$ 位得到。</p>
<p>对于询问 <code>1 = 0001</code> 和 $k_3 = 1$，回答应该是 $0$。</p>
<ul>
<li>翻转 <code>1010</code> 至多 $1$ 位可得 <code>1010</code>、<code>0010</code>、<code>1110</code>、<code>1000</code>、<code>1011</code>。</li>
<li>翻转 <code>0111</code> 至多 $1$ 位可得 <code>0111</code>、<code>1111</code>、<code>0011</code>、<code>0101</code>、<code>0110</code>。</li>
<li>无法得到 <code>1 = 0001</code>，它必定是由 Eve 干扰得到的。</li>
</ul>
<h2>样例一、样例二、样例三</h2>
<p>见样例数据下载。</p>
<h2>数据范围</h2>
<p>对于所有测试点：$1 \le n \le 4 \times {10}^5$，$1 \le m \le 1.2 \times {10}^5$，$0 \le k_i \le 15$，$a_1$ 和 $a_2$ 在 $[0, 2^{64} - 1]$ 之间均匀随机生成。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$n =$</th>
<th style="text-align:center;">$m =$</th>
<th style="text-align:center;">$k_i \le$</th>
<th style="text-align:center;">特殊性质</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$500$</td>
<td style="text-align:center;">$500$</td>
<td style="text-align:center;">$15$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">$0$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$2000$</td>
<td style="text-align:center;">$2000$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$5000$</td>
<td style="text-align:center;">$5000$</td>
<td style="text-align:center;">$15$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$10000$</td>
<td style="text-align:center;">$10000$</td>
<td style="text-align:center;">$15$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">$20000$</td>
<td style="text-align:center;">$20000$</td>
<td style="text-align:center;">$15$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">$100000$</td>
<td style="text-align:center;">$100000$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$9$</td>
<td style="text-align:center;">$400000$</td>
<td style="text-align:center;">$120000$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">$50000$</td>
<td style="text-align:center;">$50000$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$11$</td>
<td style="text-align:center;">$70000$</td>
<td style="text-align:center;">$70000$</td>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$12$</td>
<td style="text-align:center;">$100000$</td>
<td style="text-align:center;">$100000$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$13$</td>
<td style="text-align:center;">$30000$</td>
<td style="text-align:center;">$30000$</td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$14$</td>
<td style="text-align:center;">$60000$</td>
<td style="text-align:center;">$60000$</td>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$15$</td>
<td style="text-align:center;">$120000$</td>
<td style="text-align:center;">$120000$</td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$16$</td>
<td style="text-align:center;">$60000$</td>
<td style="text-align:center;">$60000$</td>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">所有询问串随机生成</td>
</tr>
<tr>
<td style="text-align:center;">$17$</td>
<td style="text-align:center;">$120000$</td>
<td style="text-align:center;">$120000$</td>
<td style="text-align:center;">$12$</td>
<td style="text-align:center;">所有询问串随机生成</td>
</tr>
<tr>
<td style="text-align:center;">$18$</td>
<td style="text-align:center;">$400000$</td>
<td style="text-align:center;">$100000$</td>
<td style="text-align:center;">$15$</td>
<td style="text-align:center;">所有询问串随机生成</td>
</tr>
<tr>
<td style="text-align:center;">$19$</td>
<td style="text-align:center;">$30000$</td>
<td style="text-align:center;">$30000$</td>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$20$</td>
<td style="text-align:center;">$60000$</td>
<td style="text-align:center;">$60000$</td>
<td style="text-align:center;">$9$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$21$</td>
<td style="text-align:center;">$90000$</td>
<td style="text-align:center;">$90000$</td>
<td style="text-align:center;">$11$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$22$</td>
<td style="text-align:center;">$200000$</td>
<td style="text-align:center;">$120000$</td>
<td style="text-align:center;">$12$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$23$</td>
<td style="text-align:center;">$400000$</td>
<td style="text-align:center;">$80000$</td>
<td style="text-align:center;">$15$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$24$</td>
<td style="text-align:center;">$400000$</td>
<td style="text-align:center;">$100000$</td>
<td style="text-align:center;">$15$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$25$</td>
<td style="text-align:center;">$400000$</td>
<td style="text-align:center;">$120000$</td>
<td style="text-align:center;">$15$</td>
<td style="text-align:center;">无</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\require{cancel}\cancel{\texttt{2s}}\texttt{3s}$</strong></p>
<p><strong>空间限制：$\texttt{384MB}$</strong></p>
