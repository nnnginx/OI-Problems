<p>��������ɹ�����˹���ԱȨ�ޣ��������� Skip ���Ȩ�ޣ������� UOJ �Ͻ������꣬������ʡ������ Rating ǿ�ƿ�$100$��</p>
<p>��������ڼ�����ʱ������ Skip ����Ȩ���ڼ䣬һλ�Ȱ��߶����� Picks �� OJ �ϴ���һ��û�� std ����Ŀ��</p>
<p>��Ϊ֮ǰ����Ϊ��������ߣ������� Picks �ܾ����������͸¶����Ľⷨ�������������׼������ ULR #2 ȱһ���⣬���ܰ�����������⿪���������� ULR �ĳﱸ��</p>
<p>����һ������Ϊ $n$ �Ĳ������С������� 4 �֣�</p>
<ol>
<li><code>| x</code>�����Ǹ����� $v$ ��Ϊ $v\ \mathrm{bitor}\ x$������ $\mathrm{bitor}$ Ϊ��λ�������</li>
<li><code>&amp; x</code>�����Ǹ����� $v$ ��Ϊ $v\ \mathrm{bitand}\ x$������ $\mathrm{bitand}$ Ϊ��λ�������</li>
<li><code>^ x</code>�����Ǹ����� $v$ ��Ϊ $v\ \mathrm{bitxor}\ x$������ $\mathrm{bitxor}$ Ϊ��λ��������</li>
<li><code>+ x</code>�����Ǹ����� $v$ ��Ϊ $(v + x) \bmod 2^{32}$��<strong>��һ�ֲ�����֤ $x=1$��</strong></li>
</ol>
<p>���в����� $x$ ��Ϊ��������ķǸ�������ÿһ�������� $x$ ����һ����ͬ�������� $0$ ��ʼ��š�</p>
<p>���� $q$ ��ѯ�ʣ�ÿ�θ������� $v,l,r,t$������� $v$ ���ν��в������������� $[l,r]$ �еĲ�����д�ɶ�������ʽ���ӵ͵��ߵ� $t+1$ ��������λ������ʾ $2^t$ ��λ����ֵ�����׷���ÿ��ѯ�ʵĴ�ֻ�п����� $0$ �� $1$��</p>
<p><strong>���ⲿ��������ǿ�����ߣ���������ʽ��������Լ�����֡�</strong></p>
<h2>�����ʽ</h2>
<p>��һ���������� $n,q,op$ ��ʾ�������г��ȡ�ѯ�ʸ�����ѯ�ʽ��ܲ�����</p>
<p>������ $n$ �������������������е�ÿ��Ԫ�ء�ÿ��һ���ַ� $c$ ��ʾ�������ͣ����һ������ $x$ ��ʾ����������<strong>���� <code>+</code> ������֤ $x=1$��</strong></p>
<p>������ $q$ ��ÿ���ĸ����� $v',l',r',t'$ ��ʾһ��ѯ�ʡ�<strong>ע��ѯ�ʽ����˼���</strong>�����ܷ������£�</p>
<ul>
<li>����Ҫ���ܵ�ѯ��Ϊ�� $t$ ��ѯ�ʣ�$ans_i$ ��ʾ�� $i$ ��ѯ�ʵĴ𰸣�ѯ�ʴ� $0$ ��ʼ��ţ� </li>
<li>���� $\mathrm{key} = op \times (\sum_{i=0}^{t-1} 2^ians_i) \mod 998244353$�� </li>
<li>���Ӧѯ�ʵ���ʵ�������£�
\begin{align}
  v &amp;= (v' + \mathrm{key})\bmod 2^{32} \\
 l &amp;= \min\{(l'\ \mathrm{bitxor}\ \mathrm{key})\bmod n,(r'\ \mathrm{bitxor}\ \mathrm{key})\bmod n\} \\
 r &amp;= \max\{(l'\ \mathrm{bitxor}\ \mathrm{key})\bmod n,(r'\ \mathrm{bitxor}\ \mathrm{key})\bmod n\} \\
 t &amp;= (t'\ \mathrm{bitxor}\ \mathrm{key}) \bmod 32
\end{align}</li>
</ul>
<p><strong>ע����ܹ����� $v$ �ļ��㷽ʽ���������߲�ͬ��ע������ѯ���Ƿ�ǿ�����߶���Ҫ����ѯ�ʽ��ܡ�</strong></p>
<h2>�����ʽ</h2>
<p>һ��һ������Ϊ $q$ �� 01 �ַ��������е� $i$ ���ַ���ʾ�� $i$ ��ѯ�ʵĴ𰸡�</p>


<pre><code class="language-input1">6 6 0
^ 17
+ 1
^ 28
| 6
&amp; 29
+ 1
3 0 2 1
8 1 5 3
7 1 4 0
12 0 4 2
31 0 2 1
50 1 2 0
</code></pre>


<pre><code class="language-output1">100111
</code></pre>


<ul>
<li>��һ��ѯ������ $3 \xrightarrow[]{\mathrm{bitxor}\ 17} 18 \xrightarrow[]{+1} 19 \xrightarrow[]{\mathrm{bitxor}\ 28} 15 = (1111)_2$�����ʾ $2^1$ �Ķ�����λ���������������� $2$ ��������λ��ֵΪ $1$���ʵ�һ��ѯ�ʴ�Ϊ $1$��</li>
<li>�ڶ���ѯ������ $8 \xrightarrow[]{+1} 9 \xrightarrow[]{\mathrm{bitxor}\ 28} 21 \xrightarrow[]{\mathrm{bitor}\ 6} 23 \xrightarrow[]{\mathrm{bitand}\ 29} 21 \xrightarrow[]{+1} 22 = (10110)_2$�����ʾ $2^3$ �Ķ�����λ���������������� $4$ ��������λ��ֵΪ $0$���ʵڶ���ѯ�ʴ�Ϊ $0$��</li>
</ul>


<pre><code class="language-input2">6 6 1
^ 17
+ 1
^ 28
| 6
&amp; 29
+ 1
3 13674554 3172638 395059201
7 6992286 3863695438 3302730626
6 122315987 1653449004 2270895617
11 277356193 306830369 65457603
22 2313889149 858796667 36414120
25 4135467483 3048814434 3407639193
</code></pre>


<pre><code class="language-output2">100111
</code></pre>


<p>���������ܺ�Ϊ����һ��</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_sequence3.in</code> �� <code>ex_sequence3.ans</code>�������������������� $1$ �����ʡ�</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_sequence4.in</code> �� <code>ex_sequence4.ans</code>�������������������� $3$ �����ʡ�</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_sequence5.in</code> �� <code>ex_sequence5.ans</code>�������������������� $6$ �����ʡ�</p>
<h2>������Լ��</h2>
<p>���� $100\%$ �����ݣ�$1 \leq n \leq 10^5 , 1 \leq q \leq 6 \times 10^5 , 0 \leq op \leq 1, 0 \leq x,v',l',r',t' &lt; 2^{32}$����֤������Ϊ <code>+</code> ����ʱ $x=1$��</p>
<table class="table table-bordered table-text-center table-vertical-middle">
<thead><tr><th>��������</th><th>$n \leq $</th><th>$q \leq $</th><th>$op \leq $</th><th>��������</th><th>��ֵ</th></tr></thead>
<tbody>
<tr><td>$1$</td><td>$3000$</td><td>$5000$</td><td>$1$</td><td>��</td><td>$2$</td></tr>
<tr><td>$2$</td><td>$4 \times 10^4$</td><td>$2 \times 10^5$</td><td>$0$</td><td>ֻ�� ^,+ ����</td><td>$8$</td></tr>
<tr><td>$3$</td><td>$4 \times 10^4$</td><td>$2 \times 10^5$</td><td>$1$</td><td>ֻ�� ^,+ ����</td><td>$14$</td></tr>
<tr><td>$4$</td><td>$10^5$</td><td>$4 \times 10^5$</td><td>$1$</td><td>ֻ�� ^,+ ����</td><td>$16$</td></tr>
<tr><td>$5$</td><td>$10^5$</td><td>$6 \times 10^5$</td><td>$1$</td><td>û�� + ����</td><td>$6$</td></tr>
<tr><td>$6$</td><td>$4 \times 10^4$</td><td>$2 \times 10^5$</td><td>$0$</td><td>��</td><td>$10$</td></tr>
<tr><td>$7$</td><td>$10^5$</td><td>$4 \times 10^5$</td><td>$0$</td><td>��</td><td>$10$</td></tr>
<tr><td>$8$</td><td>$4 \times 10^4$</td><td>$2 \times 10^5$</td><td>$1$</td><td>��</td><td>$14$</td></tr>
<tr><td>$9$</td><td>$10^5$</td><td>$6 \times 10^5$</td><td>$1$</td><td>��</td><td>$20$</td></tr>
</tbody></table>

<p><strong>���������ж��������ļ���СԼΪ $\texttt{30MB}$����ע���㷨����������ٶȶ�����ʱ�������Ӱ�졣</strong></p>
<p><strong>ʱ�����ƣ�$\texttt{2s}$</strong></p>
<p><strong>�ռ����ƣ�$\texttt{512MB}$</strong></p>
<h2>����</h2>
<p><a href="./21060/file/attachment.zip">������������</a></p>
