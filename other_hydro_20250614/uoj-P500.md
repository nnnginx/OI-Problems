<p>���� $n$ �ζ���ʽ</p>
<p>\begin{equation}
f(x) = \sum_{i=0}^{n} a_ix^i
\end{equation}</p>
<p>$Q$ ��ѯ�ʣ��� $i$ ��ѯ�� $f(q_i)$ �� $998244353$ ȡģ��ֵ��</p>
<h2>�����ʽ</h2>
<p><strong>���ڱ�������ݷ�Χ�ϴ����в��Ե��</strong> $q_i$ <strong>���ڳ��������ɡ�</strong></p>
<p>��һ���������� $n,Q$��$n,Q$ ���������Ŀ������</p>
<p>�ڶ��� $n+1$ ���������� $i$ ��������ʾ $a_{i-1}$</p>
<p>�������������� $q_0,q_{\mathrm{x}},q_{\mathrm{y}}$����ʾ $q_i$ �����ɷ�ʽ��</p>
<p>$q_i$ �������¹�������:</p>
<p>$\forall 1 \leq i \leq Q,q_i=(q_{i-1} \times q_{\mathrm{x}}+q_{\mathrm{y}})\bmod 998244353$</p>
<h2>�����ʽ</h2>
<p>���������ģ������ֻ��Ҫ�������ѯ�ʴ�ȡ��ģ֮��� $\mathbin{\mathrm{xor}}$ �ͼ��ɡ�</p>


<pre><code class="language-input1">2 2
1 2 3
1 2 1
</code></pre>


<pre><code class="language-output1">128
</code></pre>


<p>$q_1=2 \times q_0 +1=3$</p>
<p>$q_2=2 \times q_1 +1=7$</p>
<p>�� $=(1+2 \times 3+ 3 \times 3^2) \mathbin{\mathrm{xor}} (1+2 \times 7+3 \times 7^2)=34 \mathbin{\mathrm{xor}} 162=128$</p>
<h2>������</h2>
<p>��������������</p>
<h2>���ݷ�Χ</h2>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���԰����</th><th>$n\leq $</th><th>$Q \leq$</th><th>$�������� $</th><th>��ֵ</th></tr></thead><tbody><tr><td>$1$</td><td>$1000$</td><td>$1000$</td><td rowspan="3">��</td><td>$5$</td></tr><tr><td>$2$</td><td>$10^5$</td><td>$10^5$</td><td>$15$</td></tr><tr><td>$3$</td><td rowspan="4">$2.5 \times 10^5$</td><td>$2.5 \times 10^5$</td><td>$15$</td></tr><tr><td>$4$</td><td rowspan="2">$5 \times 10^5$</td><td>$q_{\mathrm{y}}=0$</td><td>$25$</td></tr><tr><td>$5$</td><td rowspan="2">��</td><td>$25$</td></tr><tr><td>$6$</td><td>$10^6$</td><td>$15$</td></tr></tbody></table></div>

<p>�������в������ݣ����� $1 \leq n \leq 2.5 \times 10^5, 1 \leq Q \leq 10^6, 2 \leq q_{\mathrm{x}} &lt; 998244353, 0 \leq q_0,q_{\mathrm{y}} &lt; 998244353$��</p>
<p><strong>ʱ������</strong>��$\texttt{1s}$</p>
<p><strong>�ռ�����</strong>��$\texttt{512MB}$</p>
<h2>����</h2>
<p><a href="./20905/file/attachment.zip">������������</a></p>
