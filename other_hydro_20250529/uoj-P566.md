<p><strong> ����ĳЩԭ�����֧�� C++, C++11 ���Ե��ύ�� </strong></p>
<p>Ringo ���ڲμ����¼��¾ٰ��һ�����껪������Ŀڴ���װ��һЩ��ȯ����Щ��ȯ�����ڼ��껪����Ϸչλʹ�á����蹲�� $n$ ����ɫ�Ľ�ȯ��ÿ�Ž�ȯͿ�������е�һ����ɫ����ӡ����һ���Ǹ���������ͬ��ȯ�ϵ����ֿ�����ͬ�����ݼ��껪��Ĺ���Ҫ��$n$ ��֤��ż����</p>
<p>Ringo ÿ����ɫ�Ľ�ȯ�� $m$ �ţ�Ҳ����˵������ $n\cdot m$ �Ž�ȯ�����У��� $i$ ����ɫ��Ӧ�ĵ� $j$ �Ž�ȯ��ӡ������Ϊ $x_{i,j}$��$0\le i\le n-1$ �� $0\le j\le m - 1$����</p>
<p>һ�ν�ȯ��ϷҪ���� $k$ �֣��ִε���Ŵ� $0$ �� $k-1$��ÿһ�ְ�������ķ�ʽ���У�</p>
<ul><li><p>���ȣ�Ringo ��ÿ����ɫ�Ľ�ȯ�и�ѡ��һ�Ž�ȯ���γ�һ�� $n$ �Ž�ȯ��<strong>����</strong>��</p>
</li>
<li><p>�����Ϸ�����˼�¼����������н�ȯ�ϵ����� $a_0, a_1, \dots, a_{n-1}$������Ҫ������ $n$ ��������˳��</p>
</li>
<li><p>����������Ϸ�����˴�һ�����˳齱���г�ȡһ�����⿨Ƭ������ӡ������ $b$��</p>
</li>
<li><p>��������������ÿһ����ȯ�ϵ����� $a_i(0\le i \le n-1)$����Ϸ�����˻���� $a_i$ �� $b$ �Ĳ�ľ���ֵ���� $S$ ������ $n$ ����ľ���ֵ֮�͡�</p>
</li>
<li><p>���õ������� $S$ ���� Ringo �����ܹ���õĽ������</p>
</li>
<li><p>һ����Ϸ�����󣬱��ּ����еĽ�ȯȫ����������������δ�����ִ���ʹ�á�</p>
</li>
</ul><p>�� $k$ ����Ϸ������Ringo �ᶪ���ڴ��е����н�ȯ��</p>
<p>ͨ����ϸ�۲죬Ringo ���������ȯ��Ϸ���ٿ��ˣ�ʵ���ϣ����˳齱������������һ̨��ӡ������ÿһ�֣���Ϸ�����������ҵ�һ���ܹ���С����ǰ�ִ���Ϸ���������� $b$��Ȼ�󽫸����ִ�ӡ��������ȡ�����⿨Ƭ�ϡ�</p>
<p>֪������Щ��Ϣ֮��Ringo ��Ҫ���ÿ����Ϸ�еĽ�ȯ���䷽����ʹ�� $k$ ����Ϸ�л�õ����影������֮�����</p>
<h2>ʵ��ϸ��</h2>
<p>��������� <code>tickets.h</code> ͷ�ļ���</p>
<p>����Ҫʵ���������������</p>
<pre><code class="sh_cpp">long long find_maximum(int k, std::vector&lt;std::vector&lt;int&gt;&gt; x)</code></pre>
<ul><li><p>$k$����Ϸ��������</p>
</li>
<li><p>$x$��һ�� $n\times m$ �����飬��¼�˽�ȯ�ϵ����֡�ÿ����ɫ�Ľ�ȯ������������ַǵݼ�˳������</p>
</li>
<li><p>�������ֻ�ᱻ����һ�Ρ�</p>
</li>
<li><p>�������Ӧ��ֻ����һ�κ��� <code>allocate_tickets</code>���μ���������ݣ����������� $k$ ����Ϸ�еĽ�ȯ���䷽����ÿһ�ֶ�Ӧһ����ȯ���ϡ���ȯ�ķ��䷽��Ӧ��ʹ������������֮�ʹﵽ���</p>
</li>
<li><p>���������Ҫ�����ܹ���õ����Ľ�������֮�͡�</p>
</li>
</ul><p>���� <code>allocate_tickets</code> �������µķ�ʽ���ж��壺</p>
<pre><code class="sh_cpp">void allocate_tickets(std::vector&lt;std::vector&lt;int&gt;&gt; s)</code></pre>
<ul><li><p>$s$��һ�� $n\times m$ �����顣����� $i$ ����ɫ�ĵ� $j$ �Ž�ȯ��������䵽�˵� $r$ ����Ϸ����ô $s_{i,j}$ ��ֵӦ��Ϊ $r$�����δ��ʹ�ã�Ӧ��Ϊ $-1$��</p>
</li>
<li><p>���� $0\le i\le n-1$���� $s_{i,0}, s_{i,1}, \dots, s_{i,m-1}$ �У�ÿ��ֵ $0, 1, \dots, k - 1$ ����ֻ����һ�Σ�������Ԫ��Ӧ��Ϊ $-1$��</p>
</li>
<li><p>������ڶ��ֽ�ȯ���䷽���ܹ��ﵽ���ŵĽ�����ֵ�����Ը��������κ�һ�����ŷ�����</p>
</li>
</ul><h2>�����ʽ</h2>
<p>�������ʾ����������ĸ�ʽ�������ݣ�</p>
<ul><li>�� $1$ �У�$n\ m\ k$</li>
<li>�� $2 + i$ �У�$0\le i\le n-1$����$x_{i, 0}\ x_{i,1}\ \dots\ x_{i,m-1}$</li>
</ul><h2>�����ʽ</h2>
<p>�������ʾ����������ĸ�ʽ��ӡ��Ĵ𰸣�</p>
<ul><li>�� $1$ �У�<code>find_maximum</code> �ķ���ֵ</li>
<li>�� $2 + i$ �У�$0\le i\le n-1$����$s_{i, 0}\ s_{i,1}\ \dots\ s_{i,m-1}$</li>
</ul>

