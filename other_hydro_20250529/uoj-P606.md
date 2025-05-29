<p><strong>����һ�������⡣</strong></p>
<p><strong>����ĳЩԭ�����֧�� C++, C++11 ���Ե��ύ��</strong></p>
<p>��Ϊ�Ļ��δ�ʦ��skip �鱻�����ѧ����μ������ѧ�ٰ������Ӫ��</p>
<p>������Ӫ�У�skip ��˳����ͨ���˿��ԣ����������ԡ��������У����Կ��ٸ��� skip ��һ�����ѵ����⡣skip ����Ҫ�³����Թ���������� $3$ ���Ǹ����� $a,b,c$ �����Թ����ʼ���� skip ��һ�������� $n$ ����ʾ $a,b,c$ �������� $[0,n]$ �С�skip ��ÿ�ο��Ը������Թ������Ǹ����� $x,y,z$ ���� $0\leq x,y,z\leq n$ �����Թٻ�ش��� $|a+b-x-y|+|b+c-y-z|+|c+a-z-x|$ ��ֵ������ skip ����Ҫͨ�������ٵ�ѯ�ʵõ����Թ�������� $3$ ���������Թ�Ϊ��ȷ�� skip �鲻��Ϲ���ɶԵģ���������� $a,b,c$ �� skip ��ȥ�¡�</p>
<h2>����</h2>
<p>��������� <code>head.h</code> ͷ�ļ���</p>
<p>����Ҫʵ������Ĺ��̣�</p>
<pre><code class="sh_cpp">void work(int N,int tp,int &amp;a,int &amp;b,int &amp;c);</code></pre>
<p>���� $N$ �����Թٸ����� $n$ ��ֵ�� $tp$ �������ݵ�����һ�����ݣ�����ܲ���Ҫ�õ�����������Ҫ�����µ��������ֱ�д�� $a,b,c$ �С�</p>
<p>����Ե������¹��̺ͽ�������н�����</p>
<pre><code class="sh_cpp">int query(int x,int y,int z);</code></pre>
<p>���� $x,y,z$ �������Թ������������������Ǹ����������� $|a+b-x-y|+|b+c-y-z|+|c+a-z-x|$ ��ֵ������뱣֤ $0\leq x,y,z\leq n$ ����Ȼ������᷵�� $-1$ ������β²�ᱻ��Ϊʧ�ܡ�</p>
<h2>���ⷽʽ</h2>
<p>��������⽫�������¸�ʽ���������ݣ�</p>
<p>��һ�а������������� $T$ �� $tp$����ʾ���Թ��� skip ��µĴ����������ݵ�����һ�����ݣ�����Ϊ $0$ ����</p>
<p>������ $T$ �У�ÿ��������� $N_i,a_i,b_i,c_i,Q_i$ ���ֱ���� $n$ �Ĵ�С�����Թ���������� $3$ �������� skip �����ѯ�ʶ��ٴΡ�</p>
<p><strong>�����ղ����У����Թ���������� $a,b,c$ ��ȷ���ģ�������Ϊ���ѯ�ʶ��ı䡣</strong></p>
<p>��������⽫������¸�ʽ��������ݣ�</p>
<p>����ÿһ�����ݣ��������ȷ������ $a,b,c$ ��ֵ��ѯ�ʴ���û�г������ƴ����������һ��һ���� $1$ ����������һ��һ���� $0$ ��</p>


<pre><code class="language-input1">1 0
4 1 2 3 3
</code></pre>


<pre><code class="language-output1">1
</code></pre>

<h2>���ݷ�Χ</h2>
<p>���� $100\%$ �����ݣ� $1\leq T\leq 10^5,1\leq n\leq 10^8,3\leq Q\leq 1000$ ��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">���Ե���</th>
<th style="text-align:center;">$tp=$</th>
<th>$T=$</th>
<th>$n$</th>
<th>$Q=$</th>
<th>��������</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1\sim 2$</td>
<td style="text-align:center;">$1$</td>
<td>$100$</td>
<td>$=9$</td>
<td>$1000$</td>
<td rowspan="3">��</td>
</tr>
<tr>
<td style="text-align:center;">$3\sim 5$</td>
<td style="text-align:center;">$2$</td>
<td>$100000$</td>
<td>$\leq 10^8$</td>
<td>$4$</td>
</tr>
<tr>
<td style="text-align:center;">$6\sim 9$</td>
<td style="text-align:center;">$3$</td>
<td>$100000$</td>
<td>$=4$</td>
<td>$3$</td>
</tr>
<tr>
<td style="text-align:center;">$10\sim 13$</td>
<td style="text-align:center;">$4$</td>
<td>$100000$</td>
<td>$\leq 10^8$</td>
<td>$3$</td>
<td>$A$</td>
</tr>
<tr>
<td style="text-align:center;">$14\sim 20$</td>
<td style="text-align:center;">$5$</td>
<td>$100000$</td>
<td>$\leq 10^8$</td>
<td>$3$</td>
<td>��</td>
</tr>
</tbody>
</table>
</div>
<p>$A$ ����֤ $a,b,c$ �� $[0,n]$ �ھ����������ֻҪ���������Թ���Ĵ����в¶��������� $40\%$ ���ɵ÷֡�</p>
<p><strong>ʱ������</strong>��$1\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$1\texttt{GB}$</p>
<h2>����</h2>
<p><a href="./21010/file/attachment.zip">������������</a></p>
