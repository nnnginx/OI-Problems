<h2>题目背景</h2>
<p>有一天你在翻 OJ 时，发现了几道有趣的题。你还发现 OJ 上多出了一种语言—— HackVM。于是你打算用 HackVM 过掉这几道题。</p>
<h2>题目描述</h2>
<p>在 HackVM 语言中，一个字符就是一个操作，一个程序就是一个字符串。这个语言的程序从字符串的第一个字符开始运行，运行完毕后移动到下一个字符，直到运行至字符串尾或遇到了运行时错误而终止，或者执行了特定的终止程序的操作。为了防止死循环，若没有特殊规定，则最多执行 $10^7$ 次操作。另外，将当前运行到的位置称为 $PC$。这个语言拥有一个操作数栈，一个内存，一个调用栈，它们均以 <code>long long</code>（$64$ 位有符号整数）为单位，即一个基本块可以存放一个 <code>long long</code>——所有的运算均是基于 <code>long long</code> 的（若你的运算过程中使用了超过 <code>long long</code> 的数，则不保证答案正确性，校验器可能会检测并报错）。其中内存有 $2097152$ 个基本块，从 $0$ 开始标号。</p>
<p>初始时，操作数栈、调用栈均为空，内存的所有块均初始化为 $0$。</p>
<h2>操作描述</h2>
<p>我们假设 $S_i$ 为该操作执行前操作数栈顶的第 $i+1$ 个块中的内容。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-verticle-middle"><thead><tr><th>操作</th><th>描述</th>
</tr></thead><tbody><tr><td><samp>' '</samp></td><td>什么都不做（计算进代码长度）</td></tr><tr><td><samp>'p'</samp></td><td>弹出 $S_0$ 并将 $S_0$ 作为 `long long` 输出</td></tr><tr><td><samp>'P'</samp></td><td>弹出 $S_0$ 并将 $S_0$ 作为字符输出</td></tr><tr><td><samp>'r'</samp></td><td>输入一个整数并压入操作数栈</td></tr><tr><td><samp>'R'</samp></td><td>输入一个字符并压入操作数栈</td></tr><tr><td><samp>'0'</samp></td><td>将数字 $0$ 压入操作数栈</td></tr><tr><td><samp>'1'</samp></td><td>将数字 $1$ 压入操作数栈</td></tr><tr><td><samp>'2'</samp></td><td>将数字 $2$ 压入操作数栈</td></tr><tr><td><samp>'3'</samp></td><td>将数字 $3$ 压入操作数栈</td></tr><tr><td><samp>'4'</samp></td><td>将数字 $4$ 压入操作数栈</td></tr><tr><td><samp>'5'</samp></td><td>将数字 $5$ 压入操作数栈</td></tr><tr><td><samp>'6'</samp></td><td>将数字 $6$ 压入操作数栈</td></tr><tr><td><samp>'7'</samp></td><td>将数字 $7$ 压入操作数栈</td></tr><tr><td><samp>'8'</samp></td><td>将数字 $8$ 压入操作数栈</td></tr><tr><td><samp>'9'</samp></td><td>将数字 $9$ 压入操作数栈</td></tr><tr><td><samp>'+'</samp></td><td>弹出 $S_0,S_1$ 并将 $S_1+S_0$ 压入操作数栈</td></tr><tr><td><samp>'-'</samp></td><td>弹出 $S_0,S_1$ 并将 $S_1-S_0$ 压入操作数栈</td></tr><tr><td><samp>'\*'</samp></td><td>弹出 $S_0,S_1$ 并将 $S_1*S_0$ 压入操作数栈</td></tr><tr><td><samp>'/'</samp></td><td>弹出 $S_0,S_1$ 并将 $S_1/S_0$ 压入操作数栈</td></tr><tr><td><samp>':'</samp></td><td>弹出 $S_0,S_1$，若 $S_1&lt;S_0$ 则压入 $-1$，若 $S_1=S_0$ 则压入 $0$，若 $S_1&gt;S_0$ 则压入 $1$</td></tr><tr><td><samp>'g'</samp></td><td>弹出 $S_0$ 并将 $PC$ 加上 $S_0$</td></tr><tr><td><samp>'?'</samp></td><td>弹出 $S_0,S_1$，若 $S_1=0$ 则将 $PC$ 加上 $S_0$</td></tr><tr><td><samp>'c'</samp></td><td>将当前 $PC$ 压入调用栈，弹出 $S_0$ 并将 $PC$ 设为 $S_0$</td></tr><tr><td><samp>'$'</samp></td><td>将 $PC$ 设为调用栈栈顶，并将调用栈弹栈</td></tr><tr><td><samp>'&lt;'</samp></td><td>弹出 $S_0$ 并将标号为 $S_0$ 的内存中的内容压入操作数栈</td></tr><tr><td><samp>'&gt;'</samp></td><td>弹出 $S_0,S_1$ 并将 $S_1$ 存在标号为 $S_0$ 的内存中</td></tr><tr><td><samp>'^'</samp></td><td>弹出 $S_0$ 后，将 $S_{S_0+1}$ 压入操作数栈（如代码段 0^ 会将之前的 $S_0$ 复制一份）</td></tr><tr><td><samp>'v'</samp></td><td>弹出 $S_0$ 与 $S_{S_0+1}$ 后将后者重新压入操作数栈（如代码段 1v 会将之前的 $S_0$ 与 $S_1$ 交换）</td></tr><tr><td><samp>'d'</samp></td><td>弹出 $S_0$</td></tr><tr><td><samp>'!'</samp></td><td>终止程序</td></tr></tbody></table></div>

