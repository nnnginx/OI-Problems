<p>UOI ��������һ�����ǰ�צ���ý�д�ġ�</p>
<p>��������д�ĺܲ��D�ײ��ò�����������ȷ�����⡣�����ǰ�צ��û���ֻظ���ֻ�ý�������æ��</p>
<p>��Щ������Գ����һ��ջ�Ľṹ����ʼΪ�գ���D�������ֲ�����</p>
<ul>
<li><code>push</code>������һ����������ջ������ʱ����Ҫ�����������������ֻ�Ӧ֮һ��R��no Response���� B��Buzhidao����</li>
<li><code>pop</code>����D���ں����ύ��֪����ջ������Ĵ𰸣������ջ���Ƴ���</li>
</ul>
<p>��Щ������ʱ��˳���γ���һ����Ϊ $2k$ �Ĳ������У���֤�������кϷ������������в�����ջ��û��Ԫ�ء�</p>
<p>����Ҫ��֤����ʱ��ջ�� R ���Ӧ���������� $c_r$��B ���Ӧ���������� $c_b$������ᱻ��D�׷����������صġ�</p>
<p>���ֻ�Ӧ���ܷ��ܣ�B ���Ӧ�����˷�ŭ��������������Ӧ�����У������� $p_r$ �� R ���Ӧ��$p_b$ �� B ���Ӧ����D�׵ķ�ŭֵ���� $p_rp_b^2$��</p>
<p>���ڣ�����֪�����л�Ӧ�����д�D�׷�ŭֵ���ܺ͡��𰸿��ܴܺ���ֻ��Ҫ������ $998244353$ ȡģ�Ľ����</p>
<h2>�����ʽ</h2>
<p>��һ���������� $k,c_r,c_b$����ʾ�������г��ȡ�ջ�� R ���Ӧ�������ơ�ջ�� B ���Ӧ�������ơ�</p>
<p>������ $2k$ ��ÿ��һ��Ϊ <code>push</code> �� <code>pop</code> ���ַ����������������С�</p>
<h2>�����ʽ</h2>
<p>���һ��һ����������ʾ���л�Ӧ�����д�D�׷�ŭֵ���ܺͶ� $998244353$ ȡģ��Ľ����</p>


<pre><code class="language-input1">3 1 2
push
push
push
pop
pop
pop
</code></pre>


<pre><code class="language-output1">12
</code></pre>


<p>���ڲ����������ȷ������������������Ƴ�������Ҫ�������ظ���ǡ���� $1$ ���� R��$2$ ���� B���ܹ��� $\binom{3}{2} = 3$ ��������ÿ�������ķ�ŭֵ���� $1 \times 2^2 = 4$�����Դ�Ϊ $3 \times 4 = 12$��</p>


<pre><code class="language-input2">3 1 2
push
push
pop
push
pop
pop
</code></pre>


<pre><code class="language-output2">14
</code></pre>


<p>����һ������ص��� R����ʣ���������ⶼֻ��ѡ��� B���ܹ��� $1$ �ַ�����ȨֵΪ $1 \times 2^2 = 4$��</p>
<p>����һ������ص��� B����ʣ����������û�����ơ�</p>
<ul>
<li>�������ζ��� B������ $1$ �ַ�����ȨֵΪ $0 \times 3^2 = 0$��</li>
<li>�������ζ��� R������ $1$ �ַ�����ȨֵΪ $2 \times 1^2 = 2$��</li>
<li>�������λ�Ӧ��ͬ������ $2$ �ַ�����ȨֵΪ $1 \times 2^2 = 4$��</li>
</ul>
<p>�������з����ķ�ŭֵ��Ϊ $1 \times 4 + 1 \times 0 + 1 \times 2 + 2 \times 4 = 14$��</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_stack3.in</code> �� <code>ex_stack3.out</code>�������������������� 1 �����ʡ�</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_stack4.in</code> �� <code>ex_stack4.out</code>�������������������� 3 �����ʡ�</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_stack5.in</code> �� <code>ex_stack5.out</code>�������������������� 5 �����ʡ�</p>
<h2>������Լ��</h2>
<p>���� $100\%$ �����ݣ�$1 \leq k \leq 2500, 0 \leq c_r,c_b \leq k$����֤�������кϷ������������в�����ջ��û��Ԫ�ء�</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">$k\le$</th>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">��ֵ</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$20$</td>
<td style="text-align:center;" rowspan="4">��</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$40$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$80$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$250$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;" rowspan="3">$2500$</td>
<td style="text-align:center;">$c_r = 1$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$c_r=c_b=k$</td>
<td style="text-align:center;">$5$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">��</td>
<td style="text-align:center;">$15$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ�����ƣ�$\texttt{1s}$</strong></p>
<p><strong>�ռ����ƣ�$\texttt{512MB}$</strong></p>
