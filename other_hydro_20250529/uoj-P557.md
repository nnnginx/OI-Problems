<p><strong> ����ĳЩԭ�����֧�� C++ ���汾���Ե��ύ�� </strong></p>
<p>�żӴ��������⹫԰���� $N$ �����㣬���Ǵ� $0$ �� $N - 1$ ��š���Щ������ $N - 1$ ��˫���·���ӣ�������������侭����Щ��·������Ψһһ����·������·�� $0$ �� $N - 2$ ��š��� $i$ ����·���ӵ� $A_i$ ��������� $B_i$ �����㣬����������·��Ҫ����һ��Сʱ��Ϊ�˱���ӵ����ÿ�����㽫������������·������</p>
<p>����Ѱ��һ������·�߲�ʹ��ÿ�����㶼���ι�һ�Ρ�����Ϊ��һ�������ߵ���һ������ʱ����̫���·��ʮ�����ĵġ�Ϊ��Ѱ��һ����Ȥ��·�ߣ�����㰲�ž���Ĳι�˳��ʹ�òι���һ�����������ѵ�ʱ�䲻�����ι�֮ǰ���������ѵ�ʱ�䡣���仰˵�������ҵ�һ������ $P_0, P_1, \ldots, P_{N-1}$ ʹ����� $0$ �� $N - 1$ �е���������ǡ��һ�Σ����Ҵӵ� $P_i$ �����㵽��� $P_{i+1}$ �����������ʱ�䲻�����ӵ� $P_{i-1}$ �����㵽��� $P_i$ �����������ʱ�䣬���� $0 \lt i \lt N - 1$��</p>
<p>������û�о����������ͼ��������������Ϣ���Ľ������ɴ�ѯ�ʲ����ҵ�һ����Ȥ·�ߡ�������ܽ��� $Q$ ��ѯ�ʣ�ÿ��ѯ����Ҫ�ṩ�������� $X$ �� $Y$������ $0 \le X, Y \lt N$��ÿ��ѯ������������һ�֣�</p>
<p>�ӵ� $X$ �����㵽�� $Y$ ��������Ҫ���Ѷ��ٸ�Сʱ���ر�أ��� $X = Y$ ��ش��� $0$��</p>
<p>�ж��ٸ����� $Z$ ���㣬������ӵ� $X$ �����㵽��� $Z$ ������ʱһ���ᾭ���� $Y$ �����㡣�� $Y$ �����㽫�ᱻ�������ڣ��ر�أ��� $X = Y$ ��ش��� $N$��</p>
<h2>ʵ��ϸ��</h2>
<p>��������� <code>fun.h</code> ͷ�ļ���</p>
<p>�����ʵ�� <code>createFunTour</code> ����:</p>
<pre><code class="sh_cpp">std::vector&lt;int&gt; createFunTour(int N, int Q)</code></pre>
<p>�ú������������ǡ�õ���һ�Ρ�</p>
<ul>
<li><p>$N$: һ��������ʾ�����������</p>
</li>
<li><p>$Q$: һ��������ʾѯ�ʴ��������ֵ��</p>
</li>
</ul>
<p>�ú������Ե���������������������</p>
<pre><code class="sh_cpp">int hoursRequired(int X, int Y)</code></pre>
<ul>
<li>$X$: һ��������ʾ��һ������ı�š�</li>
<li>$Y$: һ��������ʾ�ڶ�������ı�š�</li>
<li>�ú���������һ��������ʾ�ӵ� $X$ �����㵽�� $Y$ ��������Ҫ���ѵ�Сʱ����</li>
<li>��� $X$ �� $Y$ ��ֵ���� $0$ �� $N - 1$ �ķ�Χ�ڣ��ò��Ե㽫��Ϊ�𰸴���</li>
</ul>
<pre><code class="sh_cpp">int attractionsBehind(int X, int Y)</code></pre>
<ul>
<li>$X$: һ��������ʾ��һ������ı�š�</li>
<li>$Y$: һ��������ʾ�ڶ�������ı�š�</li>
<li>�ú���������һ��������ʾ�ж��ٸ����� $Z$ ���㣬������ӵ� $X$ �����㵽��� $Z$ ������ʱһ���ᾭ���� $Y$ �����㡣</li>
<li>��� $X$ �� $Y$ ��ֵ���� $0$ �� $N - 1$ �ķ�Χ�ڣ��ò��Ե㽫��Ϊ�𰸴���</li>
<li>�ú������뷵��һ����Ϊ $N$ ���������У���ʾ���ҵ��ľ���ι�˳��</li>
</ul>
<h2>���������</h2>
<p>��������⽫�������¸�ʽ�����ݣ�</p>
<pre>N Q
A[0] B[0]
A[1] B[1]
.
.
.
A[N-2] B[N-2]</pre><p>��� <code>createFunTour</code> ��ȷ������һ��������������У����� <code>hoursRequired</code> �� <code>attractionsBehind</code> �ĵ��ô����ܺͲ����� $Q$����ô��������⽫����� <code>createFunTour</code> �õ������С������������������⽫�����������Ϣ��</p>


