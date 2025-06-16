<p>����ɳ���꣨Shahnameh���еĹŴ���˹��˵��Zal������Ĳ�˹Ӣ�ۣ����ذ����� Kabul �����Ĺ��� Rudaba���� Zal �� Rudaba ���ʱ��Rudaba �ĸ��׸�����һ����ս��</p>
<p>�ڲ�˹�� $n$ �����У����Ϊ�� $0$ �� $n-1$���Լ� $m$ ��˫���·�����Ϊ�� $0$ �� $m-1$��ÿ����·����������ͬ�ĳ��С�ÿһ�Գ�������ᱻһ����·���ӡ���Щ��·��������royal roads����ר���ڻ�����ʻ�������Ǳ��ܵġ�Zal ���������ҳ���Щ��·��������</p>
<p>Zal ��һ�Ű������г��к����е�·�Ĳ�˹��ͼ������֪����Щ��·����������������������� Simurgh�������ĵ�����Zal �ı����ߡ�Ȼ����Simurgh ������ֱ�Ӹ�������Щ��·����������Ϊ�����Simurgh ���� Zal�����������ļ�����һ���ƽ𼯺ϣ�golden set����һ����·�ļ����ǻƽ𼯺ϣ����ҽ�����</p>
<ul>
<li>��ǡ�ð��� $n-1$ ����·������</li>
<li>����ÿһ�Գ��У���������������еĵ�·���ɴ�����һ�����еִ�����һ�����С�</li>
</ul>
<p>���⣬Zal ������ Simurgh һЩ���⡣����ÿ�����⣺</p>
<ol>
<li>Zal ѡ����·��һ���ƽ𼯺ϣ�Ȼ��</li>
<li>Simurgh ����� Zal������ѡ��Ļƽ𼯺����ж�������·��������</li>
</ol>
<p>��ĳ�������� Simurgh ��� $q$ �����⣬�Դ˰��� Zal �ҳ������ļ��ϡ����⹤�߽����� Simurgh �Ľ�ɫ��</p>
<h2>ʵ��ϸ��</h2>
<p><strong>����ֻ֧��C++��</strong></p>
<p>����Ҫʵ������ĺ�����</p>
<pre><code class="sh_cpp"> std::vector&lt;int&gt; find_roads(int n, std::vector&lt;int&gt; u, std::vector&lt;int&gt; v)</code></pre>
<ul>
<li>$n$�����е�������</li>
<li>$u$ �� $v$����Ϊ����Ϊ $m$ �����顣�������� $0\leq i\leq m-1$��$u[i]$ �� $v[i]$ �Ǳ���· $i$ �����ӵĳ��С�</li>
<li>�ú�����Ҫ����һ������Ϊ $n-1$ �����飬���а��������������ı�ţ������������˳���������</li>
</ul>
<p>��ĳ�������ֻ�ܵ������⹤���е����º��� $q$ �Σ�</p>
<pre><code class="sh_cpp"> int count_common_roads(std::vector&lt;int&gt; r)</code></pre>
<ul>
<li>$r$������Ϊ $n-1$ �����飬���а�����һ���ƽ𼯺��еĵ�·��ţ������������˳���������</li>
<li>�ú��������� $r$ �е�����������</li>
</ul>
<h2>����</h2>
<p>���⹤�ߵ��� <code>find_roads(4, [0, 0, 0, 1, 1, 2], [1, 2, 3, 2, 3, 3])</code>��</p>
<p><img src="https://img.uoj.ac/problem/324/IOI2017-simurgh-desc.png" alt="����" class="img-responsive center-block" style="width:600px;"></p>
<p>����������� $4$ �����к� $6$ ����·�����ǽ����ӳ��� $a$ �� $b$ �ĵ�·��ʾΪ $(a,b)$����Щ��·���������˳�򱻱�Ϊ�� $0$ �� $5$��$(0,1)$��$(0,2)$��$(0,3)$��$(1,2)$��$(1,3)$ �� $(2,3)$��ÿ���ƽ𼯺ϰ��� $n-1=3$ ����·��</p>
<p>���������Ǳ��Ϊ $0$��$1$ �� $5$ �ĵ�·���� $(0,1)$��$(0,2)$ �� $(2,3)$�������Ļ���</p>
<p><code>count_common_roads([0, 1, 2])</code> ���� $2$����ѯ���漰�����Ϊ $0,1$ �� $2$ �ĵ�·���� $(0,1)$��$(0,2)$ �� $(0,3)$��������������·��������</p>
<p><code>count_common_roads([5, 1, 0])</code> ���� $3$����ѯ���漰�����е�������</p>
<p>���� <code>find_roads</code> ��Ҫ���� $[5,1,0]$ ��������������������Ԫ���ҳ���Ϊ $3$ �����顣</p>
<p>ע�⣬�����г��ĵ����ǲ�����ģ�</p>
<ul>
<li><p><code>count_common_roads([0, 1])</code>������ $r$ �ĳ��Ȳ��� $3$��</p>
</li>
<li><p><code>count_common_roads([0, 1, 3])</code>������ $r$ ����һ���ƽ𼯺ϣ���Ϊ�޷����ص�· $(0,1)$��$(0,2)$��$(1,2)$ �ʹӳ��� $0$ �ߵ����� $3$��</p>
</li>
</ul>
<h2>���ݷ�Χ</h2>
<ul>
<li>$2\leq n\leq 500$</li>
<li>$n-1\leq m\leq n(n-1)/2$</li>
<li>$0\leq u[i],v[i]\leq n-1$���������� $0\leq i\leq m-1$��</li>
<li>�������� $0\leq i\leq m-1$����· $i$ ����������ͬ�ĳ��У��� $u[i]\neq v[i]$����</li>
<li>ÿ�Գ���֮����������һ����·��</li>
<li>������Щ��·������������һ�Գ���֮��������</li>
<li>���е��������һ���ƽ𼯺ϡ�</li>
<li><code>find_roads</code> ���Ե��� <code>count_common_roads</code> ��� $q$ �Ρ���ÿ�ε����У��� $r$ �������ĵ�·������һ���ƽ𼯺ϡ�</li>
</ul>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">$n\leq$</th>
<th style="text-align:center;">$q=$</th>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">��ֵ</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;" rowspan="3">$30000$</td>
<td style="text-align:center;" rowspan="2">��</td>
<td style="text-align:center;">$13$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$50$</td>
<td style="text-align:center;">$17$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$240$</td>
<td style="text-align:center;">��������������֮�䶼����һ����·</td>
<td style="text-align:center;">$21$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;" rowspan="2">$500$</td>
<td style="text-align:center;">$12000$</td>
<td style="text-align:center;" rowspan="2">��</td>
<td style="text-align:center;">$19$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$8000$</td>
<td style="text-align:center;">$30$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ������</strong>��$3\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$1024\texttt{MB}$</p>
<h2>���ֳ�������</h2>
<p>���ֳ�������������������ʽ���������ݣ�</p>
<ul>
<li>�� $1$ �У�$n\ m$</li>
<li>�� $2+i$ �У��������� $0\leq i\leq m-1$����$u[i]\ v[i]$</li>
<li>�� $2+m$ �У�$s[0]\ s[1]\ \cdots\ s[n-2]$</li>
</ul>
<p>���� $s[0],s[1],\ldots,s[n-2]$ �����������ı�š�</p>
<p>��� <code>find_roads</code> ������ <code>count_common_roads</code> �� $30000$ �Σ�������ȷ�ط����������ļ��ϣ����ֳ�������������� <code>YES</code>���������ֳ�������������� <code>NO</code>��</p>
<p>��Ҫ��ȷ���ǣ����ֳ��������еĺ��� <code>count_common_roads</code> ������ $r$ �Ƿ�����һ���ƽ𼯺ϵ���������������Եأ���������� $r$ �е��������м��������ҷ��ء�Ȼ���������ύ�ĳ������ <code>count_common_roads</code> ʱ������������Ĳ��Ƕ�Ӧĳ���ƽ𼯺ϵı�ż��ϣ������������� <code>Wrong Answer</code>��</p>
<h2>hack</h2>
<p>�� <code>hack</code> ʱ�����ݸ�ʽ���������ƣ���������Ҫ�ڵ� $1$ �����������ѯ�ʴ������� $q$������Ҫ�� $q\in \{8000,12000,30000\}$��</p>
<h2>������ʾ</h2>
<p>����Ч�ʷ���Ŀ��ǣ����� <code>count_common_roads</code> ʹ���˴����õ��ã�call by reference���ķ�ʽ���������ƽ��һ������������������⹤��ȷ������ı� $r$ �е�ֵ��</p>
<h2>����</h2>
<p><a href="./20750/file/attachment.zip">�����������������������</a></p>
