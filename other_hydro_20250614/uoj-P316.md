<p>�����Ǹ������Ů���ӡ�</p>
<p>������ڵ��ˣ�������������������������Ӿ���������������ҵ�˽�˺�̲��Ȧһ�鳤���εĺ�����Ϊ��Ӿ����Ȼ���������Ÿ��ָ�����Σ�գ���Щ�ط�ˮ̫���Щ�ط��д�����ˮĸ��û��������Ȧ��������һ�麣���ǰ�ȫ�ġ�</p>
<p>���������ķ�����������麣��������һ���ױ߳�Ϊ $N$ �ף���Ϊ $1001$ �׵ĳ�����������������ĵױ߶�Ӧ�����ҵ�˽�˺�̲��ÿһ�� $1 ��\times 1 ��$ ��С�����ζ�������һ����λ���������������ְ�����ȥ����ÿһ��С�������Ƿ�ȫ���ڵ�֪����Ϣ֮����Ҫ���ľ���Ȧ������Ҫ����Ӿ������</p>
<p>����Ŀ���������Ӿ��������������������</p>
<ul><li>���뱣֤��ȫ�ԡ�����Ӿ���е�ÿһ����λ�����ǰ�ȫ�ġ�</li>
<li>�����Ǿ��Ρ�����Ӿ�����������������е�һ�� $a \times b$ ��������</li>
<li>����ͺ�̲���ڡ�����Ӿ�����±߽�������������±߽硣</li>
</ul><p>���磺�� $N=5$ ʱ���������Ľ�����£���Ϊ $1001$ ̫�����ֻ�����������������е���Ϣ���������ֶ���Σ�յģ���</p>
<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/316/1.png" alt="��Ӿ��" style="width:400px;"></p>
<p>��ô������ѡȡ������һ�е� $1 \times 4$ ���Ӻ���Ҳ����ѡ������е� $3 \times 1$ ���Ӻ���ע��������ѡȡ������һ�е� $1 \times 5$ ���Ӻ�����Ϊ��û���뺣̲���ڡ�</p>
<p>Ϊ������������Ŀ��ģ���������Ӿ������������ܵĴ��������ѡȡ��������һ�е� $1 \times 4$ ���Ӻ�����Ϊ���շ�����</p>
<p>��Ȼ��Ҫ�������֪��ÿһ����λ�����Ƿ�ȫ�����������ھ����ж���������һ��������Ӿ������ж�󡣾����򵥵Ĺ��ƣ�������ÿһ����λ�����ж����� $q$ �ĸ����ǰ�ȫ�ģ�$1-q$ �ĸ����ǲ���ȫ�ġ�����Ҫ֪������ѡ���������Ӿ�������<strong>ǡ��</strong>Ϊ $K$ �ĸ����Ƕ��١�</p>
<p>Ȼ����������ѧ��������Ȥ�����������������������һ�������ֵ��</p>
<h2>�����ʽ</h2>
<p>�ӱ�׼����������ݡ�</p>
<p>����һ���ĸ������� $N,K,x,y$������ $1 \leq x &lt; y &lt; 998244353$��$q$ ��ȡֵΪ $\frac{x}{y}$�� </p>
<h2>�����ʽ</h2>
<p>�������׼�����</p>
<p>���һ��һ��������ʾ����ģ $998244353$ �����µ�ȡֵ��</p>
<p>����𰸻�Ϊ����ʽ�����ʽΪ $\frac{a}{b}$ ������ $a$ �� $b$ �Ļ��ʡ�������� $x$ ʹ�� $bx \equiv a \mod 998244353$ �� $0 \leq x &lt; 998244353$������֤������������ $x$ ��Ψһ�ġ� </p>


<pre><code class="language-input1">10 5 1 2
</code></pre>



<pre><code class="language-output1">342025319
</code></pre>

<h2>������</h2>
<p>���������������ء�</p>
<h2>������</h2>
<p>���������������ء�</p>
<h2>��ʾ</h2>
<p>$x^{p-1} \equiv 1 \mod p$������ $p$ Ϊ������$x \in [1,p)$��</p>
<h2>������Լ��</h2>
 <div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th rowspan="1">���Ե���</th><th rowspan="1">$N$</th><th rowspan="1">$K$</th></tr></thead><tbody><tr><td rowspan="1">1,2</td><td rowspan="1">$=1$</td><td rowspan="1">$\leq 1000$</td></tr><tr><td rowspan="1">3</td><td rowspan="1">$\leq 10$</td><td rowspan="1">$\leq 8$</td></tr><tr><td rowspan="1">4</td><td rowspan="1">$\leq 10$</td><td rowspan="1">$\leq 9$</td></tr><tr><td rowspan="1">5</td><td rowspan="1">$\leq 10$</td><td rowspan="1">$\leq 10$</td></tr><tr><td rowspan="1">6</td><td rowspan="1">$\leq 1000$</td><td rowspan="1">$\leq 7$</td></tr><tr><td rowspan="1">7</td><td rowspan="1">$\leq 1000$</td><td rowspan="1">$\leq 8$</td></tr><tr><td rowspan="1">8</td><td rowspan="1">$\leq 1000$</td><td rowspan="1">$\leq 9$</td></tr><tr><td rowspan="1">9,10,11</td><td rowspan="1">$\leq 1000$</td><td rowspan="1">$\leq 100$</td></tr><tr><td rowspan="1">12,13,14</td><td rowspan="1">$\leq 1000$</td><td rowspan="1">$\leq 1000$</td></tr><tr><td rowspan="1">15,16</td><td rowspan="1">$\leq 10^9$</td><td rowspan="1">$\leq 10$</td></tr><tr><td rowspan="1">17,18</td><td rowspan="1">$\leq 10^9$</td><td rowspan="1">$\leq 100$</td></tr><tr><td rowspan="1">19,20</td><td rowspan="1">$\leq 10^9$</td><td rowspan="1">$\leq 1000$</td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�</strong>$3\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20743/file/attachment.zip">������������</a></p>
