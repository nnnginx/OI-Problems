<p>Maryam ��һλ�������ʦ��������Ϊһ��ͨѶ����ƽ��߷����������������һЩ�ֲ��ڲ�ͬ�߶ȵ����ӵ㡣һ�����߿����������κ��������ӵ��������ÿһ�����ӵ㶼���Խ���������Ŀ�ĵ��ߡ������ӵ㹲�����֣��ֱ�Ϊ��ɫ���ӵ㼰��ɫ���ӵ㡣</p>
<p>Ϊ�˱������������ͨѶ���ᱻ��Ϊһ��ֱ�ߣ�����Щ��ɫ����ɫ���ӵ�ᱻ��Ϊ������ֱ���ϵ�һЩ�Ǹ��������ꡣһ�����ߵĳ����Ǹõ��������ӵ��������ӵ��ľ��롣</p>
<p>��Ҫ�����ǰ� Maryam �ҳ�һ�����ߵķ�����ʹ����������������</p>
<ol>
<li>ÿ�����ӵ���������һ���������ӵ�һ����ͬ��ɫ�����ӵ���</li>
<li>���õĵ��ߵ��ܳ���Ϊ��̡�</li>
</ol>
<h2>ʵ��ϸ��</h2>
<p><strong>����ֻ֧��C++��</strong></p>
<p>����Ҫʵ�����µ��ӳ���</p>
<pre><code class="sh_cpp"> long long min_total_length(std::vector&lt;int&gt; r, std::vector&lt;int&gt; b)</code></pre>
<ul>
<li>$r$: һ������Ϊ $n$ �����飬�������������������к�ɫ���ӵ��λ�á�</li>
<li>$b$: һ������Ϊ $m$ �����飬����������������������ɫ���ӵ��λ�á� </li>
<li>����ӳ����践�������п��ܵ����ӷ����У���̵����ܳ��ȵ��Ǹ������ĵ����ܳ�����Ϊ�䷵��ֵ��</li>
<li>��ע������ӳ���ķ���ֵ������Ϊ <code>long long</code>��</li>
</ul>
<h2>����</h2>
<p>������������ <code>min_total_length([1, 2, 3, 7], [0, 4, 5, 9, 10])</code>��</p>
<p>���µ�ͼ�����������е����ݡ�</p>
<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/321/wiring.png" alt="��������"></p>
<ul>
<li>ͼ����ˮƽ�ķ�ʽ��ʾ����ص�ͨѶ����</li>
<li>����Ŀ��ӡ�Ǻڰ�ɫ�ģ����Ժ�ɫ�ӵ��Խ���ɫ����ʾ������ɫ�ӵ��Խ�ǳɫ����ʾ��</li>
<li>ͼ���� $4$ ����ɫ�����ӵ㣬��λ�÷ֱ�Ϊ $1,2,3$ �� $7$��</li>
<li>ͼ���� $5$ ����ɫ�����ӵ㣬��λ�÷ֱ�Ϊ $0,4,5,9$ �� $10$��</li>
<li>���������Ž�ĵ����ܳ���Ϊ $1+2+2+2+3=10$�������ӳ���ķ���ֵΪ $10$��</li>
<li>ע�⹲����������������λ��Ϊ $7$ �����ӵ��ϡ�</li>
</ul>
<h2>���ݷ�Χ</h2>
<ul>
<li>$1\leq n,m\leq 100\ 000$</li>
<li>$0\leq r[i]\leq 10^9 $���������� $0 \leq i \leq n-1$��</li>
<li>$0\leq b[i]\leq 10^9 $���������� $0 \leq i \leq m-1$��</li>
<li>���� $r$ �� $b$ ���Ѿ��������ź���</li>
<li>������ $r$ �� $b$ ������ $n+m$ ��ֵ���ǲ�ͬ�ġ�</li>
</ul>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">������Լ��</th>
<th style="text-align:center;">��ֵ</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$n,m\leq 200$</td>
<td style="text-align:center;">$7$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">���к�ɫ�ӵ��λ������С���κ���ɫ�ӵ��λ������</td>
<td style="text-align:center;">$13$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">��ÿ $7$ �������������������ӵ��ڱ�������һ����ɫ�ӵ㼰һ����ɫ�ӵ�</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">���нӵ��� $[1,n+m]$ ��Χ���в�ͬ��λ������</td>
<td style="text-align:center;">$25$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">�޸�������</td>
<td style="text-align:center;">$45$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ������</strong>��$1\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$256\texttt{MB}$</p>
<h2>���ֳ�������</h2>
<p>���ֳ�����������������¸�ʽ�����ݣ�</p>
<ul>
<li>�� $1$ �У�$n,m$</li>
<li>�� $2$ �У�$r[0]\ r[1]\ ... \ r[n-1]$</li>
<li>�� $3$ �У�$b[0]\ b[1]\ ... \ b[m-1]$</li>
</ul>
<p>���ֳ������������������һ�����ݣ����溬�� <code>min_total_length</code> �ķ���ֵ��</p>
<h2>����</h2>
<p><a href="./20748/file/attachment.zip">�����������������������</a></p>
