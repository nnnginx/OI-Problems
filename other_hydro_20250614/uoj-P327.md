<p>Scape��Mythological�������漸�γ�̵ľ���֮��Mythological�ǳ����ˣ����Ƽ���Scapeһ����ϷTo the moon��</p>
<p>��Ϸ��һλ����John�ļ��䱻ҩ�ﳾ�⣬�����˽���������ʽ֮��Scape���������ļ��䡣</p>
<p>John�ļ�������һ������RiverŮ������Ӱ��������������ֽ���ӣ���һ��ɳ����һֻѼ������ż��һ��������Scape������Ĵ��ˡ�</p>
<p>���ҵ�Ѽ���޺�ɳ�����������أ��� Scape�����뵽�����������Mythological���������� $n$ ��������е� $i$ �ݵ������� $a_i$����Щ���ﰴ˳���ų�һ�С�</p>
<p>����ѡ����ķ�ʽ���ر���ÿ�λ�ѡ������<strong>������ͬ</strong>������������������������֮��û��<strong>��δ����</strong>�������������������ߡ�</p>
<p>����Scape���������ɴ�ѯ�ʣ�ÿ��ѯ��������͸����������� $\left [L_i,R_i\right ]$ ֮��������ô����������߶��ٷ����</p>
<h2>����</h2>
<p>����Ҫ��д��������/���̣��������Ŀ������</p>
<ul><li>init(n, m, a[], t);<ul><li>�ڳ����ʼ����ʱ�����һ������ɳ�ʼ����</li>
<li>$n$ ��ʾ $a$ �ĳ����� $n$��$m$ ��ʾ $a_i$ ��������ֵ��$a$ ������±�� $1$ ��ʼ��$t$ ��ʾ�������š�</li>
</ul></li>
<li>query(l, r);<ul><li>��ʾѯ������ $\left [L ,R\right ]$ �Ĵ� ��</li>
<li>��֤ $L\leq R$��</li>
</ul></li>
</ul><h2>ʵ��ϸ��</h2>
<p>����ֻ֧�� C/C++��</p>
<p>��ֻ���ύһ��Դ�ļ�ʵ������������ init �� query ����/���̣�������ѭ����������ͽӿڡ�����Ҫ����ͷ�ļ� mythological.h��</p>
<pre><code class="sh_cpp">void init(int n, int m, int a[], int t);
int query(int l, int r);</code></pre>
<p>����в�����ĵط��������������������أ�<strong>�ڸ�����������</strong>��</p>
<p>���������Ҫռ��$8\texttt{MB}$���ڴ��$100\texttt{ms}$��ʱ�䡣</p>
<p>��Ϊ�����ʹ����fread�����п��ٶ��룬�������������������ݵ�ѡ����Ҫ������������Ϻ���"<samp>Ctrl+D<samp>"������EOF��</samp></samp></p>
<h2>���ⷽʽ</h2>
<p>����ϵͳ���������¸�ʽ���������ݣ�</p>
<ol><li>�� $1$ �У��ĸ����� $n,m,q,t$���ֱ�������������ݵĴ�С��$a_i$ ��������ֵ��ѯ�ʸ������������š�</li>
<li>�� $2$ �У�$n$ ���������� $i$ ��������ʾ $a_i$��</li>
<li>�� $2+i$ �У�$1\le i\le q$������������ $L_i,R_i$����ʾѯ�ʵ����䡣</li>
</ol>

<pre><code class="language-input1">9 10 3 0
1 1 3 2 1 1 2 3 1
2 9
1 2
2 5
</code></pre>


<pre><code class="language-output1">8
2
0
</code></pre>



<pre><code class="language-input2">10 10 3 0
1 2 3 4 5 6 7 8 9 10
1 9
2 3
4 5
</code></pre>


<pre><code class="language-output2">0
0
0
</code></pre>


<h2>������</h2>
<p>�����������������ء�</p>
<h2>������Լ��</h2>
<p>�����������ݣ�$1\le n\le 1\times 10^5$��$1\le m\le 1\times10^5$��$ q\leq 2\times 10^6$��$ L_i \le  R_i$��</p>
<p>Ϊ���õ�ÿ��������ķ����������ͨ��<strong>����</strong>��������������</p>
<div class="table-responsive">
 <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>������</th>
    <th>��ֵ</th>
    <th>$n$</th>
    <th>$q$</th>
    <th>��������</th>
    <th>������subtask</th>
   </tr></thead><tbody><tr><td>1</td>
    <td>20</td>
    <td>$\le 1000$</td>
    <td>$\le 1000$</td>
    <td>��</td>
    <td>��</td>
   </tr><tr><td>2</td>
    <td>16</td>
    <td>$\le 1\times 10^5$</td>
    <td>$\le 1\times 10^5$</td>
    <td>ÿ��Ȩֵ����������</td>
    <td>$1$</td>
   </tr><tr><td>3</td>
    <td>25</td>
    <td>$\le 1\times 10^5$</td>
    <td>$\le 1\times 10^5$</td>
    <td>ѯ�ʵ� $L,R$ ���ɷ�ʽ���������£�</td>
    <td>$1$</td>
   </tr><tr><td>4</td>
    <td>19</td>
    <td>$\le 1\times 10^5$</td>
    <td>$\le 1\times 10^5$</td>
    <td>��</td>
    <td>$1,2,3$</td>
   </tr><tr><td>5</td>
    <td>20</td>
    <td>$\le 1\times 10^5$</td>
    <td>$\le 2\times 10^6$</td>
    <td>��</td>
    <td>$1,2,3,4$</td>
   </tr></tbody></table></div>



<p>������3����ѯ�ʵķ�ʽ���£�</p>
<p>����
$$F_i=(2000i^2+629i+2333) \bmod n+1$$</p>
<p>������е� $1\le i\le q$����
$$L_i = \min\left\{F_{2i-1},F_{2i} \right\}$$
$$R_i = \max\left\{F_{2i-1},F_{2i} \right\}$$</p>
<p><a href="/faq">����ʽ���͵���Ŀ��ô���ز���</a></p>
<p><strong>ʱ�����ƣ�</strong>$2\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20753/file/attachment.zip">������������</a></p>
