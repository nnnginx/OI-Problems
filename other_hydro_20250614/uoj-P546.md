<p>�ڰ���д�� $n$ ����������Ҷ�С�� $p$ �������� $a_1, a_2, \cdots, a_n$��С J ������Щ���ֺ�С M ��һ��������Ϸ��</p>
<p>��Ϸ����ʮ�ּ򵥣���Ϸ��ʼʱ��С J �����Щ���������ѡ�����ɸ���С M ���£���С M �����ͨ�����ɴ�ѯ����ȷ��С J ѡ������Щ���֡�</p>
<p>ÿһ��ѯ�ʵ�ģʽ���£�С M ��������ָ��һ������ $a_k$��������С J ��ѡ�������֮һ����С J �����С M ����ѡ��������������ܱ�ʾ�� $(a_k)^m \bmod p$ ���������� $m$ ��������������$\bmod$ ��ʾ�������������������������֮���� $a_k$ û�б�С J ѡ�У���С J ֻ�����С M $a_k$ û�б�ѡ�С�</p>
<p>��Ϸ����С M ȷ��С J ��ѡ�е��������ֺ����̽�����</p>
<p>���磬�� $n=4,p=7$������ $\{a_n\}$ ���±�˳������Ϊ $\{1, 3, 4, 6\}$��С J ѡ��������Ϊ $\{1, 4, 6\}$��һ�ֿ��ܵ���Ϸ���еĹ��̣����������Ź��̣����£�</p>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle">
        <thead><tr><th>С M ��ѯ��</th><th>С J �ķ���</th></tr></thead>
        <tbody>
            <tr><td>$a_2=3$</td><td>$a_2$δѡ��</td></tr>
            <tr><td>$a_4=6$</td><td>$a_1=1,a_4=6$</td></tr>
            <tr><td>$a_3=4$</td><td>$a_1=1,a_3=4$</td></tr>
        </tbody>
    </table>
</div>

<p>3 ��ѯ�ʺ�С J ��ѡ�������������ѱ�С M ȷ������Ϸ������</p>
<p>С M ������ҵû��д�꣬�������Ҫ����Ϸ���е�ʱ���������������֪��Ϊ��ʹ��Ϸ������������Ҫ����ѯ�ʵ���С���������� $S$ �Ƕ��١�</p>
<p>Ϊ�˱��⾫��������Ҫ����𰸳� $(2^n - 1)$ ��ģ $998244353$ ���������ڱ����У��������ΪС J ÿ����ѡ��ʱ���ڼ��� $\{a_1, a_2, \cdots, a_n\}$ ��ȫ���ǿ��Ӽ��еȸ��ʵ�ѡ��һ���������ǰ���¿���֤�� $(2^n - 1) \times S$ һ����һ��������</p>
<h2>�����ʽ</h2>
<p>��һ������������ $n$ �� $p$��</p>
<p>�ڶ��� $n$ �������������α�ʾ $a_1, a_2, \cdots, a_n$��</p>
<h2>�����ʽ</h2>
<p>��һ��һ��������ʾ�𰸡�</p>


<pre><code class="language-inputundefined"><code class="sh_plain">4 7
1 3 4 6</code>
</code></pre>

<pre><code class="language-outputundefined"><code class="sh_plain">17</code>
</code></pre>

<p>�±������С J ��ѡ���Ӽ���С M ��Сѯ�ʴ����Ĺ�ϵ��</p>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle">
        <thead><tr><th>С J ��ѡ���Ӽ�</th><th>���ŵ�ѯ�ʼ���</th></tr></thead>
        <tbody>
            <tr><td>$\{1\}$</td><td>$\{1\}$</td></tr>
            <tr><td>$\{3\},\{3,4\},\{3,6\},\{3,4,6\},\{3,1\},\{3,1,4\},\{3,1,6\},\{3,1,4,6\}$</td><td>$\{3\}$</td></tr>
            <tr><td>$\{4\},\{1,4\}$</td><td>$\{4\}$</td></tr>
            <tr><td>$\{6\},\{1,6\}$</td><td>$\{6\}$</td></tr>
            <tr><td>$\{4,6\},\{1,4,6\}$</td><td>$\{4,6\}$</td></tr>
    </tbody></table>
</div>

<p>�����Сѯ�ʴ��������� $S = \frac{17}{15}$��</p>


<pre><code class="language-inputundefined"><code class="sh_plain">8 9
1 2 3 4 5 6 7 8</code>
</code></pre>

<pre><code class="language-outputundefined"><code class="sh_plain">532</code>
</code></pre>
<h2>����3</h2>
<p>�������ļ���</p>
<h2>���ݷ�Χ</h2>
<p>�������в��Ե㣺$1 \leq n \leq 5000$��$3 \leq p \leq 10^8$ ��$1 \leq a_i &lt; p\ (1 \leq i \leq n)$�� $a_i$ ������ͬ��</p>
<p>�������б��Ϊ�����Ĳ��Ե㣬��֤ $p$ ��һ���������������б��Ϊż���Ĳ��Ե㣬��֤���������� $q$ �������� $k &gt; 1$ ʹ�� $p = q^k$</p>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle">
        <thead><tr><th>���Ե���</th><th>$n \le$</th><th>$p \le$</th><th>��������</th><th>���Ե���</th><th>$n \le$</th><th>$p \le$</th><th>��������</th></tr></thead>
        <tbody>
            <tr><td>$1$</td><td rowspan="2">$10$</td><td rowspan="2">$100$</td><td rowspan="4">$��$</td><td>$2$</td><td rowspan="2">$10$</td><td rowspan="2">$100$</td><td rowspan="4">$��$</td></tr>
            <tr><td>$3$</td><td>$4$</td></tr>
            <tr><td>$5$</td><td>$200$</td><td>$5000$</td><td>$6$</td><td>$200$</td><td>$5000$</td></tr>
            <tr><td>$7$</td><td rowspan="2">$300$</td><td rowspan="2">$10^6$</td><td>$8$</td><td rowspan="2">$300$</td><td rowspan="2">$10^6$</td></tr>
          <tr><td>$9$</td><td rowspan="2">$A$</td><td>$10$</td><td>$B$</td></tr>
            <tr><td>$11$</td><td rowspan="5">$5000$</td><td rowspan="2">$10^7$</td><td>$12$</td><td rowspan="5">$5000$</td><td rowspan="2">$10^7$</td><td rowspan="2">$��$</td></tr>
            <tr><td>$13$</td><td>$��$</td><td>$14$</td></tr>
            <tr><td>$15$</td><td rowspan="3">$10^8$</td><td>$A$</td><td>$16$</td><td rowspan="3">$10^8$</td><td>$B$</td></tr>
            <tr><td>$17$</td><td rowspan="2">$��$</td><td>$18$</td><td rowspan="2">$��$</td></tr>
            <tr><td>$19$</td><td>$20$</td></tr>
        </tbody>
    </table>
</div>

<p>�������� $A$����ģ $p$ ������ $3^i\ (1 \leq i \leq p - 1)$������ͬ�ࡣ</p>
<p>�������� $B$�������е� $1 \leq i \leq n$ ���� $(a_i, p) &gt; 1$��</p>
<p><strong>ʱ������:</strong> $2\texttt{s}$</p>
<p><strong>�ռ�����:</strong> $128\texttt{MB}$</p>
<p><a href="http://uoj.ac/download.php?type=problem&amp;id=546">�����ļ�</a></p>
