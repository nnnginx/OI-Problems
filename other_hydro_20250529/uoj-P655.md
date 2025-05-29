<p><strong>����һ�������⡣</strong></p>
<p>�����������ͨ�������ƽ����룬����Ҫ�ȵ� 2050 ���ˡ�</p>
<p>��ˣ������������ֱ���ƽ⿪����������Ϊ��Ч��</p>
<p>������������Ա���ʾΪһ�����ص� $n$ �׾��� $A$������Ԫ�ض��� $0\sim 998244352$ ֮���������</p>
<p>�������־����޷�ֱ�ӻ�ÿ������롣���ǿ���ͨ�� Linux ������©����ù����������Ϣ��</p>
<p>������˵��������򽻻���������ɴ�ѯ�ʣ�ÿ�θ�����������һ��Ԫ�ض��� $0\sim 998244352$ ֮�������� $n$ �׾��� $B$��������᷵�� $\det(A+B)$ �� $998244353$ ȡģ��ֵ����Ϊ��ȫ���ƣ������ֻ�ܽ��� $T$ ��ѯ�ʡ�</p>
<p>��������ǰ��������²��ԭ���ľ��� $A$�� </p>
<p>���� $\det(A)$ ��ʾ���� $A$ ������ʽ��</p>
<h2>����</h2>
<p><strong>����ֻ֧��C++��</strong></p>
<p>��������� <code>password.h</code> ͷ�ļ���</p>
<p>����Ҫʵ������Ĺ��̣�</p>
<pre><code class="sh_cpp">std::vector&lt;int&gt; solve(int n,int T);</code></pre>
<p>���� $n$ �Ǿ��� $A$ �Ľ�����$T$ ��������ѯ�ʴ���������Ҫ����һ������ǡΪ $n^2$ �� <code>vector</code>�����������г����� $A$ ������Ԫ�أ������±�Ϊ $(i-1)\times n+j-1$ ��λ��Ϊ���� $A$ �� $(i,j)$ λ��Ԫ�� $A_{i,j}$��</p>
<p>����Ե������¹��̺ͽ�������н�����</p>
<pre><code class="sh_cpp">int query(std::vector&lt;int&gt; vt);</code></pre>
<p>���� <code>vt</code> ��һ������ǡΪ $n^2$ �� <code>vector</code>�����������г�����θ����ľ��� $B$ ������Ԫ�أ������±�Ϊ $(i-1)\times n+j-1$ ��λ��Ϊ���� $B$ �� $(i,j)$ λ��Ԫ�� $B_{i,j}$��������᷵�� $\det(A+B)$ �� $998244353$ ȡģ��ֵ������뱣֤ <code>vt</code> ������Ԫ�ض��� $0\sim 998244352$ ֮���ҳ���Ϊ $n^2$����Ȼ������᷵�� $-1$ ����Ľ������̻ᱻ�ж�Ϊʧ�ܡ�������ֻ�ܵ��� $T$ �� <code>query</code> ������</p>
<h2>���ⷽʽ</h2>
<p>��������⽫�������¸�ʽ���������ݣ�</p>
<p>��һ�а������������� $n$ �� $T$����ʾ���� $A$ �Ľ�����������ѯ�ʴ�����</p>
<p>������ $n$ �У�ÿ�� $n$ �����������е� $i$ �е� $j$ ������Ϊ���� $A$ �� $(i,j)$ λ��Ԫ�� $A_{i,j}$��</p>
<p><strong>�����ղ����У����� $A$ ��ȷ���ģ�������Ϊ���ѯ�ʶ��ı䡣</strong></p>
<p>��������⽫������¸�ʽ��������ݣ�</p>
<p>����ÿһ�����ݣ��������ȷ�²���˾��� $A$ ��ѯ�ʴ���û�г������ƴ�������������ѯ�ʴ��� $cnt$���������� <code>Wrong Answer.</code>��</p>


<pre><code class="language-input1">1 1
2
</code></pre>


<pre><code class="language-output1">1
</code></pre>


<p>�����ֱ�ӵ��� <code>query([0])</code> ���õ� $\det(A)$������ $n=1$��������Ҳ�� $A$ ��Ψһһ��Ԫ�ء�</p>
<h2>���ݷ�Χ</h2>
<p>�����������ݣ�$1\leq n\leq 50,1\leq T\leq 8000,0\leq A_{i,j}\leq 998244352$��</p>
<p>��֤����Ľ�������������Ŀ���ƣ������ⲻ��ռ�ó��� $0.5\texttt{s}$ ʱ��� $32\texttt{MB}$ �ڴ档</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">$n\le$</th>
<th style="text-align:center;">$T=$</th>
<th style="text-align:center;">��ֵ</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$5$</td>
<td>$14$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$4$</td>
<td>$6$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$20$</td>
<td style="text-align:center;">$8000$</td>
<td>$24$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$50$</td>
<td style="text-align:center;">$2501$</td>
<td>$27$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$50$</td>
<td style="text-align:center;">$2500$</td>
<td>$29$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ������</strong>��$2\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./21056/file/attachment.zip">�����������������������</a></p>
