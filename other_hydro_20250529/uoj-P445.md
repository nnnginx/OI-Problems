<p>这是一道<strong>交互题</strong>。</p>
<p>Old Pigeon是一名神仙OI选手，在鸽国信息学冬令营PWC2017 Challenge一题中仅用$1ms$就完成了第二个子任务——对于$2\times 10^8$个数排序，吊打了$std$。当ljt12138向他询问解题方法时，他总是笑而不语。</p>
<p>进入鸽华大学后，他遇到了这样一道数据结构课习题：给你$n$个数和一个三元比较器$compare(x, y, z)$，你可以给三元比较器三个数，它会将最大的数和最小的数返回给你，要求你用尽可能少的次数给$n$个数排序。看到这道似曾相识的题目，Old Pigeon变得暴躁了起来：“我有一只神奇的排序鸽，你给它不超过$k$个数，它就能将$k$个数返回给你，比三元比较器高到不知哪里去了！”</p>
<p>在PWC2017中获得狗牌的ljt12138想知道，如果你有一只这样的排序鸽，可以在多少次比较之内将$n$个数排序呢？</p>
<h2>任务介绍</h2>
<p>你需要实现一个函数<code>sort(int id, int n, int k, int *a)</code>：</p>
<ul><li>$1\le id\le 3$为传入的子任务编号；</li>
<li>$n$为序列长度；</li>
<li>$k$为排序鸽允许的最大排序个数；</li>
<li>$a$为传出答案的数组。</li>
</ul><p>你需要将排序后第$1\le i\le n$小的数<strong>在原数列中的位置</strong>$0\le p &lt; n$，存放到$a[i-1]$的位置。所有的下标都是从<strong>0</strong>开始的。</p>
<p>举例而言，如果待排序的数组$A = [3, 2, 0, 1, 4]$，排好序后的数组是$A' = [0, 1, 2, 3, 4]$，你应当返回的数组$a = [2, 3, 1, 0, 4]$。</p>
<p>在每个测试点中，交互库都会调用恰好一次<code>sort</code>函数。</p>
<p>你可以调用函数<code>super_sort(int *a, int len, int *b)</code>来请求排序鸽为你排序：</p>
<ul><li>$len$表示待排序的数的个数，要求$len \le k$；</li>
<li>$a$传入待排序的数<strong>在原数列中的位置</strong>，且$0\le a[i] &lt; n$；</li>
<li>$b$传出排好序的数<strong>在原数列中的位置</strong>，即$b$是$a$的一个排列，且对于任意的$i &lt; j$，$A[b[i]] &lt; A[b[j]]$。</li>
</ul><h2>实现方法</h2>
<p>本题只支持C++。</p>
<p>源代码中需要包含头文件<code>sort.h</code>。</p>
<p>你需要实现的函数<code>sort</code>：</p>
<pre><code class="sh_cpp">void sort(int id, int n, int k, int *a);</code></pre>
<p>函数<code>super_sort</code>的接口信息如下：</p>
<pre><code class="sh_cpp">void super_sort(int *a, int len, int *b);</code></pre>
<h2>如何测试你的程序</h2>
<p>你需要在本题目录下使用如下命令编译得到可执行程序：</p>
<pre><code class="sh_bash">g++ grader.cpp sort.cpp -o sort -O2</code></pre>
<p>可执行文件将从<strong>标准输入</strong>读取以下格式的数据：</p>
<ul><li><p>第一行包含六个数：$id, n, k, L1, L2, L4$，其中$1\le id\le 3$为子任务编号，$n$为排序数组长度，$k$为排序鸽每次能排序的最长长度，$L1, L2, L4$为评分参数，将在子任务中解释用处。</p>
</li>
<li><p>第二行包含$n$个数：$A_0, A_1, \dots, A_{n-1}$，表示待排序的数组。$A$应该是$\{0, 1, 2, \dots, n-1\}$的一个<strong>排列</strong>，表示待排序的数组。</p>
</li>
</ul><p>交互库将会输出以下信息：</p>
<ul><li>如果数组成功排序，输出一行形如"cmp_cnt = cnt"，表示你调用super_sort的次数</li>
<li>否则，将输出对应的错误信息。</li>
</ul><p>如果输入数据不合法，交互库可能不能正常运行。</p>
<p>你可以参考下发的交互库了解更多的信息。</p>
<p><a href="/faq">交互式类型的题目怎么本地测试</a></p>
<h2>样例源代码</h2>
<p>按照上文中提到的方式进行编译，即能通过编译得到可执行程序。</p>
<p>样例源代码只是帮助理解题目，结果<strong>不一定正确</strong>。</p>
<p>由于提供了交互式验证答案正确性的方法，本题不提供输出样例。</p>


<pre><code class="language-input1"><code>0 8 2 100 1000 10000
2 1 0 3 4 6 5 7</code>
</code></pre>
<p><strong>注意：</strong> 样例中的$id = 0$，在实际的测试数据中不会出现。这里仅用于演示输入的格式。</p>
<h2>限制及约定</h2>
<p>Subtask1（8分）：$n = 1024, k = 4, L1 = 5700, L2 = 10000, L4 = 100000$</p>
<p>Subtask2（24分）：$n = 1024, k = 16, L1 = 840, L2 = 1100, L4 = 3100$</p>
<p>Subtask3（68分）：$n = 524288, k = 16, L1 = 562000, L2 = 800000, L4 = 1016000$</p>
<p>对于每个子任务，设<code>c = cmp_cnt</code>：</p>
<ul><li>如果 $c \le L1$ ，将获得子任务全部的分数；</li>
<li>如果 $L1 &lt; c \le L2$，将获得子任务一半的分数；</li>
<li>如果 $L2 &lt; c \le L4$ ，将获得子任务四分之一的分数；</li>
<li>如果 $L4 &lt; c$ 或没有成功排序，将不会获得任何分数，并被暴躁的排序鸽D一番。</li>
</ul><p><strong>时间限制</strong>：$\texttt{2s}$</p>
<p><strong>空间限制</strong>：$\texttt{512MB}$</p>
<p>题目中所给的时间、空间限制为你的代码和交互库加起来可以使用的时间和空间。我们保证，对于任何合法的数据及在限制范围内的调用，任何版本的交互库（包括下发给选手的和最终评测使用的），运行所用的时间不会超过0.5s，运行所用的空间不会超过12MB，也就是说，选手实际可用的时间至少为<strong>1.5s</strong>，实际可用的空间至少为<strong>500MB</strong>。</p>
<h2>下载</h2>
<p><a href="./20850/file/attachment.zip">交互库下载</a></p>
