<p>2048�꣬����ʮ�� CSP ��֤�Ŀ����ϣ���Ϊѡ�ֵ�С�����˵�һ�⡣������������$n$�����ݣ����ݴ�$1 \sim n$��ţ�$i$�����ݵĹ�ģΪ$a_i$��</p>
<p>С���Ը�����Ƴ���һ���������򣬶���һ���ģΪ$u$�����ݣ��ó����<strong>����ʱ��</strong>Ϊ$u^2$��Ȼ���������������һ���ģΪ$u$������֮���������κ�һ���ģ<strong>С��</strong>$u$�����������д��������е�$a_i$��һ����������С�������ڲ��޸ĳ�����������ȷ��������������С������ʹ��һ�ַǳ�ԭʼ�Ľ�����������������ݻ��ֳ����ɸ����ݶΣ����ڱ�����������Ž�ͬһ���ڵ����ݺϲ��������ݣ����ģ���ڶ���ԭ���ݵ�<strong>��ģ֮��</strong>��С�����������ݵĹ�ģ�ܹ�������</p>
<p>Ҳ����˵��С����Ҫ�ҵ�һЩ�ֽ��$1 \leq k_1 &lt; k_2 &lt; \cdots &lt; k_p &lt; n$��ʹ��</p>
<p>$$\sum\limits_{i=1}^{k_1}a_i \leq \sum\limits_{i=k_1+1}^{k_2}a_i \leq  \cdots \leq \sum\limits_{i=k_p+1}^{n}a_i$$</p>
<p>ע��$p$����Ϊ$0$�Ҵ�ʱ$k_0=0$��Ҳ����С�����Խ��������ݺϲ���һ�����С�</p>
<p>С��ϣ�����ĳ����������ȷ������������£� ����ʱ��Ҳ�ܾ���С��Ҳ����<strong>��С��</strong></p>
<p>$$(\sum\limits_{i=1}^{k_1}a_i)^2+(\sum\limits_{i=k_1+1}^{k_2}a_i)^2+\cdots+(\sum\limits_{i=k_p+1}^{n}a_i)^2$$</p>
<p>С�������������ǳ���Ȥ����������̣�����$n$��$a_i$������������Ż��ַ����£�С���ĳ��������ʱ�䡣</p>
<h2>�����ʽ</h2>
<p><strong>���ڱ�������ݷ�Χ�ϴ󣬲��ֲ��Ե��</strong>$a_i$<strong>���ڳ��������ɡ�</strong></p>
<p>��һ����������$n,type$��$n$���������Ŀ������$type$��ʾ���뷽ʽ��</p>
<ol><li>��$type=0$����ò��Ե��$a_i$<strong>ֱ�Ӹ���</strong>�������ļ����������ڶ���$n$���Կո�ָ�������$a_i$����ʾÿ�����ݵĹ�ģ��</li>
<li>��$type=1$����ò��Ե��$a_i$��<strong>��������</strong>�����ɷ�ʽ�����ġ������ļ����������ڶ��������Կո�ָ�������$x,y,z,b_1,b_2,m$��������$m$���У��� $i(1 \leq i \leq m)$ �а��������Կո�ָ���������$p_i,l_i,r_i$��</li>
</ol><p>����$type=1$��$23\sim 25$�Ų��Ե㣬$a_i$�����ɷ�ʽ���£�</p>
<p>��������$x,y,z,b_1,b_2,m$���Լ�$m$����Ԫ�� $(p_i,l_i,r_i)$��</p>
<p>��֤$n \geq 2$����$n &gt; 2$���� $\forall 3\leq i \leq n,b_i=(x\times b_{i-1} + y \times b_{i-2} + z) \bmod 2^{30}$��</p>
<p>��֤$1 \leq p_i \leq n, p_m=n$����$p_0=0$����$p_i$������ $\forall 0 \leq i &lt; m$��$p_i &lt; p_{i+1}$��</p>
<p>��������$1 \leq j \leq m$�����±�ֵ $i (1 \leq i \leq n)$ ���� $p_{j-1} &lt; i \leq p_j$������</p>
<p>$$a_i=(b_i \bmod (r_j-l_j+1)) + l_j$$</p>
<p><strong>�����������ɷ�ʽ����Ϊ�˼�����������С����׼�㷨�������ڸ����ɷ�ʽ��</strong></p>
<h2>�����ʽ</h2>
<p>���һ��һ����������ʾ�𰸡�</p>


