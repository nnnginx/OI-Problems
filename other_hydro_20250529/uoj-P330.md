<p>小明正在学习一种新的编程语言 A++ ，刚学会循环语句的他激动地写了好多程序并给出了他自己算出的时间复杂度，可他的编程老师实在不想一个一个检查小明的程序，于是你的机会来啦！下面请你编写程序来判断小明对他的每个程序给出的时间复杂度是否正确。</p>
<p>A++ 语言的循环结构如下：</p>
<pre>F i x y
    循环体
E</pre><p>其中“<samp>F i x y</samp>”表示新建变量 $i$（$i$ 变量 $i$ 不可与未被销毁的变量重名）并初始化为 $x$，然后判断 $i$ 和 $y$ 的大小关系，若 $i$ 小于等于 $y$ 则进入循环，否则不进入。每次循环结束后 $i$ 都会被修改成 $i +1$，一旦 $i$ 大于 $y$ 终止循环。</p>
<p>$x$ 和 $y$ 可以是正整数（$x$ 和 $y$ 的大小关系不定）或变量 $n$。$n$ 是一个表示数据规模的变量，在时间复杂度计算中需保留该变量而不能将其视为常数，该数远大于 $100$。</p>
<p>“<samp>E</samp>”表示循环体结束。循环体结束时，这个循环体新建的变量也被销毁。</p>
<p>注：本题中为了书写方便，在描述复杂度时，使用大写英文字母“<samp>O</samp>”表示通常意义下“$\Theta$”的概念。</p>
<h2>输入格式</h2>
<p>输入文件第一行一个正整数 $t$，表示有 $t$（$t \le 10$）个程序需要计算时间复杂度。每个程序我们只需抽取其中“<samp>F i x y</samp>”和“<samp>E</samp>”即可计算时间复杂度。注意：循环结构允许嵌套。</p>
<p>接下来每个程序的第一行包含一个正整数 $L$ 和一个字符串，$L$ 代表程序行数，字符串表示这个程序的复杂度，“<samp>O(1)</samp>”表示常数复杂度，“<samp>O(n^w)</samp>”表示复杂度为 $n^w$，其中 $w$ 是一个小于 $100$ 的正整数（输入中不包含引号），输入保证复杂度只有 <samp>O(1)</samp> 和 <samp>O(n^w)</samp> 两种类型。</p>
<p>接下来 $L$ 行代表程序中循环结构中的“<samp>F i x y</samp>”或者 “<samp>E</samp>”。</p>
<p>程序行若以“<samp>F</samp>”开头，表示进入一个循环，之后有空格分离的三个字符（串）<samp>i x y</samp>，其中 $i$ 是一个小写字母（保证不为“<samp>n</samp>”），表示新建的变量名，$x$ 和 $y$ 可能是正整数或 <samp>n</samp> ，已知若为正整数则一定小于 $100$ 。</p>
<p><strong>注意在第10组数据中可能存在变量名为<samp>n</samp>的情况，这与之前的描述不符。</strong></p>
<p>程序行若以“<samp>E</samp>”开头，则表示循环体结束。</p>
<h2>输出格式</h2>
<p>输出文件共 $t$ 行，对应输入的 $t$ 个程序，每行输出“<samp>Yes</samp>”或“<samp>No</samp>”或者“<samp>ERR</samp>”（输出中不包含引号），若程序实际复杂度与输入给出的复杂度一致则输出“<samp>Yes</samp>”，不一致则输出“<samp>No</samp>”，若程序有语法错误（其中语法错误只有: ① <samp>F</samp> 和 <samp>E</samp> 不匹配 ②新建的变量与已经存在但未被销毁的变量重复两种情况），则输出“<samp>ERR</samp>”。</p>
<p>注意：即使在程序不会执行的循环体中出现了语法错误也会编译错误，要输出“<samp>ERR</samp>”。</p>


<pre><code class="language-input1">8
2 O(1)
F i 1 1
E
2 O(n^1)
F x 1 n
E
1 O(1)
F x 1 n
4 O(n^2)
F x 5 n
F y 10 n
E
E
4 O(n^2)
F x 9 n
E
F y 2 n
E
4 O(n^1)
F x 9 n
F y n 4
E
E
4 O(1)
F y n 4
F x 9 n
E
E
4 O(n^2)
F x 1 n
F x 1 10
E
E
</code></pre>


<pre><code class="language-output1">Yes
Yes
ERR
Yes
No
Yes
Yes
ERR
</code></pre>


<p>第一个程序 <samp>i</samp> 从 $1$ 到 $1$ 是常数复杂度。</p>
<p>第二个程序 <samp>x</samp> 从 $1$ 到 $n$ 是 $n$ 的一次方的复杂度。</p>
<p>第三个程序有一个 <samp>F</samp> 开启循环却没有 <samp>E</samp> 结束，语法错误。</p>
<p>第四个程序二重循环，$n$ 的平方的复杂度。</p>
<p>第五个程序两个一重循环，$n$ 的一次方的复杂度。</p>
<p>第六个程序第一重循环正常，但第二重循环开始即终止（因为 $n$ 远大于 $100$，$100$ 大于 $4$）。</p>
<p>第七个程序第一重循环无法进入，故为常数复杂度。</p>
<p>第八个程序第二重循环中的变量 <samp>x</samp> 与第一重循环中的变量重复，出现语法错误②，输出 <samp>ERR</samp>。</p>
<h2>样例二</h2>
<p>见样例数据下载。</p>
<h2>限制与约定</h2>
<p>对于30%的数据：不存在语法错误，数据保证小明给出的每个程序的前 $L/2$ 行一定为以 <samp>F</samp> 开头的语句，第 $L/2+1$ 行至第 $L$ 行一定为以 <samp>E</samp> 开头的语句，$L \le 10$，若 $x$、$y$ 均为整数，$x$ 一定小于 $y$，且只有 $y$ 有可能为 <samp>n</samp>。</p>
<p>对于50%的数据：不存在语法错误，$L \le 100$，且若 $x$、$y$ 均为整数，$x$ 一定小于 $y$，且只有 $y$ 有可能为 <samp>n</samp>。</p>
<p>对于70%的数据：不存在语法错误，$L\le 100$。</p>
<p>对于100%的数据：$L \le 100$。</p>
<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20756/file/attachment.zip">样例数据下载</a></p>