<pre><code class="language-input1">2 3 2
0 2 5
1 1 3
</code></pre>


<pre><code class="language-output1">7
0 -1 1
-1 1 0
</code></pre>


<p>��������ĺ������ã�</p>
<pre><code class="sh_cpp">find_maximum(2, [[0, 2, 5],[1, 1, 3]])</code></pre>
<p>����ζ�ţ�
- ��Ϸ������ $k=2$ �֣�
- �� $0$ ����ɫ��ȯ�ϵ��������ֱַ��� $0, 2$ �� $5$��
- �� $1$ ����ɫ��ȯ�ϵ��������ֱַ��� $1, 1$ �� $3$��</p>
<p>һ���ܹ�������Ž�����ֵ�ķ��䷽���ǣ�</p>
<ul><li><p>�ڵ� $0$ �֣�Ringo ѡ��� $0$ ����ɫ�ĵ� $0$ �Ž�ȯ��ӡ������ $0$���͵� $1$ ����ɫ�ĵ� $2$ �Ž�ȯ��ӡ������$3$�������ֻ�õ���С���������� $3$�����磬��Ϸ�����˿���ѡ�� $b=1$��$|1-0| + |1-3| = 1+2 = 3$��</p>
</li>
<li><p>�ڵ� $1$ �֣�Ringo ѡ��� $0$ ����ɫ�ĵ� $2$ �Ž�ȯ��ӡ������ $5$���͵� $1$ ����ɫ�ĵ� $1$ �Ž�ȯ��ӡ������ $1$���������ܹ���õ���С������ $4$�����磬��Ϸ�����˿���ѡ�� $b=3$��$|3-1|+|3-5|=2+2=4$��</p>
</li>
<li><p>��ˣ�������Ϸ���ֵĽ���֮��Ϊ $3+4=7$��</p>
</li>
</ul><p>Ϊ�˸���������䷽�������� <code>find_maximum</code> Ӧ�ð������·�ʽ���� <code>allocate_tickets</code>��</p>
<ul><li><code>allocate_tickets([[0, -1, 1], [-1, 1, 0]])</code></li>
</ul><p>���գ����� <code>find_maximum</code> Ӧ�÷������� $7$��</p>