<pre><code class="language-input1">7 400000
0 1
0 5
0 6
1 2
1 4
2 3
</code></pre>


<pre><code class="language-output1">3 6 4 5 2 0 1
</code></pre>


<p>����ͼ�������� $N = 7$��$Q = 4\times 10^5$��$A = [0, 0, 0, 1, 1, 2]$��$B = [1, 5, 6, 2, 4, 3]$��</p>
<p><img src="//img.uoj.ac/problem/557/557_ex1.png" alt="����һ" class="img-responsive center-block" style="width:300px;"></p>
<p>����⽫���� <code>createFunTour(7, 400000)</code>��</p>
<p>�����ѯ�� <code>hoursRequired(3, 5)</code>������������ $4$��
�����ѯ�� <code>hoursRequired(5, 4)</code>������������ $3$��
�����ѯ�� <code>attractionsBehind(5, 1)</code>������������ $4$���ӵ�������㵽��һ�����������ĸ����㽫һ���ᾭ����һ�����㡣
�����ѯ�� <code>attractionsBehind(1, 5)</code>������������ $1$��
һ������Ҫ��ķ�������Ϊ $[3, 6, 4, 5, 2, 0, 1]$��������һ���ι۾��������ʱ�䰴˳��ֱ�Ϊ $[4, 3, 3, 3, 2, 1]$��</p>
<h2>������Լ��</h2>
<p>���� $100\%$ �����ݣ���֤��</p>
<ul>
<li>$2 \le N \le 10^5$</li>
<li>$Q = 4\times 10^5$</li>
<li>����������������ͨ��˫���·���ൽ�</li>
<li>ÿ����������������������·��</li>
</ul>
<h4>������ $1$��$10$ �֣�</h4>
<ul>
<li>$N \le 17$</li>
</ul>
<h4>������ $2$��$16$ �֣�</h4>
<ul>
<li>$N \le 500$</li>
</ul>
<h4>������ $3$��$21$ �֣�</h4>
<ul>
<li>�����е� $1 \le i \lt N$����һ�������ŵ� $i$ ��������� $\left\lfloor\frac{i - 1}{2} \right\rfloor$ �������˫���·��</li>
</ul>
<h4>������ $4$��$19$ �֣�</h4>
<ul>
<li><p>��������һ������ $T$ ʹ�ö������� $0 \le i \lt N$��<code>hoursRequired(T, i)</code> $\lt 30$ ���Ҵ���һ���������� $[L_i, R_i](0 \le L_i \le i \le R_i \lt N)$ ��������������</p>
<ul>
<li>�ӵ� $T$ �����㵽��� $j$ ��������뾭���� $i$ �����㵱�ҽ��� $L_i \le j \le R_i$��</li>
<li>�� $L_i \lt i$����ǡ��һ������ $X$ ���㣺<ul>
<li>$L[i] \le X \lt i$</li>
<li>��һ�����ӵ� $i$ ��������� $X$ ������ĵ�·��</li>
</ul>
</li>
<li>�� $i \lt R_i$����ǡ��һ������ $Y$ ���㣺<ul>
<li>$i \lt Y \le R_i$</li>
<li>��һ�����ӵ� $i$ ��������� $Y$ ������ĵ�·��</li>
</ul>
</li>
</ul>
</li>
</ul>
<h4>������ $5$��$34$ �֣�</h4>
<ul>
<li>�޸������ơ�</li>
</ul>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">������</th>
<th style="text-align:center;">���������ݰ�</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">1</td>
<td style="text-align:center;">1, 2, 3, 4</td>
</tr>
<tr>
<td style="text-align:center;">2</td>
<td style="text-align:center;">1, 2, 3, 4, 5, 6, 7</td>
</tr>
<tr>
<td style="text-align:center;">3</td>
<td style="text-align:center;">1, 2, 5, 8</td>
</tr>
<tr>
<td style="text-align:center;">4</td>
<td style="text-align:center;">1, 3, 6, 9</td>
</tr>
<tr>
<td style="text-align:center;">5</td>
<td style="text-align:center;">1, 2, 3, 4, 5, 6, 7, 8, 9, 10</td>
</tr>
</tbody>
</table>
</div>
<p><strong> ʵ�ʲ����У�ǰ 10 �� subtask Ϊ���ݰ����� 5 �� subtask Ϊ 5 �������� </strong></p>
<p><strong>ʱ������</strong>��$2 \texttt{s}$</p>
<p><strong>�ռ�����</strong>��$512 \texttt{MB}$</p>
<h2>������</h2>
<p><a href="./20961/file/attachment.zip">����������������</a></p>
