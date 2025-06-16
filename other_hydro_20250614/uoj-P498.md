<p>�������ڱ���ķ׷����</p>
<p>Ϊ�˰���׷����������Ҫ֪���е�ͼ�ж��ٸ����󶴿������أ�</p>
<p>����ֻЬ̫̫�ļ�ʵ��̫���ˣ�Ϊ�˼򵥵�˵������������������ͼ $G_{1} =( V_{1} ,E_{1}) ,G_{2} =( V_{2} ,E_{2})$ �ĳ˻�Ϊһ���µ�ͼ $G_{1} \times G_{2} =\left( V^{*} ,E^{*} \right)$��</p>
<p>�����µĵ㼯 $V^{*}$ Ϊ:</p>
<p>$$
V^{*} = \left\{{(a,b)| a \in V_{1}, b \in V_{2}}\right\}
$$</p>
<p>�����µı߼� $E^{*}$ Ϊ��</p>
<p>$$
E^{*} =\left\{\left(( u_{1} ,v_{1}) ,( u_{2} ,v_{2})\right) \mid ( u_{1} ,u_{2}) \in E_{1}, ( v_{1} ,v_{2}) \in E_{2}\right\}
$$</p>
<p>���������� $n$���Լ�������ͼ $G_{1} ,G_{2} ,\dotsc ,G_{n}$����ֻЬ̫̫�ļҿ��Ա�ʾ��</p>
<p>$$
H = (((G_1 \times G_2) \times G_3) \times \cdots) \times G_n
$$</p>
<p>Ϊ�˷���������ϷŪ��ķ��������ͬһ����ͨ�飬�������ȴ�ͨ�����е����󶴣���ֻ��Ҫ����һ�顣</p>
<p>Ϊ�˷���������ϷŪ��ķ��������ͬһ���κ�һ����ͨ�飬�������󶴡�</p>
<p>Ҳ����˵������Ҫ����� $H$ ����ͨ�����������ǽ���������ÿ�� $G_k$ �ľ���ϸ�ڣ������������ڼ���ÿ�� $G_k$ ����������䶼�� $\frac12$ �ĸ������ߣ��� $H$ ����ͨ�����������Ȼ $G_k$ ��ȫ��ȡ������ ${\large {2^{\binom{m_1}2 + \binom{m_2}2 + \cdots + \binom{m_n}2}}}$ �֡�</p>
<p>�����������ֻ��Ҫ����𰸳��� ${\large {2^{\binom{m_1}2 + \binom{m_2}2 + \cdots + \binom{m_n}2}}}$���� $998244353$ ȡģ���ɡ�</p>
<h2>�����ʽ</h2>
<p>��һ������һ�������� $n$��</p>
<p>������һ������ $n$ ��������,�� $k$ ��������Ϊ $m_k$����ʾ�� $k$ ��ͼ�Ķ���������</p>
<h2>�����ʽ</h2>
<p>���һ����������ʾ�� $\bmod 998244353$��</p>


<pre><code class="language-input1">1
3
</code></pre>


<pre><code class="language-output1">13
</code></pre>


<p>ע����� $n=1$ �����������ö�����нڵ����Ϊ$m_1$�Ĵ��������ͼ����ͨ������֮�͡�</p>


<pre><code class="language-input2">2
2 3
</code></pre>


<pre><code class="language-output2">73
</code></pre>


<p>$G_1$ ���� $0$ ���ߵ�����£��κ�һ�� $G_2$ ���ᵼ�� $H$ ���� $6$ ����ͨ�飬�����ķ������� $8$ �֡�</p>
<p>$G_1$ ���� $1$ ���ߣ�$G_2$ ���� $0$ ���ߵ�����£�$H$ ���� $6$ ����ͨ�飬�����ķ����� $1$ �֡�</p>
<p>$G_1$ ���� $1$ ���ߣ�$G_2$ ���� $1$ ���ߵ�����£�$H$ ���� $4$ ����ͨ�飬�����ķ����� $3$ �֡�</p>
<p>$G_1$ ���� $1$ ���ߣ�$G_2$ ���� $2$ ���ߵ�����£�$H$ ���� $2$ ����ͨ�飬�����ķ����� $3$ �֡�</p>
<p>$G_1$ ���� $1$ ���ߣ�$G_2$ ���� $3$ ���ߵ�����£�$H$ ���� $1$ ����ͨ�飬�����ķ����� $1$ �֡�
$$
6\times 8 + 6\times 1 + 4\times 3 + 2\times 3 + 1\times 1 = 73
$$</p>


<pre><code class="language-input3">2
4 4
</code></pre>


<pre><code class="language-output3">21565
</code></pre>

<h2>������Լ��</h2>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th><th>$n$</th><th>$m_k$</th></tr></thead><tbody><tr><td>$1$</td><td rowspan="1">$\le 4$</td><td rowspan="1">$\le 4$</td></tr><tr><td>$2$</td><td rowspan="1">$ = 1$</td><td rowspan="1">$\le 10^3$</td></tr><tr><td>$3$</td><td rowspan="1">$ = 1$</td><td rowspan="1">$\le 10^5$</td></tr><tr><td>$4$</td><td rowspan="1">$ = 2$</td><td rowspan="1">$\le 10^3$</td></tr><tr><td>$5$</td><td rowspan="1">$ = 2$</td><td rowspan="1">$\le 10^5$</td></tr><tr><td>$6$</td><td rowspan="1">$\le 10^3$</td><td rowspan="1">$\le 10^3$</td></tr><tr><td>$7$</td><td rowspan="1">$\le 10^5$</td><td rowspan="1">$\le 10^3$</td></tr><tr><td>$8$</td><td rowspan="1">$\le 10^5$</td><td rowspan="1">$\le 10^5$</td></tr><tr><td>$9$</td><td rowspan="1">$\le 10^5$</td><td rowspan="1">$\le 10^5$</td></tr><tr><td>$10$</td><td rowspan="1">$\le 10^5$</td><td rowspan="1">$\le 10^5$</td></tr></tbody></table></div>

<p>�������в������ݣ����� $1\le n, m_k\le 10^5$��</p>
<p><strong>ʱ������</strong>��$\texttt{1s}$</p>
<p><strong>�ռ�����</strong>��$\texttt{512MB}$</p>
<h2>����</h2>
<p><a href="./20903/file/attachment.zip">������������</a></p>