<pre><code class="language-input2">4 2 1
5 9
1 4
3 6
2 7
</code></pre>


<pre><code class="language-output2">12
-1 0
0 -1
0 -1
-1 0
</code></pre>

<h4>eplanation</h4>
<p>��������ĺ������ã�</p>
<pre><code class="sh_cpp">find_maximum(1, [[5, 9], [1, 4], [3, 6], [2, 7]])</code></pre>
<p>����ζ�ţ�</p>
<ul><li>��Ϸֻ����һ�֣�</li>
<li>�� $0$ ����ɫ��ȯ�ϵ����ֱַ��� $5$ �� $9$��</li>
<li>�� $1$ ����ɫ��ȯ�ϵ����ֱַ��� $1$ �� $4$��</li>
<li>�� $2$ ����ɫ��ȯ�ϵ����ֱַ��� $3$ �� $6$��</li>
<li>�� $3$ ����ɫ��ȯ�ϵ����ֱַ��� $2$ �� $7$��</li>
</ul><p>һ���ܹ�������Ž����ķ��䷽���ǣ�</p>
<ul><li>�ڵ� $0$ �֣�Ringo ѡ��� $0$ ����ɫ�ĵ� $1$ �Ž�ȯ��ӡ������ $9$�� ���� $1$ ����ɫ�ĵ� $0$ �Ž�ȯ��ӡ������ $1$������ $2$ ����ɫ�ĵ� $0$ �Ž�ȯ��ӡ������ $3$������ $3$ ����ɫ�ĵ� $1$ �Ž�ȯ��ӡ������ $7$���������ܹ���õ���С������ $12$�����磬��Ϸ�����˿���ѡ�� $b=3$��</li>
</ul><p>$$
|3-9| + |3-1| + |3-3| + |3-7| = 6 + 2 + 0 + 4 = 12
$$</p>
<p>Ϊ�˸���������䷽�������� <code>find_maximum</code> Ӧ�ð������·�ʽ���� <code>allocate_tickets</code>��</p>
<ul><li><code>allocate_tickets([[-1, 0], [0, -1], [0, -1], [-1, 0]])</code></li>
</ul><p>���գ����� <code>find_maximum</code> Ӧ�÷������� $12$��</p>
<h2>������Լ��</h2>
<p>���� $100\%$ �����ݣ���֤��</p>
<ul><li>$2\le n\le 1500$ �� $n$ Ϊż��</li>
<li>$1\le k\le m\le 1500$</li>
<li>$0\le x_{i,j}\le 10^9$���������е� $0\le i\le n-1$ �� $0\le j\le m-1$��</li>
<li>$x_{i,j-1}\le x_{i,j}$���������е� $0\le i\le n-1$ �� $1\le j\le m-1$��</li>
</ul><div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th style="text-align:center;">������</th>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">��ֵ</th>
</tr></thead><tbody><tr><td style="text-align:center;">$1$</td>
<td style="text-align:center;">$m=1$</td>
<td style="text-align:center;">$11$</td>
</tr><tr><td style="text-align:center;">$2$</td>
<td style="text-align:center;">$k=1$</td>
<td style="text-align:center;">$16$</td>
</tr><tr><td style="text-align:center;">$3$</td>
<td style="text-align:center;">$0\le x_{i,j}\le 1$���������е� $0\le i\le n-1$ �� $0\le j\le m-1$��</td>
<td style="text-align:center;">$14$</td>
</tr><tr><td style="text-align:center;">$4$</td>
<td style="text-align:center;">$k=m$</td>
<td style="text-align:center;">$14 $</td>
</tr><tr><td style="text-align:center;">$5$</td>
<td style="text-align:center;">$n,m\le 80$</td>
<td style="text-align:center;">$12$</td>
</tr><tr><td style="text-align:center;">$6$</td>
<td style="text-align:center;">$n,m\le 300$</td>
<td style="text-align:center;">$23$</td>
</tr><tr><td style="text-align:center;">$7$</td>
<td style="text-align:center;">û����������</td>
<td style="text-align:center;">$10$</td>
</tr></tbody></table></div>
<p><strong>ʱ������</strong>��$2 \texttt{s}$</p>
<p><strong>�ռ�����</strong>��$1024 \texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20970/file/attachment.zip">����������������</a></p>
