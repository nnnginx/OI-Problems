<p>���й���Ա������ȫ���ܹ��� $n$ �����У����� $1$ �ų������׶�����Ϊ������Ŀ̫�࣬�ڳ���֮ǰͨ�žͳ���һ�������⡣</p>
<p>��ս������֮ǰ���Ƽ��������й����ڲ�����ԭʼ�ķ�ʽͨ�š�����һЩ���úܿ�����е����ʲ�ڳ��м����������ż�����Ϊ��Щ����������úܿ죨����ۼ��߻�Ҫ�죩���������й�����ά��������ͨ�š������ھ�����������ս����ȫ���󲿷ֵĵ�·���ܵ������ص��ƻ�����Щ���úܿ�����У����ܵ������ƻ��ĵ�·��Ҳֻ�������������м��ͨ��Ч�ʾͱ�õ����ˡ����޵�·��Ҫ���Ѵ����������������ڶ����ڿ�����ϣ����</p>
<p>���ؾ�����������ĸ��¼�����������绰�����������⡣����绰�������ɶԵģ�ÿһ������绰�����Է������鲨���໥������Ϣ��������֪��������ֻ��Ҫ�� $n-1$ �Գ��м䰲װ����绰�������������м�Ͷ�����ֱ�ӻ���ͨ���ˡ�</p>
<p>���ڷ����Ѿ��ⶨ��һ�����յİ�װ�ƻ������������Ҫ��װ����绰�� $n-1$ �Գ��С������ڰ�װ��Щ�绰��˳��ȴ����һ�����⣬���ؾ���������ķ�ʽ����װ���ǣ�</p>
<ul>
<li>��ʼʱ��û���κγ��а�װ�˵绰���ǰ������ $1$ �ų���ֱ�ӻ���ͨ�ŵĳ��м���Ϊ $S$  ����ʼʱ $S=\{1\} $��</li>
<li>ÿһ�������ֲ�����ѡ��һ���� $S$ ���ҵ�ǰ����<strong>ֱ��</strong>ͨ�ţ����гɶԵ绰���ĳ��� $x$ �� $y$ ��$x &lt; y$������ѡ����һ������ $S$ �еĳ��� $z$  ����ȥ $x$ �� $y$ ��ɶԵĵ绰�����ֱ��� $x$ �� $z$ �� $y$ �� $z$ �������ɶԵĵ绰���� $z$ ���� $S$ ������ѡ��һ���� $S$ �еĳ��� $x$ �Ͳ��� $S$ �еĳ��� $y$ ���� $x$ �� $y$ �������ɶԵ绰���� $y$ ���� $S$ ��</li>
<li>�ظ��������̣�ֱ�����г��ж��� $S$ �С���Ȼ��ǡ�û�ִ�� $n-1$ ������Ĺ��̡�</li>
</ul>
<p>���׿���������İ�װ��ʽ������Ҫ���еĲ�����Ŀ���٣����ܱ�֤����ʱ���� $S$ �еĳ��ж���ֱ�ӻ���ͨ�š�</p>
<p>�����׷��ּ�ʹ���������յİ�װ�ƻ�����������ʽ��ɼƻ��ľ��巽��Ҳ����Ψһ�ġ����ؾ��������п��ܵľ��巽�������һ����������Ҫ���ȼ�������ܵķ������������ڴ𰸿��ܴܺ���ֻ��Ҫ����𰸶� $998244353$ ȡģ���ֵ��</p>
<p>���������ǲ�ͬ�ģ����ҽ���ĳһ��ִ�еĲ�������ȫ��ͬ��</p>
<h2>�����ʽ</h2>
<p>��һ��һ�������� $n$ ��</p>
<p>������ $n-1$ �У�ÿ������������ $u_i,v_i$ ����ʾ��װ�ƻ���һ�԰�װ�绰�ĳ��С�</p>
<h2>�����ʽ</h2>
<p>���һ��һ���Ǹ���������ʾ�𰸶� $998244353$ ȡģ���ֵ��</p>


<pre><code class="language-input1">4
1 2
2 3
2 4
</code></pre>


<pre><code class="language-output1">4
</code></pre>


<p>������ $(x,y,z)$ �� $(x,y)$ �ֱ��ʾ���ֲ����������� $4$ �ֺϷ��ķ�����</p>
<p>���� $1$ �� $(1,2),(2,3),(2,4)$ ��</p>
<p>���� $2$ �� $(1,2),(2,4),(2,3)$ ��</p>
<p>���� $3$ �� $(1,3),(1,3,2),(2,4)$ ��</p>
<p>���� $4$ �� $(1,4),(1,4,2),(2,3)$ ��</p>


<pre><code class="language-input2">10
1 9
4 8
10 6
9 7
7 3
4 6
5 7
6 3
2 9
</code></pre>


<pre><code class="language-output2">56980
</code></pre>

<h2>������</h2>
<p>�������ļ��� <code>ex_telephone3.in</code> �� <code>ex_telephone3.out</code> ��</p>
<h2>���ݷ�Χ</h2>
<p>�����������ݣ� $2\leq n\leq 10^5,1\leq u_i,v_i \leq n$ ����֤�����ļƻ��ǺϷ��ģ�������һ�Գ��ж�����ֱ�ӻ���ͨ�š�</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">$n\leq$</th>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">��ֵ</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;" rowspan="4">��</td>
<td style="text-align:center;">$9$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$20$</td>
<td style="text-align:center;">$11$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$200$</td>
<td style="text-align:center;">$16$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$2000$</td>
<td style="text-align:center;">$21$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;" rowspan="2">$10^5$</td>
<td style="text-align:center;">�� $1$ �ų��е�������е����ͨ��·���ϳ��и��������� $3$</td>
<td style="text-align:center;">$14$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">��</td>
<td style="text-align:center;">$29$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ������</strong>��$1\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./21011/file/attachment.zip">������������</a></p>
