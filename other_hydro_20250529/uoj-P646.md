<p><strong>这是一道交互题</strong></p>
<p>蒜斜有一个神秘的随机数生成器 $A$。其工作原理如下：</p>
<p>$A$ 中有 $100$ 个类型为 unsigned long long 的变量，编号为 $0 \sim 99$。这其中编号 $0 \sim m-1$ 的变量与生成的随机数有关。</p>
<p>每一次初始化 $A$ 的时候，$A$ 都会独立随机的生成一段代码来生成随机数，代码规则如下：</p>
<ul>
<li>编号为 $0 \sim m-1$ 的变量为特殊变量，他们的值在一轮随机过程后不会被清空。其余变量的值会被清零。</li>
<li>一轮程序由不超过 $10^4$ 条赋值语句组成和恰好一条返回语句组成，赋值语句种类如下：<ul>
<li>$a = b\ \mathrm{xor}\ c$，其中 $a$ 为一变量，$b,c$ 为一$[0,2^{64})$整数常数或者变量</li>
<li>$a = b\ \mathrm{&lt;&lt;}\ c$，其中 $a$ 为一变量，$\mathrm{&lt;&lt;}$ 为二进制左移操作，$b$ 为一$[0,2^{64})$整数常数或者变量, $c$ 为一个 $0 \sim 63$ 的整数常数</li>
<li>$a = b\ \mathrm{&gt;&gt;}\ c$，其中 $a$ 为一变量，$\mathrm{&gt;&gt;}$ 为二进制右移操作，$b$ 为一$[0,2^{64})$整数常数或者变量, $c$ 为一个 $0 \sim 63$ 的整数常数</li>
<li>$a = b\ \mathrm{and}\ c$，其中 $a$ 为一变量，$b$ 为一$[0,2^{64})$整数常数或者变量, $c$ 为一$[0,2^{64})$整数常数</li>
<li>$a = b\ \mathrm{or}\ c$，其中 $a$ 为一变量，$b$ 为一$[0,2^{64})$整数常数或者变量, $c$ 为一$[0,2^{64})$整数常数</li>
<li>这里保证，如果在某一次运算中出现了编号为 $m \sim 99$ 的变量，则其要不为被赋值对象 $a$，要不在先前的计算中已经被赋值。</li>
</ul>
</li>
<li>返回语句形如 $\mathrm{return}\ a$，其中 $a$ 为一变量，其作为这一轮程序运行后生成的随机数的值。蒜斜保证这一条返回语句是每一轮程序运行时候最后一个语句。且返回的变量 $a$ 满足其编号小于 $m$ 或者 $a$ 在执行时进行过至少一次赋值操作。</li>
<li>程序初始化时蒜斜会手动设定变量 $0 \sim m-1$ 的值。</li>
<li>蒜斜保证生成每一轮执行的代码片段完全相同。 </li>
</ul>
<p>蒜斜给他的程序加了密，于是任何人无法访问这个随机数生成器中生成的任何中间变量的值，也不知道蒜斜设定的 $m$ 个初始值，以及蒜斜随机数生成器的程序。蒜斜觉得他的程序可以输出一个超级随机的序列，这个序列无法被预知。</p>
<p>你是一名大预言家，你打算采用一些奇怪的占星术，预言蒜斜的程序在若干轮后的输出结果。</p>
<h2>交互格式</h2>
<p>本题只支持 <code>c++</code>。</p>
<p>你需要包含头文件 <code>interactor.h</code>。</p>
<p>你不需要，也不应该实现主函数，你只需要实现如下两个函数：</p>
<ol>
<li><code>void solve(int m)</code>：<ul>
<li>你可以在这个函数内调用若干次蒜斜的随机数生成器 $A$。</li>
<li>参数 $m$ 含义如题面所示。</li>
<li>这个函数没有返回值。</li>
</ul>
</li>
<li><code>unsigned long long query(int x)</code>：<ul>
<li>蒜斜在已经结束的所有操作的基础上，又执行了恰好 $x$ 次随机数生成器 $A$.</li>
<li>你需要返回最后一次调用操作后，随机数生成器返回的结果。</li>
<li>蒜斜 保证 $1 \le x \le 10^9$</li>
</ul>
</li>
</ol>
<p>你可以通过如下函数调用蒜斜的随机数生成器</p>
<ol>
<li><code>unsigned long long random_ull()</code>：<ul>
<li>蒜斜 执行了恰好 $1$ 次随机数生成器 $A$.</li>
<li>返回这一次操作后随机数生成器返回的结果。</li>
<li>注意<strong>在执行 <code>query</code> 时你无法调用该操作</strong>。也就是说，这个操作仅能在执行 <code>solve</code> 时执行。</li>
</ul>
</li>
</ol>
<p>由于蒜斜的耐心有限，你至多只能调用 $K$ 次 蒜斜 的随机数生成器。也就是说你至多只能调用 $K$ 次 <code>random_ull</code>，且仅仅能在 <code>solve</code> 中调用。</p>
<p><strong>本题保证所使用的程序以及询问的值在交互开始之前已经完全确定，不会根据和你的程序的交互过程动态构造，因此题目中的交互操作都是确定性的，你不需要关心这些操作在交互库中的具体实现。</strong></p>
<p><strong>数据保证在调用次数限制下，交互库运行所需的时间不超过 0.5s；交互库使用的内存大小固定，且不超过 128MB。</strong></p>
<h2>测试程序方式</h2>
<p><strong>试题目录下的 <code>grader.cpp</code>  是我们提供的交互库参考实现，最终测试时所用的交互库实现与该参考实现有所不同，因此选手的解法不应该依赖交互库实现。</strong></p>
<ol>
<li>你需要在本题目录下使用如下命令编译得到可执行程序：<ul>
<li><code>g++ grader.cpp sample.cpp -o sample -O2 -lm</code></li>
</ul>
</li>
<li>对于编译得到的可执行程序：<ul>
<li>可执行文件将从<strong>标准输入</strong>读入以下格式的数据：<ul>
<li>第一行包含三个整数 $m,K,Q$。</li>
<li>接下来 $Q$ 行，一行一个正整数，表示一次 蒜斜 的询问。</li>
</ul>
</li>
<li>读入完成之后，交互库将调用恰好一次函数 $\texttt{solve}$，和 $Q$ 次函数 $\texttt{query}$ 你的函数正确返回后，交互库会判断你的计算是否正确，若正确则会输出 <code>Correct</code> 和交互函数调用次数相关信息，否则会输出相应的错误信息。</li>
</ul>
</li>
</ol>
<p>试题目录下有出题人提供的一份参考代码 <code>sample.cpp</code>，注意这份代码 <strong>不保证可以通过所有的测试用例</strong> 。 </p>
<h2>数据范围</h2>
<p><strong><em>本题严禁任何形式的攻击交互库的行为，一旦发现，将取消相关选手的参赛资格。</em></strong></p>
<p><strong>Small Task:</strong> 蒜斜保证程序中仅包含 $\mathrm{xor}$ 操作，且 $\mathrm{xor}$ 语句中的 $b,c$ 均不是常量。</p>
<p><strong>Large Task:</strong> 无特殊限制</p>
<p>对于所有数据，满足 $1 \le m \le 3,Q = 101,K = 2000$</p>
<p><strong>时间限制:</strong> $1\texttt{s}$</p>
<p><strong>空间限制:</strong> $512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21047/file/attachment.zip">样例及测评库下载</a></p>
