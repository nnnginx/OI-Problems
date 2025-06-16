<p>������ 01 ��ϲ���ӷ���Ҳ��ϲ��������㣨�� C/C++ ��� <code>^</code> ���������������һ���Դ��������������һ��������ˣ�</p>
<p>����һ������ $b_1, \dots, b_m$����ϣ���㽫���� $b$ ����Ϊ $k$ �������ǿ������У�ʹ��ÿһ�ε�����֮����С����������֪������������ $0 = p_0 &lt; p_1 &lt; \cdots &lt; p_k = m$ ���������� $p$ ����ʽ����Сֵ��
$$
\sum_{i=1}^{k} (b_{p_{i-1} + 1} \mathbin{\mathrm{xor}} \cdots \mathbin{\mathrm{xor}} b_{p_i})
$$
�����Сֵ����Ϊ������е�<strong>����ֵ</strong>��</p>
<p>�����������ǳ��򵥣����ǳ����� 01 ������һ������ǡ��Ϊ $n$ �ķǸ��������� $a_1, \dots, a_n$�����뿼���㣬$a$ ��ÿ��ǰ׺ $a_1, \dots, a_j$ ��$k \le j \le n$��������ֵ�ֱ��Ƕ����أ�</p>
<h2>�����ʽ</h2>
<p>��һ������������ $n,k$������ͬ���档</p>
<p>������һ�� $n$ ���Ǹ��������� $i$ ���Ǹ�������ʾ $a_i$��</p>
<h2>�����ʽ</h2>
<p>��һ�� $n-k+1$ ���������ֱ��ʾǰ $j = k, k+1, \dots, n$ ��Ԫ����ɵ����е�����ֵ��</p>


<pre><code class="language-input1">6 2
1 1 4 5 1 4
</code></pre>


<pre><code class="language-output1">2 4 1 0 4
</code></pre>


<p>�������� $a_1, \dots, a_6$,���Խ����л���Ϊ $a_1, a_2$ �� $a_3, a_4, a_5, a_6$ ���Ρ�</p>
<p>��ʱ��Ϊ $(1 \mathbin{\mathrm{xor}} 1)+(4 \mathbin{\mathrm{xor}} 5 \mathbin{\mathrm{xor}} 1 \mathbin{\mathrm{xor}} 4)=0+4=4$��</p>
<p>ע�� $a_1, a_2, a_3, a_4, a_5$ �� $a_6$ Ҳ��һ�ֺϷ��Ļ��ַ�����</p>
<h2>������</h2>
<p>���·��ļ���</p>
<p>���ݷ�Χͬ���Ե� 3 ~ 4��</p>
<h2>������Լ��</h2>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th><th>$n$</th><th>��������</th></tr></thead><tbody><tr><td>1 ~ 2</td> <td>$\le 15$</td>  <td rowspan="2">��</td></tr><tr><td>3 ~ 4</td> <td>$\le 5000$</td> </tr><tr><td>5 ~ 6</td> <td rowspan="3">$\le 60000$</td> <td>$a_i \lt 2^8$</td> </tr><tr><td>7 ~ 8</td> <td>$a_i \lt 2^{12}$</td> </tr><tr><td>9 ~ 10</td> <td>��</td> </tr></tbody></table></div>

<p>�������в��Ե㣬���� $1 \le k \le n \le 60000, k \le 8,a_i &lt; 2^{16}$</p>
<p><strong>ʱ������</strong>��$2\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20953/file/attachment.zip">������������</a></p>
