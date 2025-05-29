<p>Scape�ǳ�ϲ���ں�Mythological�乫԰��ʱ�򣬽�ʱ�临�Ӷȵ�֪ʶ���������������ܿ�����ĵط���Mythological�Ը��Ӷȵ���Ȥ����û���Աߵ�����жӱ��ݵ���Ȥ�ߣ�ֻ����whx�߿ࡣ</p>
<p>whx���Scape���ɻ󣬸���������Ҫ����Mythologicalϲ��ʲô�����������Լ�ϲ��ʲô��Scape����Mythological�ر�ϲ����Geometry Dash����������������һ�����档</p>
<p>����Ϸ��Scape����ƽ��ֱ������ϵ���� $n$ ����� $P_0,P_1,\cdots,P_{n-1}$ �� $m$ ������ $Q_0,Q_1,\cdots,Q_{m-1}$���������� $n+m$ �����ԭ�� $O$ һ�� $n+m+1$ �����У��������㲻���ߡ���</p>
<p>Scape�ܿ췴Ӧ��������ԭ�� $O$ ������������� $P_i,P_j$ Ϊ���㹹�ɵ������� $OP_iP_j$ һ���� ${n(n-1)\over 2}$ ����</p>
<p>���һ�������ε��ڲ��������κ����㣬Scape�Ƹ��������ǿյģ�����Scape�Ƹ��������Ƿǿյġ�</p>
<p>Scape���������ж���ԭ��������������Ϊ���㹹�ɵ� ${n(n-1)\over 2}$ ���������У�ÿ���������ǿյĻ��Ƿǿյġ�Ϊ��֤��һ�������ηǿգ�����ÿ���ǿյ������Σ����������һ���ڸ��������ڲ������� $Q_k$��$0\le k &lt; m$����</p>
<h2>����</h2>
<p>����Ҫ��дһ������ check_triangles���������Ŀ������</p>
<ul><li>check_triangles(n, m, rx, ry, bx, by, result)<ul><li>n: ����ϵ�ϸ����ĺ�������</li>
<li>m: ����ϵ�ϸ��������������</li>
<li>rx: ��СΪ $n$ �����飻rx[i] ��ʾ��� $P_i$ �ĺ����꣬���� $0\le i &lt; n$��</li>
<li>ry: ��СΪ $n$ �����飻ry[i] ��ʾ��� $P_i$ �������꣬���� $0\le i &lt; n$��</li>
<li>bx: ��СΪ $m$ �����飻bx[i] ��ʾ���� $Q_i$ �ĺ����꣬���� $0\le i &lt; m$��</li>
<li>by: ��СΪ $m$ �����飻by[i] ��ʾ���� $Q_i$ �������꣬���� $0\le i &lt; m$��</li>
<li>result: ��СΪ $n\times n$ �Ķ�ά���飻����Ҫ�������� $OP_iP_j$��$0\le i &lt; j &lt; n$�����жϽ����ŵ� result[i][j] �У��������� $OP_iP_j$ �ǿգ�������һ�������ڲ������� $Q_k$ �ı�� $k$ ��ŵ� result[i][j] �У����� $-1$ ��ŵ� result[i][j] �С��㲻Ӧ������ $0\le i &lt; j &lt; n$ ��Χ����� result[i][j]��</li>
</ul></li>
</ul><h2>ʵ��ϸ��</h2>
<p>����ֻ֧�� C/C++��</p>
<p>��ֻ���ύһ��Դ�ļ�ʵ������������ check_triangles ������������ѭ����������ͽӿڡ�����Ҫ����ͷ�ļ� triangles.h��</p>
<pre><code class="sh_cpp">void check_triangles(int n, int m, int *rx, int *ry, int *bx, int *by, int **result);</code></pre>
<p>����в�����ĵط��������������������أ�<strong>�ڸ�����������</strong>��</p>
<h2>���ⷽʽ</h2>
<p>����ϵͳ���������¸�ʽ���������ݣ�</p>
<ol><li>�� $1$ �У��������� $\mathrm{type}$��ֵΪ $0$ �� $1$����</li>
<li>�� $2$ �У�$n$, $m$��</li>
<li>�� $3+i$ �У�rx[i], ry[i]��</li>
<li>�� $3+n+i$ �У�bx[i], by[i]��</li>
</ol><p>�����������ݣ�$\mathrm{type}=1$������ϵͳ������� $n-1$ �У����е� $i+1$ �а��� $n-i-1$ ������������Ϊ result[i][i+1], result[i][i+2], ..., result[i][n-1] ��ֵ��</p>
<p>���ڲ������ݣ�$\mathrm{type}=0$������ϵͳ�����һ��һ����������ʾ�������ݺ� result �������õ���У��͡�</p>
<p>ע�⣺$\mathrm{type}=0$ ʱ���·��Ĳ���������У���Ϊ result[i][j]��$0\le i &lt; j &lt; n$���зǸ����ĸ�����<strong>��������ʱ��У��ͼ��㷽�����·��Ĳ�������㷽����ͬ��</strong></p>


<pre><code class="language-input1">1
4 3
3 3
-2 4
5 -5
-4 -2
3 -1
1 0
-3 -2
</code></pre>


<pre><code class="language-output1">-1 0 -1
1 -1
2
</code></pre>


<p>����ͼ��ʾ��</p>
<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/326/326.png" alt="��������" width="300"></p>
<p>��������� result[0][2]=0 ���Ըĳ� 1��������Ϊ $B_1(1,0)$ ͬ������ $O(0,0),A_0(3,3),A_2(5,-5)$ Ϊ����������� $OA_0A_2$ �ڲ���</p>
<h2>������</h2>
<p>�����������������ء���������������� $17926$ ���Ǹ�����</p>
<h2>������</h2>
<p>�����������������ء���������������� $38756$ ���Ǹ�����</p>
<h2>������Լ��</h2>
<p>�����������ݣ�$2\le n\le 4000$��$1\le m\le 4000$�����е�ĺᡢ��������� $[-10^9,10^9]$ ��Χ�ڡ�</p>
<p>Ϊ���⾫������֤�������㹹�ɵļн��� $[10^{-12}\pi,\pi-10^{-12}\pi]$ ֮�䡣</p>
<div class="table-responsive">
 <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>������</th>
    <th>��ֵ</th>
    <th>$n$</th>
    <th>$m$</th>
   </tr></thead><tbody><tr><td>1</td>
    <td>32</td>
    <td>$\le 200$</td>
    <td>$\le 200$</td>
   </tr><tr><td>2</td>
    <td>46</td>
    <td>$\le 1200$</td>
    <td>$\le 1200$</td>
   </tr><tr><td>3</td>
    <td>22</td>
    <td>$\le 4000$</td>
    <td>$\le 4000$</td>
   </tr></tbody></table></div>

<p><a href="/faq">����ʽ���͵���Ŀ��ô���ز���</a></p>
<p><strong>ʱ�����ƣ�</strong>$2\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20752/file/attachment.zip">����������������</a></p>
