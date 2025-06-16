<p>wangyisong1996 ��һ��С���磬��ϧ��������ɳĮ��С��������ˡ����� wangyisong1996 ��ʹ������ʱ�򣬴�ɳ���г�����һ�������ơ�</p>
<p>���һ��������ͨͼ������һ�����������һ���򵥻������Ǿͳ�֮Ϊ�����ơ���ν�򵥻����������ظ��Ľ��Ļ���</p>
<p><img class="img-responsive center-block" src="//img.uoj.ac/utility/what-is-cactus.png" alt="ʲô��������"></p>
<p>��һ�� $n$ �����������ƣ�ÿ������һ������ $l$������ͬ�ıߵĳ��Ȳ�һ����ͬ��</p>
<p>�� $q$ ���㼯��ÿ���㼯�������������� $u, d$ ��������$1 \leq u \leq n$����һ����� $v$ ������㼯�е��ҽ������ $v$ ���� $u$ �ľ��벻���� $d$���������֮��ľ���Ϊ����֮������·���ĳ��ȡ�</p>
<p>����Ҫ����һ�������޻�ͼ��DAG�������㣺</p>
<ol><li>��� DAG ������ $n+q$ ����㣬������ $1200000$ ������ $2400000$ ���ߡ�</li>
<li>����ÿһ���ߣ�����Ǵ� $u$ ���� $v$ �ģ���ô $u &gt; n$ �� $u \neq v$��</li>
<li>���ڽ�����ڵ� $i$ ���㼯��$1 \leq i \leq q$����ÿһ����� $x$���� $n+i$ ����㵽�� $x$ ��������ҽ���һ��·����</li>
<li>���ڽ������ $\{ 1, 2, \dots, n\}$ �е����ڵ� $i$ ���㼯��$1 \leq i \leq q$����ÿһ����� $x$�������ڵ� $n+i$ ����㵽�� $x$ ������·����</li>
</ol><h2>�����ʽ</h2>
<p>��һ������������ $n, m, q$������ $n, m$ ��ʾ���������һ���� $n$ ����� $m$ ���ߡ�</p>
<p>������ $m$ �У�ÿ���������� $u,v,l$����ʾ $u$ �� $v$ ֮����һ������Ϊ $l$ ������ߡ���֤ $1 \leq u, v \leq n$��</p>
<p>������ $q$ �У��� $i$ �б�ʾ�� $i$ ���㼯������������ $u, d$ ����������֤ $1 \leq u \leq n$��</p>
<h2>�����ʽ</h2>
<p>��һ�������Ǹ����� $V,E$����ʾ�㹹��� DAG �ĵ����ͱ�����</p>
<p>������ $E$ �У�ÿ���������� $u,v$����ʾ $u$ �� $v$ ��һ������ߡ�����Ҫ��֤ $1 \leq u, v \leq V$��</p>


<pre><code class="language-input1">10 9 5
2 1 9553
3 2 8499
4 3 5171
5 1 7123
6 3 1904
7 5 5526
8 7 5853
9 6 6635
10 8 7858
6 4981
7 14400
3 21290
4 9451
10 16609
</code></pre>


<pre><code class="language-output1">15 19
11 6
11 3
12 7
12 5
12 1
12 8
12 10
13 3
13 6
13 9
13 4
13 2
13 1
14 4
14 3
14 6
15 10
15 8
15 7
</code></pre>

<h2>������Լ��</h2>
<p>����ÿһ���ߣ�$1 \leq l \leq 10000$������ÿ���㼯��$0 \leq d \leq 10^9$��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th>
<th>$n$</th>
<th>$m$</th>
<th>$q$</th>
</tr></thead><tbody><tr><td>1</td><td>$= 1000$</td><td rowspan="5">$m = n - 1$</td><td>$= 1000$</td></tr><tr><td>2</td><td rowspan="2">$= 10000$</td><td rowspan="2">$= 10000$</td></tr><tr><td>3</td></tr><tr><td>4</td><td>$= 9000$</td><td>$= 9000$</td></tr><tr><td>5</td><td>$= 10000$</td><td>$= 10000$</td></tr><tr><td>6</td><td>$= 1000$</td><td rowspan="5">$n - 1 \leq m \leq 2n - 2$</td><td>$= 1000$</td></tr><tr><td>7</td><td rowspan="4">$= 10000$</td><td rowspan="4">$= 10000$</td></tr><tr><td>8</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p>�� 2 �����Ե�����ɷ�ʽ��</p>
<pre><code class="sh_python">for i in range(2, 10001):
    addedge(i, i / 2)</code></pre>
<p>�� 3 �����Ե�����ɷ�ʽ��</p>
<pre><code class="sh_python">for i in range(2, 5000):
    addedge(i, i - 1)
for i in range(5000, 10001):
    addedge(i, randint(1, i - 1))</code></pre>
<p>���� <samp>range(l,r)</samp> ��ʾ���� $[l,r)$ �е���������<samp>randint(l,r)</samp> ����һ���� $[l,r]$ �ڵ����������</p>
<p><samp>addedge(u, v)</samp> ��ʾ�� $u$ �� $v$ ����һ���ߡ����ߵĳ��ȵ����ɷ�ʽ������Ϊ�һ�������𣿣�</p>
<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<h2>��Դ</h2>
<p>�й����Ҽ�ѵ�ӻ���2015 - By ������</p>
<h2>����</h2>
<p><a href="./20532/file/attachment.zip">������������</a></p>
