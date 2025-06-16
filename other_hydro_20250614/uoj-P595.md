<p>̫����Ϊ����췲�����飬���� <span class="uoj-username" data-rating="1797">EntropyIncreaser</span> �·���<span class="uoj-username" data-rating="1797">EntropyIncreaser</span>��Ҳ���� EI��������д�����գ���˼��̫����</p>
<p>���죬<span class="uoj-username" data-rating="1797">EntropyIncreaser</span> �ټ��˷�˿Ⱥ��� $n$ ��ȺԱ����������ʢ�硣����ϣ�����ȺԱ��������������Ϸ����չʾ�Լ��������ǻۡ�</p>
<p>��Ϸ��һ���� <span class="uoj-username" data-rating="1797">EntropyIncreaser</span>����һ���� $n$ ��ȺԱ�������ų���һ�У����α��Ϊ $1, 2, \ldots, n$���ַ�����ǰ $k$ ��Ӣ����ĸ���� $\Sigma$��Ҳ����˵����Ϸ�������ַ������� $\Sigma$ ��Ԫ�ع��ɡ�</p>
<p>��Ϸһ��ʼ��<span class="uoj-username" data-rating="1797">EntropyIncreaser</span> ��ÿ��ȺԱ������һ���ַ������� $i$ ��ȺԱ���ַ����� $S_i$�����ÿ��ȺԱ������ش��յ����ַ��� $S_i$ ����ѡһ���Ӵ� $T_i$���Ӵ�����������������Ϊ�մ�����ȺԱ�ǰѸ�������ѡ���Ӵ� $T_i$ ������ֻ������ǰ���˳��û�м���ؽӳ���һ���������ַ��� $T=T_1T_2\cdots T_n$��<span class="uoj-username" data-rating="1797">EntropyIncreaser</span> ֻ��֪�� $T$������֪��ÿ���ַ�����λȺԱ����ġ���Ϸ�Ĺ����ǣ�ֻҪ���һ����ܵ� $T_1, T_2, \ldots, T_n$�����ܻ��ʤ����</p>
<p><span class="uoj-username" data-rating="1797">EntropyIncreaser</span> �����ַ��� $T$������˼�����������ֳ� $n$ ���ַ��� $T'_1T'_2\cdots T'_n$��ͬ������Ϊ�գ���ȺԱ�Ǿ���ط��֣�$T'_i$ ȷʵ���������յ��Ĵ� $S_i$ ���Ӵ���</p>
<p><span class="uoj-username" data-rating="1797">EntropyIncreaser</span> ЦЦ��������һ����ˮ�⣬ûʲô�ѵġ��������Ӵ�һ����Ѷȡ���</p>
<p>��ʱ����Ů�������������Ϸ�ļ�ǿ�档</p>
<p>���ڵ� $i$ λȺԱ��Ȼȡ�����Ӵ� $T_i$����ÿλȺԱ����ǰ�����̵ļ�λ���ᱻ���ܴ��ң���ȺԱ��Ȼ�ճ����룬Ҳ����ÿλȺԱ���ڷ�����һ�� $\Sigma$ �ϵ��û� $f_i$��$T_i$ �ĵ� $j$ ���ַ� $T_{ij}$ ����ʱ����� $f_i(T_{ij})$������������ַ��������������� $T$��<span class="uoj-username" data-rating="1797">EntropyIncreaser</span> ��Ŀ����Ȼ�ǽ��һ����ܵ� $T_1, T_2, \ldots, T_n$��</p>
<p><span class="uoj-username" data-rating="1797">EntropyIncreaser</span> ��ϸ���꣬�ٴν� $T$ �ֳ��� $n$ ���ַ��� $T'_1, T'_2, \ldots, T'_n$��ȺԱ�Ƿ����ˣ�ȷʵ�����û� $f_i$��ʹ�� $S_i$ ��һ���Ӵ����� $f_i$ �����õõ� $T'_i$��</p>
<p>�����峿���е�ҹ��������β����<span class="uoj-username" data-rating="1797">EntropyIncreaser</span> ���������񽫴���Ⱥ����ѧ���ǻۣ�����Ҫ�Ⱦ����������顣��</p>
<p>���ڣ����Լ���֮����ǿ�ĵ�һ���������������ǰ������������һ���������һ����Ϸ�У��ж��ٸ��ַ��� $T$ ������һ��⣿�𰸿��ܴܺ����Զ� $998244353$ ȡģ��</p>
<h2>�����ʽ</h2>
<p>��һ������������ $n, k$��</p>
<p>������ $n$ �У�ÿ��һ���ַ��������α�ʾ $S_1, S_2, \ldots, S_n$��</p>
<h2>�����ʽ</h2>
<p>����н���ַ������������� $998244353$ ȡģ��</p>


<pre><code class="language-input1">2 2
aa
a
</code></pre>


<pre><code class="language-output1">11
</code></pre>


<p>�� $\epsilon$ ָ���մ���</p>
<p>$S_1$ ���Ӵ��� $\epsilon$, <code>a</code>, <code>aa</code>�����Ҽ�λ��ɻ�� $\epsilon$, <code>a</code>, <code>b</code>, <code>aa</code>, <code>bb</code>��</p>
<p>$S_2$ ���Ӵ��� $\epsilon$, <code>a</code>�����Ҽ�λ��ɻ�� $\epsilon$, <code>a</code>, <code>b</code>��</p>
<p>�����������н�Ĵ��У�$\epsilon$, <code>a</code>, <code>b</code>, <code>aa</code>, <code>ab</code>, <code>ba</code>, <code>bb</code>, <code>aaa</code>, <code>aab</code>, <code>bba</code>, <code>bbb</code>��</p>


<pre><code class="language-input2">2 2
aa
ab
</code></pre>


<pre><code class="language-output2">17
</code></pre>

<h2>������Լ��</h2>
<p>��� $L=\sum_{i=1}^n|S_i|$��</p>
<p>��֤ $2 \le k \le 26$��$S_i$ �ǿգ�$L \le 10^6$��</p>
<p>������һ��2�֣���$n=1$��$k=2$��$L \le 1000$��</p>
<p>���������7�֣���$n=1$��$L \le 1000$��</p>
<p>����������11�֣���$n=1$��$L \le 10^5$��</p>
<p>�������ģ�13�֣���$k=2$��$L \le 1000$��</p>
<p>�������壨17�֣���$L \le 1000$��</p>
<p>����������31�֣���$k \le 5$��</p>
<p>�������ߣ�19�֣������������ơ�</p>
<p><strong>ʱ������</strong>��$3\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$2048\texttt{MB}$</p>
<h2>����</h2>
<p><a href="https://uoj.ac/download.php?type=problem&amp;id=595">������������</a></p>
