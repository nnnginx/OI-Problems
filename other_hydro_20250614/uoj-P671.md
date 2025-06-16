<p>UOI ��Ȼ�ǳ��߼�������ʱ�Ϳ��Եõ��ɼ��������ڱ���������һɲ�ǣ�һ�����ǁ����������˴洢�ű����ɼ��Ļ�����漴������ʼð�̡�</p>
<p>���ǁ���������̱����˿���ס�ˣ���������ɼ��Ӹû�������������ָ����������ǁ�������Ի�·�Ƚ���֣����Իָ����ݵķ�ʽҲ�ǳ��Ĺ֡�</p>
<p>��һ��ʼ������������洢��һ���������� $a$��Ȼ��ÿһ�������������ȸ���һ������ $[l, r] (1 \leq l \leq r \leq n)$��Ȼ������������ֲ���֮һ��</p>
<ul>
<li><p>$1\ l\ r\ v$: ���� $v$, ���� $l \leq i \leq r$���� $a_i$ ��Ϊ $\lfloor \frac{a_i}{v} \rfloor$���������Ǳ�֤ $v \ge 1$��</p>
</li>
<li><p>$2\ l\ r\ v$: ���� $v$, ���� $l \leq i \leq r$���� $a_i$ ��Ϊ $a_i \&amp; v$������ $\&amp;$ �ǰ�λ�����㡣</p>
</li>
<li><p>$3\ l\ r$: ����ѯ�� $a_i$��$l \leq i \leq r$�����ܺ͡�</p>
</li>
</ul>
<p>��Ȼ�㲻̫��⁁�������ͨ����Ĳ��������㻹�ǹԹԵػش��Ł�������һ����ѯ�ʡ�������û�п������ÿ�һ���أ�</p>
<h2>�����ʽ</h2>
<p>��һ������������ $n, q$����ʾ���� $a$ �ĳ��Ⱥ�ѯ�ʸ�����</p>
<p>����һ�� $n$ ������ $a_i$��<strong>�� $16$ ���ƶ���</strong>��</p>
<p>���� $q$ �У�ÿ�е�һ�������� $op_i$ ��ʾ������š�</p>
<p>���� $op_i = 1$ �� $op_i = 2$����������������� $l_i, r_i, v_i$����ʾִ��������Ӧ����, <strong>���� $v_i$ �� $16$ ���ƶ���</strong>��</p>
<p>���� $op_i = 3$����������������� $l_i, r_i$����ʾѯ����������Ԫ�صĺͶ� $2^{128}$ ȡģ��ֵ��<strong>�� $16$ �������</strong>��</p>
<p>�ڱ��������е�ʮ�������� <strong> �������ַ� <code>0</code> $\sim$ <code>9</code>,<code>a</code> $\sim$ <code>f</code>���ֱ������ $0 \sim 9,10 \sim 15$</strong>��ͬʱ <strong>��������Чǰ����</strong> ����������� $16$ �������뱣֤�������ϸ�ʽ��ѡ�ֵ����Ҳ��Ҫ�������ϸ�ʽ��</p>
<p><strong>��ʾ: UOJ �п���ʹ�� $128$ λ�޷����������� <code>__uint128_t</code>������Ҫ�ֶ�ʵ�� IO�������ṩ�� IO ģ���������β��</strong></p>
<h2>�����ʽ</h2>
<p>�����У�����ÿ��ѯ�ʣ������𰸡�</p>


<pre><code class="language-input1">5 5
1 9 1 9 1
3 2 3
2 1 3 5
3 1 5
1 1 5 3
3 1 5
</code></pre>


<pre><code class="language-output1">a
d
3
</code></pre>

<h2>������</h2>
<p>�������ļ��� <code>ex_machine2.in</code> �� <code>ex_machine2.out</code>��</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_machine3.in</code> �� <code>ex_machine3.out</code>������������������ $2^{40}$��</p>
<h2>������Լ��</h2>
<p>���� $100\%$ �����ݣ�$1 \leq l_i \leq r_i \leq n \leq 300000, 1 \leq q \leq 200000, 0 \leq v_i, a_i \lt 2^{128}$�����в���һ�� $v_i \geq 1$��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">$n\le$</th>
<th style="text-align:center;">$q\le$</th>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">��ֵ</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$3000$</td>
<td style="text-align:center;">$3000$</td>
<td style="text-align:center;">��</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;" rowspan="4">$3\times 10^5$ </td>
<td style="text-align:center;" rowspan="4">$2\times 10^5$</td>
<td style="text-align:center;">$op_i \neq 2$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$l_i = 1, r_i = n$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$op_i \neq 1$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">��</td>
<td style="text-align:center;">$25$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ�����ƣ�$\texttt{3s}$</strong></p>
<p><strong>�ռ����ƣ�$\texttt{1GB}$</strong></p>
<h2>��ʾ</h2>
<p><strong>��ʾ����ע������㷨��ʱ�临�Ӷȡ�</strong></p>
<p><strong>��ʾ: UOJ �п���ʹ�� $128$ λ�޷����������� <code>__uint128_t</code>������Ҫ�ֶ�ʵ�� IO���������·��ṩ��ģ�塣</strong></p>
<pre><code class="sh_cpp">typedef __uint128_t u128;
inline u128 read() {
    static char buf[100];
    scanf("%s", buf);
    // std::cin &gt;&gt; buf;
    u128 res = 0;
    for(int i = 0;buf[i];++i) {
        res = res &lt;&lt; 4 | (buf[i] &lt;= '9' ? buf[i] - '0' : buf[i] - 'a' + 10);
    }
    return res;
}
inline void output(u128 res) {
    if(res &gt;= 16)
        output(res / 16);
    putchar(res % 16 &gt;= 10 ? 'a' + res % 16 - 10 : '0' + res % 16);
    //std::cout.put(res % 16 &gt;= 10 ? 'a' + res % 16 - 10 : '0' + res % 16);
}</code></pre>
