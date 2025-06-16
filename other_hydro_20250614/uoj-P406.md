<p>��Ҫ��һ�������δ�����ٰ���ʱ�̱������ô������� $HW$ ����λ��$H$ �� $W$ �У����еı���Ǵ� $0$ �� $H-1$���еı���Ǵ� $0$ �� $W-1$��λ�� $r$ �� $c$ �е���λ�� $(r,c)$ ��ʾ��һ�������� $HW$ λ�����ߣ�����Ǵ� $0$ �� $HW-1$�����ƶ�����һ����λ���� $i$��$0\le i\le HW-1$���������߱����ŵ���λ $(R_i,C_i)$����λ���в����ߺ���λ��һһ��Ӧ�ġ�</p>
<p>������һ����λ���� $S$ ����Ϊ�ǳ����εģ������������ $r_1,r_2,c_1$ �� $c_2$ ��������������</p>
<ul><li>$0\le r_1\le r_2\le H-1$��</li>
<li>$0\le c_1\le c_2\le W-1$��</li>
<li>$S$ �������������� $r_1\le r\le r_2$ �� $c_1\le c\le c_2$ ����λ $(r,c)$ �ļ��ϡ�</li>
</ul><p>���һ����������λ���ϰ��� $k$��$1\le k\le HW$������λ�����ұ����䵽������ϵĲ����ߵı��ǡ���Ǵ� $0$ �� $k-1$����ô�ü�����<strong>�����</strong>��һ����λ���<strong>�����</strong>����Ϊ�����������ĳ�������λ���ϵĸ�����</p>
<p>��׼������λ�������յ�һЩ����������������λ�����󡣾�����˵���� $Q$ �����������󣬰�ʱ��˳����Ϊ $0$ �� $Q-1$���� $j$��$0\le j\le Q-1$��������ϣ������������ $A_j$ �� $B_j$ ����λ������������ÿ�����󲢸�����λ��ÿ�θ��º����Ŀ���Ǽ��㵱ǰ��λ�������ȡ�</p>
<h2>ʵ��ϸ��</h2>
<p>��Ӧ��ʵ�����й��̺ͺ�����</p>
<pre><code class="sh_cpp">give_initial_chart(int H, int W, int[] R, int[] C)</code></pre>
<ul><li><code>H</code>, <code>W</code>������������</li>
<li><code>R</code>, <code>C</code>����������Ϊ $HW$ �����飬�����ʼ����λ��</li>
<li>�������ֻ������һ�Σ��������� <code>swap_seats</code> ���κε���֮ǰ��</li>
</ul><pre><code class="sh_cpp">int swap_seats(int a, int b)</code></pre>
<ul><li>�ú�����������һ�ν�����λ������</li>
<li><code>a</code>, <code>b</code>����Ҫ������λ�Ĳ�����</li>
<li>�ú��������� $Q$ ��</li>
<li>�ú���Ӧ���ؽ�����λ����λ��������</li>
</ul><h2>����</h2>
<p>�� $H=2$��$W=3$��$R=[0,1,1,0,0,1]$��$C=[0,0,1,1,2,2]$���� $Q=2$��</p>
<p>��������ȵ��� <code>give_initial_chart(2, 3, [0, 1, 1, 0, 0, 1], [0, 0, 1, 1, 2, 2])</code>��</p>
<p>�������λ�����£�</p>
<p>\begin{matrix}
0 &amp; 3 &amp; 4 \\
1 &amp; 2 &amp; 5
\end{matrix}</p>
<p>�������������� <code>swap_seats(0, 5)</code>����������Ϊ $0$ ��������ɺ���λ���ɣ�</p>
<p>\begin{matrix}
5 &amp; 3 &amp; 4 \\
1 &amp; 2 &amp; 0
\end{matrix}</p>
<p>��Ӧ�����߼��� $\{0\},\{0,1,2\}$ �� $\{0,1,2,3,4,5\}$ ��������λ���϶��ǳ����κ�����ġ����ԣ�����λ��������Ϊ $3$��<code>swap_seats</code> Ӧ�÷��� $3$��</p>
<p>������������ٴε��� <code>swap_seats(0, 5)</code>����������Ϊ $1$ ��������ɺ���λ��ص���ʼ״̬����Ӧ�����߼��� $\{0\},\{0,1\},\{0,1,2,3\}$ �� $\{0,1,2,3,4,5\}$ ���ĸ���λ���϶��ǳ����κ�����ġ����ԣ��ñ�������Ϊ $4$��<code>swap_seats</code> Ӧ�÷��� $4$��</p>
<p>���������������е��ļ�<code>ex_seats1.in</code>��<code>ex_seats1.out</code>��Ӧ���������ӡ����⣬�������ݰ��л���һЩ����������������ӡ�</p>
<h2>��������</h2>
<ul><li>$1\le H$</li>
<li>$1\le W$</li>
<li>$HW\le 1\ 000\ 000$</li>
<li>$0\le R_i\le H-1$��$0\le i\le HW-1$��</li>
<li>$0\le C_i\le W-1$��$0\le i\le HW-1$��</li>
<li>$(R_i,C_i)\ne(R_j,C_j)$��$0\le i&lt;j\le HW-1$��</li>
<li>$1\le Q\le 50\ 000$</li>
<li>���� <code>swap_seats</code> �����е��ã�$0\le a\le HW-1$</li>
<li>���� <code>swap_seats</code> �����е��ã�$0\le b\le HW-1$</li>
<li>���� <code>swap_seats</code> �����е��ã�$a\ne b$</li>
</ul><h2>������</h2>
<ol><li>��5�֣�$HW\le 100$��$Q\le 5\ 000$</li>
<li>��6�֣�$HW\le 10\ 000$��$Q\le 5\ 000$</li>
<li>��20�֣�$H\le 1\ 000$��$W\le 1\ 000$��$Q\le 5\ 000$</li>
<li>��6�֣� ���� <code>swap_seats</code> �����е��ã�$Q\le 5\ 000$��$|a-b|\le 10\ 000$ </li>
<li>��33�֣�$H=1$</li>
<li>��30�֣��޸�����������</li>
</ol><h2>�������ʾ��</h2>
<p>�������ʾ���������¸�ʽ��������</p>
<ul><li>�� $1$ �У�$H\ W\ Q$</li>
<li>�� $2+i$ �У�$0\le i\le HW-1$�� : $R_i\ C_i$</li>
<li>�� $2+HW+j$ �У�$0\le j\le Q-1$����$A_j\ B_j$</li>
</ul><p>���� $A_j$ �� $B_j$ �ǵ��� <code>swap_seats</code> ��������ʱ�Ĳ�����</p>
<p>�������ʾ���������¸�ʽ��ӡ��Ĵ𰸣�</p>
<ul><li>�� $1+j$ �У�$0\le j\le Q-1$����<code>swap_seats</code> �������� $j$ �ķ���ֵ</li>
</ul><h2>Լ��������</h2>
<p>������֧�ֵĸ��ֱ�����ԣ������г��˶�Ӧ���������͡������������͵�ϸ�ڵȣ��μ�ʵ��ʾ����</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>����</th>
<th>$\texttt{int}$</th>
<th>$\texttt{int64}$</th>
<th>$\texttt{int[]}$</th>
<th>����$a$�ĳ���</th>
<th>$\texttt{string}$</th>
</tr></thead><tbody><tr><td>$\texttt{C++}$</td><td>$\texttt{int}$</td><td>$\texttt{long long}$</td><td>$\texttt{std::vector&lt;int&gt;}$</td><td>$\texttt{a.size()}$</td><td>$\texttt{std::string}$</td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�</strong>$3\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$268\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20811/file/attachment.zip">������������</a></p>