<p>样例、具体实现以及可执行代码可以参考解释器 <samp>hackvm.cpp</samp>。</p>
<h2>任务</h2>
<h4>测试点 1（3 分）</h4>
<p>输入两个整数 $a,b$，输出 $a+b$。</p>
<h4>测试点 2（5 分）</h4>
<p>输入两个正整数 $a,b$，输出 $a\mod b$。</p>
<h4>测试点 3（8 分）</h4>
<p>输入三个整数 $a,b,c(1\le a,b,c&lt; 2^{31})$，输出 $a^b\mod c$。</p>
<h4>测试点 4、5（各 7 分）</h4>
<p>第一行给出一个奇数 $n(1\le n\le 100)$。</p>
<p>接下来给出 $n$ 个整数。</p>
<p>输出这 $n$ 个数的中位数。</p>
<h4>测试点 6、7（各 9 分）</h4>
<p>给一个无向图，求 $1$ 号点到每个点的最短路。</p>
<p>第一行给出 $n,m(1\le n\le 40,1\le m\le 500)$，表示点数和边数。</p>
<p>接下来 $m$ 行，每行三个整数 $u,v,w$，表示 $u$ 到 $v$ 有一条权值为 $w$（$0\le w\le 10^9$）的边。</p>
<p>输出 $1$ 号点到每个点的最短路之和（结果可能会超过 <code>int</code>）。</p>
<p>保证没有重边和自环，点从 $1$ 开始标号。</p>
<h4>测试点 8、9（各 13 分）</h4>
<p>给一个有向图，求强联通分量个数。</p>
<p>第一行给出 $n,m(1\le n\le 100,1\le m\le 3000)$，表示点数和边数。</p>
<p>接下来 $m$ 行，每行两个整数 $u,v$，表示 $u$ 到 $v$ 有一条边。</p>
<p>输出答案。</p>
<p>保证没有重边和自环，点从 $1$ 开始标号。</p>
<h4>测试点 10（12 分）</h4>
<p>你需要输出程序本身（即实现一个 Quine 程序）。</p>
<p>注意代码长度不能为 0。</p>
<h4>测试点 11（14 分）</h4>
<p>给一段 HackVM 代码，你需要运行这段代码并输出其结果。</p>
<p>保证没有 <code>r</code> <code>R</code> <code>P</code> 操作，且 <code>p</code> 只会调用一次。保证会调用 <code>!</code> 退出。</p>
<p>保证这段程序使用的操作数不高于 60000 且内存使用不多于 65536，没有行末换行，你需要读到 EOF（-1）为止。</p>
<h2>提示</h2>
<p>你的程序应在对应的 <code>data*.out</code> 中，其中 <code>*</code> 是对应的测试点编号，每一个程序应仅有一行，程序及输出的结尾<strong>不应</strong>有换行或者多余的空格（空格虽然为空操作，但会被计入代码长度）。</p>
<p>对于测试点 10 以外的测试点，你<strong>不能</strong>使用 <code>P</code> 操作（只需要输出一个整数）；而对于测试点 10，你<strong>不能</strong>使用 <code>p</code> 操作，且你的输出<strong>不能</strong>包含多余的换行符或空格。</p>
<p>所有程序的代码长度应该在 1B 到 50KB 之间。保证所有<strong>输入</strong>的数都在 <code>int</code> 范围内。每个测试点均只包含<strong>一组</strong>数据。上面写在一起的测试点，并<strong>没有</strong>捆绑。</p>
<h2>下载</h2>
<p><a href="./20837/file/attachment.zip">解释器下载</a></p>
<p>这个解释器，无疑是善良的出题人无私的馈赠。这个解释器涵盖了 Hackvm 中所有操作的实现。你可以利用这个解释器，对自己的程序进行全面的检查。足量的操作组数和多种多样的错误提示，能让程序中的错误无处遁形。出题人相信，这个美妙的解释器，可以给拼搏于 AC 这道题的逐梦之路上的你，提供一个有力的援助。</p>
