<p><strong> ����ĳЩԭ�����֧�� C++, C++11 ���Ե��ύ�� </strong></p>
<p>Khong ��������֯һ���� $x$ λѡ�ֲμӵľ������������ÿλѡ��<strong>һ������</strong>���ܹ��� $k$ �ֲ�ͬ���͵ı��ɣ����Ϊ�� $0$ �� $k - 1$������Ϊ $i$��$0 \le i \le k - 1$����ÿ����ɶ���һ��<strong>��ζֵ</strong> $2^i$���� Khong ���̵�ʳƷ��������� $a_i$���п���Ϊ $0$��������Ϊ $i$ �ı��ɡ�</p>
<p>��ÿ�����͵ı��ɣ�Khong ������ÿ�����Ӷ���װ�� $0$ ���߶�顣���д�����������Ϊ $i$ �ı��ɵ��ܿ������ܳ��� $a_i$��һ�������������б��ɵĿ�ζֵ���ܺͣ�����Ϊ������ɵ�<strong>�ܿ�ζֵ</strong>��</p>
<p>��� Khong ������һ�£��������ڶ��ٲ�ͬ�� $y$ ֵ��ʹ��������װ�� $x$ �����ɣ�����ÿ�����ɵ��ܿ�ζֵ������ $y$��</p>
<h2>ʵ��ϸ��</h2>
<p>��������� <code>biscuits.h</code> ͷ�ļ���</p>
<p>����Ҫʵ�����º�����</p>
<pre><code class="sh_cpp">long long count_tastiness(long long x, std::vector&lt;long long&gt; a)</code></pre>
<ul><li>$x$����Ҫװ�ı��ɴ���������</li>
<li>$a$������Ϊ $k$ �����顣�� $0 \le i \le k - 1$��$a_i$ ��ʾ��ʳ�ﴢ����������Ϊ $i$ �ı���������</li>
<li>�˺���Ӧ�����ز�ͬ $y$ ֵ����Ŀ��ʹ�ð��̿���װ�� $x$ �����ɣ���ÿ�����ɵ��ܿ�ζֵ��Ϊ $y$��</li>
<li>�˺����ᱻ���� $q$ �Σ���������� $q$ ֵ�����Լ�������������񲿷֣���ÿ�ε���Ӧ���������Ƕ����ĳ�����</li>
</ul><h2>�����ʽ</h2>
<p>�������ʾ������ȡ���¸�ʽ���������ݡ���һ�а���һ������ $q$���������� $q$ �����������У����ǰ�������ĸ�ʽ������һ�������ĳ�����</p>
<ul><li>��һ�У�$k\ x$</li>
<li>�ڶ��У�$a_0\ a_1\ \ldots\ a_{k - 1}$</li>
</ul><h2>�����ʽ</h2>
<p>�������ʾ�����������ĸ�ʽ���£�</p>
<ul><li>�� $i$ �У�$1 \le i \le q$����<code>count_tastiness</code> �������������е� $i$ �������ķ���ֵ��</li>
</ul>

<pre><code class="language-input1">2
3 3
5 2 1
3 2
2 1 2
</code></pre>


<pre><code class="language-output1">5
6
</code></pre>


<p>���ڵ�һ�����ݣ�
�������µ��ã�</p>
<pre><code class="sh_cpp">count_tastiness(3, [5, 2, 1])</code></pre>
<p>����ζ�Ű��̴���װ $3$ �����ɣ�����ʳ�ﴢ�������ܹ��� $3$ �����͵ı��ɣ�
- $5$ ������Ϊ $0$ �ı��ɣ�ÿ��Ŀ�ζֵΪ $1$��
- $2$ ������Ϊ $1$ �ı��ɣ�ÿ��Ŀ�ζֵΪ $2$��
- $1$ ������Ϊ $2$ �ı��ɣ����ζֵΪ $4$��</p>
<p>$y$ �ܹ�ȡ��ֵΪ $[0,1,2,3,4]$��������˵��Ϊ��װ���ܿ�ζֵ��Ϊ $3$ �� $3$ �����ɣ����̿�������װ��</p>
<ul><li>һ���������� $3$ ������Ϊ $0$ �ı��ɣ��Լ�</li>
<li>�������ɣ����и���һ������Ϊ $0$ �ı��ɺ�һ������Ϊ $1$ �ı��ɡ�</li>
</ul><p>�����ܹ��� $5$ �����ܵ� $y$ ֵ������Ӧ������ $5$��</p>
<p><img src="https://img.uoj.ac/problem/567/567_ex1.png" alt="����һ" class="img-responsive center-block" style="width:500px;"></p>
<p>���ڵڶ������ݣ�</p>
<p>�������µ��ã�</p>
<pre><code class="sh_cpp">count_tastiness(2, [2, 1, 2])</code></pre>
<p>����ζ�Ű��̴���װ $2$ �����ɣ�����ʳ�ﴢ�������ܹ��� $3$ �����͵ı��ɣ�
- $2$ ������Ϊ $0$ �ı��ɣ�ÿ��Ŀ�ζֵΪ $1$��
- $1$ ������Ϊ $1$ �ı��ɣ����ζֵΪ $2$��
- $2$ ������Ϊ $2$ �ı��ɣ�ÿ��Ŀ�ζֵΪ $4$��</p>
<p>$y$ �ܹ�ȡ��ֵΪ $[0,1,2,4,5,6]$�������ܹ��� $6$ �����ܵ� $y$ ֵ������Ӧ������ $6$��</p>
<h2>������Լ��</h2>
<p>����ȫ�����ݣ����㣺</p>
<ul><li>$1\le k\le 60$</li>
<li>$1\le q\le 1000$</li>
<li>$1\le x\le 10^{18}$</li>
<li>$0\le a_i\le 10^{18}$���������е� $0\le i\le k-1$��</li>
<li>���� <code>count_tastiness</code> ��ÿ�ε��ã�ʳ�ﴢ���������б��ɵĿ�ζֵ�ܺͶ����ᳬ�� $10^{18}$��</li>
</ul><p>��ϸ�������ֵ�븽���������±�</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th style="text-align:center;">������</th>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">��ֵ</th>
</tr></thead><tbody><tr><td style="text-align:center;">$1$</td>
<td style="text-align:center;">$q\le 10$���Ҷ��� <code>count_tastiness</code> ��ÿ�ε��ã�ʳ�ﴢ���������б��ɵĿ�ζֵ�ܺͶ����ᳬ�� $100\ 000$��</td>
<td style="text-align:center;">$9$</td>
</tr><tr><td style="text-align:center;">$2$</td>
<td style="text-align:center;">$x=1,q\le 10$</td>
<td style="text-align:center;">$12$</td>
</tr><tr><td style="text-align:center;">$3$</td>
<td style="text-align:center;">$x\le 10\ 000,q\le 10$</td>
<td style="text-align:center;">$21$</td>
</tr><tr><td style="text-align:center;">$4$</td>
<td style="text-align:center;">���� <code>count_tastiness</code> ��ÿ�ε��ã���ȷ�ķ��ؽ�������ᳬ�� $200\ 000$��</td>
<td style="text-align:center;">$35$</td>
</tr><tr><td style="text-align:center;">$5$</td>
<td style="text-align:center;">û�и�������������</td>
<td style="text-align:center;">$23$</td>
</tr></tbody></table></div>
<p><strong>ʱ������</strong>��$1 \texttt{s}$</p>
<p><strong>�ռ�����</strong>��$1024 \texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20971/file/attachment.zip">����������������</a></p>
