<p><strong>����ĳЩԭ�����֧�� C++, C++11 ���Ե��ύ��</strong></p>
<p>�ڸ���һ����԰��� $n$ ����Ȫ�����Ϊ�� $0$ �� $n - 1$�����ǰ���Ȫ�����Ƕ�άƽ���ϵĵ㡣Ҳ����˵����Ȫ $i$��$0 \le i \le n - 1$����һ���� $(x[i], y[i])$������ $x[i]$ �� $y[i]$ ��ż������Ȫ��λ�ø�����ͬ��</p>
<p>����ʦ Timothy �ܹ����滮һЩ��·�Ľ��裬�Լ�ÿ����·��Ӧ�ĳ��εİڷš�ÿ����·����һ������Ϊ $2$ �ĺ����������߶Σ���˵���������ͬ����Ȫ���ο�Ӧ���ܹ��������Ǽ���������������Ȫ֮�以��ִ���ʼʱ����԰��û���κε�·��</p>
<p>����ÿ����·����Ҫ�ڹ�԰��ڷ�ǡ��һ�����Σ�������������Ҳ�����泯��������·��ÿ�����α���ڷ���ĳ���� $(a, b)$ �ϣ����� $a$ �� $b$ �������������г��ε�λ�ñ��붼�ǲ�ͬ�ġ��� $(a, b)$ ���ĳ��Σ�ֻ�ܷ���������˵��Ϊ $(a - 1, b - 1)$��$(a - 1, b + 1)$��$(a + 1, b - 1)$ �� $(a + 1, b + 1)$ ����֮һ�ĵ�·��������˵���� $(3, 3)$ ���ĳ���ֻ�ܷ�������������߶�����ʾ�ĵ�·֮һ��$(2, 2) - (2, 4)$��$(2, 4) - (4, 4)$��$(4, 4) - (4, 2)$��$(4, 2) - (2, 2)$��</p>
<p>����� Timothy �ж�һ�£��ܷ���������������Ҫ���ǰ���£�������е�·�����ڷźͷ��䳤�Ρ�������������������һ�����еĽ������������ж����������Ҫ��Ŀ��з���������Ա������е����ⷽ����</p>
<h2>ʵ��ϸ��</h2>
<p>��������� <code>parks.h</code> ͷ�ļ���</p>
<p>��Ҫʵ�����º�����</p>
<pre><code class="sh_cpp">int construct_roads(int[] x, int[] y)</code></pre>
<ul>
<li>$x, y$������Ϊ $n$ ���������顣������ $i$��$0 \le i \le n - 1$������Ȫ $i$ ��һ���� $(x[i], y[i])$������ $x[i]$ �� $y[i]$ ����ż����</li>
<li>�������ĳ�����跽��������Ӧ������ <code>build</code>���μ����ģ�ǡ��һ�������潨�跽�����������ŷ��� $1$��</li>
<li>���򣬺���Ӧ������ $0$�����Ҳ��� <code>build</code> ���κε��á�</li>
<li>�ú�����������ǡ��һ�Ρ�</li>
</ul>
<p>��ʵ�ֵĺ������Ե�������ĺ��������ṩһ�����еĵ�·�����볤�ΰڷŷ�����</p>
<pre><code class="sh_cpp">void build(int[] u, int[] v, int[] a, int[] b)</code></pre>
<p>�� $m$ Ϊ���跽���е�·��������</p>
<ul>
<li>$u, v$������Ϊ $m$ ���������飬��ʾҪ����ĵ�·����Щ��·�ı��Ϊ�� $0$ �� $m - 1$�������е� $j$��$0 \le j \le m - 1$������· $j$ Ҫ������Ȫ $u[j]$ �� $v[j]$��ÿ����·�����ǳ���Ϊ $2$ �ĺ���������߶Ρ�����������ͬ�ĵ�·�����ֻ����һ�������˵㣨ĳ����Ȫ������Щ��·�ڽ���֮�󣬱����ܹ��������ǾͿ���������������Ȫ֮�以��ִ</li>
<li>$a, b$������Ϊ $m$ ���������飬��ʾ���Ρ������е� $j$��$0 \le j \le m - 1$�������� $(a[j], b[j])$ ���ڷ�һ�����Σ����ҷ������· $j$����ͬ�ĳ��β��ܰڷ���ͬһλ�á�</li>
</ul>
<h2>�����ʽ</h2>
<p>�������ʾ����ȡ���¸�ʽ�����룺</p>
<ul>
<li>�� $1$ �У�$n$</li>
<li>�� $2 + i$ �У�$0 \le i \le n - 1$����$x[i] \; y[i]$</li>
</ul>
<h2>�����ʽ</h2>
<p>�������ʾ����������Ϊ���¸�ʽ��</p>
<ul>
<li>�� $1$ �У�<code>construct_roads</code> �ķ���ֵ</li>
</ul>
<p>��� <code>construct_roads</code> �ķ���ֵΪ $1$�����ҵ��ù� <code>build(u, v, a, b)</code>���������ʾ�������������</p>
<ul>
<li>�� $2$ �У�$m$</li>
<li>�� $3 + j$ �У�$0 \le j \le m - 1$����$u[j] \; v[j] \; a[j] \; b[j]$</li>
</ul>


