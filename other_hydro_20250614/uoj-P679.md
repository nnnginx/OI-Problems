<p>你现在要把一个由 <code>01</code> 组成的比特串编码为一张 $M=100$ 个顶点的无标号无向图，并且需要在图的点和边随机打乱之后仍然恢复出这个比特串。此外，你需要让这个比特串尽可能长。</p>
<h2>评测方式</h2>
<p>你需要提交<strong>一个</strong>程序。你的程序需要支持三个运行模式 <code>N, A, B</code>，分别表示输出比特串长度、加密、解密。<strong>每次加密或解密时，你的程序都会被重新执行。</strong></p>
<p>首先评测程序会将单个字母 <code>N</code> 作为输入运行你的程序，你需要输出一个正整数 $n$，表示你能编码的比特串最长有多长。出于一些原因，我们知道这个长度不会超过 $5000$。</p>
<p>然后，以下过程会被执行若干次：</p>
<ul>
<li>评测程序会运行你的程序，输入两行，第一行是单个字母 <code>A</code>，第二行是一个长度为 $n$ 的比特串。你需要输出一张 $M$ 个顶点的无向图，具体格式见下文。</li>
<li>评测程序会打乱这张无向图的点标号和边标号。</li>
<li>评测程序会重新运行你的程序，输入若干行，第一行是单个字母 <code>B</code>，第二行及以后表示一张 $M$ 个顶点的无向图。你的程序需要输出一个长度为 $n$ 的比特串，且输出串需要和这一轮最开始输入的串相同。</li>
</ul>
<p>上述的无向图的格式如下：首先一行一个整数 $e$，表示图的边数（我们知道图的点数固定为 $M=100$）；此后 $e$ 行每行两个整数 $u_i, v_i$，表示一条无向边。我们不允许 $u_i=v_i$。图的下标从 $1$ 开始。</p>
<h2>范例代码与执行过程</h2>
<p>例如，假设你写了这样的程序：</p>
<pre><code class="sh_cpp">#include &lt;bits/stdc++.h&gt;
using namespace std;
int main() {
  int n = 1;
  string s;
  cin &gt;&gt; s;
  if (s == "N") {
    cout &lt;&lt; n &lt;&lt; endl;
  } else if (s == "A") {
    string z;
    cin &gt;&gt; z;
    if (z == "0") {
      cout &lt;&lt; 0 &lt;&lt; endl;
    } else {
      cout &lt;&lt; 1 &lt;&lt; endl;
      cout &lt;&lt; 1 &lt;&lt; ' ' &lt;&lt; 2 &lt;&lt; endl;
    }
  } else if (s == "B") {
    int e;
    cin &gt;&gt; e;
    if (e == 0) {
      cout &lt;&lt; "0" &lt;&lt; endl;
    } else if (e == 1) {
      cout &lt;&lt; "1" &lt;&lt; endl;
    }
  }
}</code></pre>
<p>这个程序会把长度为 $1$ 的两个比特串 <code>0</code>，<code>1</code> 分别加密为空图和只有一条 $(1,2)$ 边的图。上述算法按照下面的给分方式可以获得 $1$ 分。</p>
<p>交互库会先运行该程序，将 <code>N</code> 输入进去，得到长度 $n=1$，然后会运行若干次，每次把以下两个输入：</p>
<pre><code class="sh_plain">A
0</code></pre>
<p>或</p>
<pre><code class="sh_plain">A
1</code></pre>
<p>输入该程序，该程序会分别输出</p>
<pre><code class="sh_plain">0</code></pre>
<p>或</p>
<pre><code class="sh_plain">1
1 2</code></pre>
<p>对于这两种图，评测器会试图将它们点边打乱；当然打乱空图毫无意义。该程序会再次被执行，以下面的内容为输入：</p>
<pre><code class="sh_plain">B
0</code></pre>
<p>或</p>
<pre><code class="sh_plain">B
1
11 45</code></pre>
<p>或者一些别的什么数字；该程序当然会正确恢复出原来的两个一位比特串。</p>
<h2>给分方式</h2>
<p>该题目与常见算法竞赛题目有显著不同，因此有奇妙的给分方式。首先，我们鼓励你写保证正确性的算法，因此在这些测试中，解密错误哪怕一次都会有较高的惩罚；其次，你能加密的比特串越长越好。</p>
<p>假设在 $100$ 组测试中你犯错了 $u$ 次，且你的程序能加密的比特串长度为 $n$，则你的分数</p>
<p>$$
\mathrm{score} = \left\lfloor\frac{f(u)}{f(0)}g(x)\right\rfloor,
$$</p>
<p>其中</p>
<p>$$
f(u)=\max{\left(\frac{1}{1+u}-\frac{1}{51},0\right)}
$$</p>
<p>是对你的解密犯错的惩罚次数：换言之，你哪怕犯错一次都会让分数下降大约一半。</p>
<p>$$
g(x)=
\begin{cases}
x,&amp;0 &lt; x\le10\\
2\sqrt{x-9}+8,&amp;10 &lt; x\le130\\
2\sqrt[3]{x-103}+24,&amp;130 &lt; x\le2300\\
-6\log_2\left(4348-x\right)+116,&amp;2300 &lt; x\le4092\\
\frac{x}{8}-\frac{887}{2},&amp;4092 &lt; x\le4348\\
100,&amp;4348 &lt; x\le4355\\
x-4255,&amp;x &gt; 4355
\end{cases}
$$</p>
<p>是对你能加密的比特串的长度的奖励。注意，不要被这个式子的长度给吓到；这是一个单调的函数，这里有几个特殊值可以给你参考：$g(10)=10,g(130)=30,g(2300)=50,g(4092)=68,g(4348)=100$。在 $[0,4355]$ 这个范围内，它大概长这样：</p>
<p><img src="https://img.uoj.ac/problem/679/sp20210730_234256_975.png" alt="函数图像" class="img-responsive center-block"></p>
<h2>自测程序</h2>
<p>你可以使用<a href="https://paste.ubuntu.com/p/VvFHtWmjH5/">这份程序</a>来在本地对你的代码进行测试。</p>
<h2>致谢</h2>
<p>这道题目归功于 <a href="https://uoj.ac/user/profile/kczno1">kczno1</a> 同学。感谢 <a href="https://mcfx.moe/">mcfx</a> 同学提供的打爆标程的<a href="https://mcfxmcfx.blog.uoj.ac/blog/7279">题解</a>。感谢 UOJ 各位管理员群友帮我按后台的按钮。</p>