<pre><code class="language-inputundefined"><code class="sh_plain">5 0
5 1 7 9 9</code>
</code></pre>

<pre><code class="language-outputundefined"><code>247</code>
</code></pre>

<p>���ŵĻ��ַ���Ϊ $\{5, 1\},\{7\},\{9\},\{9\}$����$5+1 \leq 7 \leq 9 \leq 9$֪�÷����Ϸ���</p>
<p>��Ϊ $(5+1)^2+7^2+9^2+9^2=247$��</p>
<p>��Ȼ���ַ���  $\{5\},\{1\},\{7\},\{9\},\{9\}$ ��Ӧ������ʱ��� $247$С����������һ��Ϸ���������Ϊ$5&gt;1$��</p>
<p>��Ȼ���ַ��� $\{5\},\{1,7\},\{9\},\{9\}$ �Ϸ������÷�����Ӧ������ʱ��Ϊ$251$���� $247$��</p>


<pre><code class="language-inputundefined"><code class="sh_plain">10 0
5 6 7 7 4 6 2 13 19 9</code>
</code></pre>

<pre><code class="language-outputundefined"><code class="sh_plain">1256</code>
</code></pre>

<p>���ŵĻ��ַ���Ϊ $\{5\},\{6\},\{7\},\{7\},\{4,6,2\},\{13\},\{19,9\}$��</p>


<pre><code class="language-inputundefined"><code class="sh_plain">10000000 1
123 456 789 12345 6789 3
2000000 123456789 987654321
7000000 234567891 876543219
10000000 456789123 567891234</code>
</code></pre>

<pre><code class="language-outputundefined"><code class="sh_plain">4972194419293431240859891640</code>
</code></pre>
<h2>������Լ��</h2>
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th>
    <th>$n \leq$</th>
    <th>$a_i \leq$<br></th>
    <th>$type =$</th>
    </tr></thead><tbody><tr><td>$1 \sim 3$<br></td>
    <td>$10$<br></td>
    <td>$10$<br></td>
    <td rowspan="5">$0$<br></td>
  </tr><tr><td>$4 \sim 6$</td>
    <td>$50$<br></td>
    <td>$10^3$<br></td>
  </tr><tr><td>$7 \sim 9$</td>
    <td>$400$</td>
    <td>$10^4$</td>
  </tr><tr><td>$10 \sim 16$<br></td>
    <td>$5000$</td>
    <td>$10^5$</td>
  </tr><tr><td>$17 \sim 22$</td>
    <td>$5 \times 10^5$</td>
    <td>$10^6$</td>
  </tr><tr><td>$23 \sim 25$</td>
    <td>$4 \times 10^7$</td>
    <td>$10^9$</td>
    <td>$1$<br></td>
  </tr></tbody></table><p>�������в�����������$type \in {0,1},2 \leq n \leq 4 \times 10^7,1 \leq a_i \leq 10^9,1 \leq m \leq 10^5,1 \leq l_i \leq r_i \leq 10^9,0 \leq x,y,z,b_1,b_2 &lt; 2^{30}$</p>
<p>�������� $type=0$ �Ĳ��Ե㣬��֤���մ𰸲����� $4 \times 10^{18}$��</p>
<p><strong>ʱ������:</strong> $2\texttt{s}$</p>
<p><strong>�ռ�����:</strong> $1\texttt{GB}$</p>
<h2>����Hack����</h2>
<p>�����hack���ݶ���$type = 0$������$2 \le n \le 500000$������$type = 1$������$2 \le n \le 40,000,000$�� ����matthew99</p>
<h2>����</h2>
<p><a href="./20897/file/attachment.zip">������������</a></p>
