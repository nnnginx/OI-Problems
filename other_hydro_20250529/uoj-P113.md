<p>���ڵ��ż����ķ�չ�����˶�����ͨ���ֻ�������ϵ��</p>
<p>��һλ���Ŵ������������һ�����ֻ���Ȼ������������һ̨һ̨������ʵ��̫���ˣ������������һ���취 ���� ���ֻ����Ҹ��ơ�</p>
<p>���������ֻ�������һ�����õĺ��� <samp>fork()</samp>���ֻ��ĳ���������������������ô�ֻ���������һ̨<strong>��ȫһģһ��</strong>���ֻ���<strong>������������״̬</strong>���������Լ���̨�ĺ�������ֵΪ $1$�����ֻ��ĺ�������ֵΪ $0$��Ȼ����̨�ֻ���<strong>����ִ�г���</strong>������ע����������ݣ�</p>
<p>��ʼʱ��ֻ��һ̨�ֻ������ţ��������ֻ��������������ı��ʽ��</p>
<pre><code class="sh_cpp">fork() &lt;op&gt; fork() &lt;op&gt; ... &lt;op&gt; fork()</code></pre>
<p>���� <samp>&lt;op&gt;</samp> �Ƕ�Ԫ�������Ϊ <samp>&amp;&amp;</samp> ���� <samp>||</samp> �е�һ�֡����磺</p>
<pre><code class="sh_cpp">fork() &amp;&amp; fork() || fork() &amp;&amp; fork() &amp;&amp; fork() || fork()</code></pre>
<p>�������㶼�����ϵģ��� <samp>&amp;&amp;</samp> �����ȼ��� <samp>||</samp> �ߣ�����������Ǹ����ʽ�൱�ڣ�</p>
<pre><code class="sh_cpp">((fork() &amp;&amp; fork()) || ((fork() &amp;&amp; fork()) &amp;&amp; fork())) || fork()</code></pre>
<p>���ڱ��ʽ <samp>a &amp;&amp; b</samp>���ֻ����ȼ��� <samp>a</samp> ��ֵ�����Ϊ $0$ ��ô<strong>������</strong> <samp>b</samp> ��ֵ����Ϊ����Ҫ����˵���飬��ע������<strong>������</strong> <samp>b</samp> ��ֵ�����ñ��ʽֵΪ $0$��������� <samp>b</samp> ��ֵ������ֵ��Ϊ�ñ��ʽ��ֵ��</p>
<p>���ڱ��ʽ <samp>a || b</samp>���ֻ����ȼ��� <samp>a</samp> ��ֵ�����Ϊ $1$ ��ô<strong>������</strong> <samp>b</samp> ��ֵ����Ϊ����Ҫ����˵���飬��ע������<strong>������</strong> <samp>b</samp> ��ֵ�����ñ��ʽֵΪ $1$��������� <samp>b</samp> ��ֵ������ֵ��Ϊ�ñ��ʽ��ֵ��</p>
<p>���ʽ������ɺ󣬴�����������������˵��ֻ�����������ߵ����ָ������ҵ����Ĵ��š�</p>
<p>һ�������һλ����ѧ�ҵ����˴˴��¼������õ��˴������ֻ�����ı��ʽ������֪�����е��꾿��������˶���̨�ֻ�����������ʼ����̨�ֻ���</p>
<p><strong>����Բ����������������õ�������⡣</strong></p>
<h2>�����ʽ</h2>
<p>��һ��һ�������� $n$����ʾ���ʽ�е� <samp>fork()</samp> ��������</p>
<p>������һ�� $n - 1$ ���ÿո�������ַ�����ÿ���ַ���Ϊ ��<samp>&amp;&amp;</samp>�� ���� ��<samp>||</samp>�������α�ʾ���ʽ�ж�Ӧλ�õ��������</p>
<h2>�����ʽ</h2>
<p>һ�У�һ��������ʾ��������ֻ�����������ֻ������𰸶� $998244353$��$7 \times 17 \times 2^{23} + 1$��һ��������ȡģ��Ľ����</p>


<pre><code class="language-input1">2
&amp;&amp;
</code></pre>


<pre><code class="language-output1">3
</code></pre>


<p>������ $3$ ̨�ֻ����������£�</p>
<ol><li>�� $1$ ̨�ֻ���ʼ���� <samp>fork() &amp;&amp; fork()</samp>��</li>
<li>�� $1$ ̨�ֻ���ʼ���� <samp>fork()</samp>�������˵� $2$ ̨�ֻ���</li>
<li>�� $1$ ̨�͵� $2$ ̨�� <samp>fork()</samp> ������ɣ��� $1$ ̨���� $1$���� $2$ ̨���� $0$��</li>
<li>�� $1$ ̨�ֻ����� <samp>fork()</samp> ����ֵΪ $1$����ʼ���� <samp>fork() &amp;&amp; fork()</samp> �ұߵ� <samp>fork()</samp>�������˵� $3$ ̨�ֻ���</li>
<li>�� $2$ ̨�ֻ����� <samp>fork()</samp> ����ֵΪ $0$������ <samp>fork() &amp;&amp; fork()</samp> ֵΪ $0$�������ұߵ� <samp>fork</samp> �ļ��㣩�����������</li>
<li>�� $1$ ̨�͵� $3$ ̨�� <samp>fork()</samp> ������ɣ��� $1$ ̨���� $1$���� $3$ ̨���� $0$��</li>
<li>�� $1$ ̨�ֻ����� <samp>fork()</samp> ����ֵΪ $1$������ <samp>fork() &amp;&amp; fork()</samp> ֵΪ $1$�����������</li>
<li>�� $3$ ̨�ֻ����� <samp>fork()</samp> ����ֵΪ $0$������ <samp>fork() &amp;&amp; fork()</samp> ֵΪ $0$�����������</li>
</ol>

<pre><code class="language-input2">6
&amp;&amp; || &amp;&amp; &amp;&amp; ||
</code></pre>


<pre><code class="language-output2">15
</code></pre>

<h2>������Լ��</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th>
<th>$n$�Ĺ�ģ</th>
</tr></thead><tbody><tr><td>1</td><td>$n = 1$</td></tr><tr><td>2</td><td rowspan="3">$n \leq 5$</td></tr><tr><td>3</td></tr><tr><td>4</td></tr><tr><td>5</td><td rowspan="3">$n \leq 100$</td></tr><tr><td>6</td></tr><tr><td>7</td></tr><tr><td>8</td><td rowspan="3">$n \leq 100000$</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20553/file/attachment.zip">������������</a></p>