<pre><code class="language-input1">5
4 4
4 6
6 4
4 2
2 4
</code></pre>


<pre><code class="language-output1">1
4
0 2 5 5
0 1 3 5
3 0 5 3
4 0 3 3
</code></pre>


<p>�������µ��ã�</p>
<pre><code class="sh_cpp">construct_roads([4, 4, 6, 4, 2], [4, 6, 4, 2, 4])</code></pre>
<p>����ζ���ܹ��� $5$ ����Ȫ��</p>
<ul>
<li>��Ȫ $0$ ������ $(4, 4)$ ����</li>
<li>��Ȫ $1$ ������ $(4, 6)$ ����</li>
<li>��Ȫ $2$ ������ $(6, 4)$ ����</li>
<li>��Ȫ $3$ ������ $(4, 2)$ ����</li>
<li>��Ȫ $4$ ������ $(2, 4)$ ����</li>
</ul>
<p>���Խ����������� $4$ ����·������ÿ����·����������Ȫ�����Ұڷ��Ŷ�Ӧ�ĳ��Σ�</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:left;">��·���</th>
<th style="text-align:left;">��·�����ӵ���Ȫ�ı��</th>
<th style="text-align:left;">������ĳ��ε�λ��</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">$0$</td>
<td style="text-align:left;">$0, 2$</td>
<td style="text-align:left;">$(5, 5)$</td>
</tr>
<tr>
<td style="text-align:left;">$1$</td>
<td style="text-align:left;">$0, 1$</td>
<td style="text-align:left;">$(3, 5)$</td>
</tr>
<tr>
<td style="text-align:left;">$2$</td>
<td style="text-align:left;">$3, 0$</td>
<td style="text-align:left;">$(5, 3)$</td>
</tr>
<tr>
<td style="text-align:left;">$3$</td>
<td style="text-align:left;">$4, 0$</td>
<td style="text-align:left;">$(3, 3)$</td>
</tr>
</tbody>
</table>
</div>
<p>�÷�����Ӧ��ͼ��</p>
<p><img src="https://loj-img.upyun.menci.memset0.cn/2021/06/24/60d3671b71ec2.png" alt="" class="img-responsive center-block"></p>
<p>Ϊ����˷�����<code>construct_roads</code> Ӧ�������µ��ã�</p>
<pre><code class="sh_cpp">build([0, 0, 3, 4], [2, 1, 0, 0], [5, 3, 5, 3], [5, 5, 3, 3])</code></pre>
<p>�����Ӧ������ $1$��</p>
<p>ע�⣬����������У��ж������Ҫ��ķ��������Ƕ�������Ϊ��ȷ�����磬���� <code>build([1, 2, 3, 4], [0, 0, 0, 0], [5, 5, 3, 3], [5, 3, 3, 5])</code> ������ $1$��Ҳ����ȷ�ġ�</p>


<pre><code class="language-input2">2
2 2
4 6
</code></pre>


<pre><code class="language-output2">0
</code></pre>


<p>�������µ��ã�</p>
<pre><code class="sh_cpp">construct_roads([2, 4], [2, 6])</code></pre>
<p>��Ȫ $0$ ������ $(2, 2)$ ��������Ȫ $1$ ������ $(4, 6)$ �������ڲ����ܽ��������Ҫ��ĵ�·��<code>construct_roads</code> Ӧ������ $0$�����Ҳ��� <code>build</code> ���κε��á�</p>
<h2>���ݷ�Χ</h2>
<p>�����������ݣ�</p>
<ul>
<li>$1 \le n \le 200 \, 000$</li>
<li>$2 \le x[i], y[i] \le 200 \, 000$���������� $0 \le i \le n - 1$��</li>
<li>$x[i]$ �� $y[i]$ ����ż������������ $0 \le i \le n - 1$��</li>
<li>����������Ȫ��λ�þ�����ͬ</li>
</ul>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">������</th>
<th style="text-align:center;">��ֵ</th>
<th style="text-align:center;">��������</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$x[i] = 2$���������� $0 \le i \le n - 1$��</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">$2 \le x[i] \le 4$���������� $0 \le i \le n - 1$��</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$15$</td>
<td style="text-align:center;">$2 \le x[i] \le 6$���������� $0 \le i \le n - 1$��</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$20$</td>
<td style="text-align:center;">����ֻ��һ�ֵ�·���跽�����ܹ����ο�������������Ȫ֮��������Щ��·���ɻ���ִ�</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$20$ </td>
<td style="text-align:center;">����������Ȫ�����ṹ��ĳһ�� $2 \times 2$ �����ε��ĸ�����</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$30$</td>
<td style="text-align:center;">û�ж����Լ������</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ�����ƣ�$\texttt{3s}$</strong></p>
<p><strong>�ռ����ƣ�$\texttt{2GB}$</strong></p>
