<p>СP���������ʯͷ�����������ۿ���һ��ɳ��ʯͷ����������</p>
<p>�������� $2^n$ ��ɳ��μӣ� ��Ϊ $n$ �֣���ÿ���У��� $0$ λѡ�ֺ͵� $1$ λѡ�ֶ�ս��ʤ����Ϊ�µĵ� $0$ λѡ�֣��� $2$ λ�͵� $3$ λ��ս��ʤ����Ϊ�µĵ� $1$ λѡ�֣��Դ����ơ�</p>
<p>СP��֪��ÿ��ɳ����һ�̶ֹ���ƫ�����ߣ�ÿ��ɳ����ÿһ�ζ�ս�ж�ֻ��ʹ������ƫ�����ߡ�</p>
<p>���һ�ζ�ս��˫����ƫ��������ͬ����ô��ζ�ս����Զ�����������ô��Ϊ���ڻ�ʮ�����ġ�</p>
<p>���ڣ�СP֪����ƫ��ÿ�־��ߵ�ɳ����Ŀ������֪��һ���ܹ���������ʤ���ĳ�ʼ�Ĵ���</p>
<p>���ж��ֿ��ܴ���������<strong>�ֵ�����С</strong>��Ϊ�𰸡�</p>
<p>��Ϊ�𰸿��ܺܳ�����ֻ��Ҫ����𰸵�$hash$ֵ�Լ���$l$��$r$λ��</p>
<p>$$hash=\sum_{i=0}^{2^n-1}S_i \times 233^i \bmod998244353$$</p>
<p>($S_i$��ʾ��ʼ���Ϊ$i$���˵�ƫ�þ��߶�Ӧ�Ĵ�д��ĸ ASCII ��)</p>
<h2>�����ʽ</h2>
<p>��һ����������$n, op$����ʾ���ݹ�ģ���������͡�</p>
<p>�ڶ���һ������������ʾƫ������Ϊʯͷ$R$��������</p>
<p>������һ������������ʾƫ������Ϊ����$S$��������</p>
<p>������һ������������ʾƫ������Ϊ��$P$��������</p>
<p>��$op\neq 1$�����壬���У�����$n$λ��������$l,r$����ʾҪ��������ķ�Χ��</p>
<h2>�����ʽ</h2>
<p>�������ںϷ���ʼ���У����<code>-1</code>������</p>
<p>��$op\neq 2$�����һ����������ʾ��������$hash$ֵ��</p>
<p>��$op\neq 1$�����һ����$"R,S,P"$���ɵ��ַ�������ʾ�������еĵ�$l$��$r$λ��</p>


<pre><code class="language-input1"><code>4 3
4
4
8
0000
1111</code>
</code></pre>

<pre><code class="language-output1"><code>-1</code>
</code></pre>


<pre><code class="language-input2"><code>1 1
1
1
0</code>
</code></pre>

<pre><code class="language-output2"><code>19421</code>
</code></pre>


<pre><code class="language-input3"><code>2 2
1
2
1
01
10</code>
</code></pre>

<pre><code class="language-output3"><code>SR</code>
</code></pre>


<pre><code class="language-input4"><code>3 3
2
3
3
011
110</code>
</code></pre>

<pre><code class="language-output4"><code>879001374
SPSR</code>
</code></pre>
<h2>��������������</h2>
<p>�������������ء�</p>
<h2>������Լ��</h2>
<p>�������������ԡ�</p>
<p>������������������� $1\ \leq\ n\ \leq\ 300000,\ 0\leq\ r-l\leq\ 300000 ,\ R+S+P=2^n$��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-verticle-middle"><thead><tr><th>��������</th><th>�������ֵ</th><th>$n$�ķ�Χ</th><th>$r-l$�ķ�Χ</th><th>��������</th></tr></thead><tbody><tr><td>$1$</td><td>3</td><td>$4$</td><td>$10$</td><td>$3$</td></tr><tr><td>$2$</td><td>19</td><td>$20$</td><td>$1000$</td><td>$3$</td></tr><tr><td>$3$</td><td>11</td><td>$2000$</td><td>$10000$</td><td>$1$</td></tr><tr><td>$4$</td><td>8</td><td>$2000$</td><td>$10000$</td><td>$2$</td></tr><tr><td>$5$</td><td>14</td><td>$2000$</td><td>$10000$</td><td>$3$</td></tr><tr><td>$6$</td><td>15</td><td>$300000$</td><td>$300000$</td><td>$1$</td></tr><tr><td>$7$</td><td>10</td><td>$300000$</td><td>$300000$</td><td>$2$</td></tr><tr><td>$8$</td><td>20</td><td>$300000$</td><td>$300000$</td><td>$3$</td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�$\texttt{1s}$</strong></p>
<p><strong>�ռ����ƣ�$\texttt{512MB}$</strong></p>
<h2>����</h2>
<p><a href="./20847/file/attachment.zip">������������</a></p>
