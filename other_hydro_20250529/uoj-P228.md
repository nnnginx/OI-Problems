<p>sylvia ��һ���Ȱ�ѧϰ��Ů���ӣ���������Ҫѧϰ���ݽṹ���ɡ�</p>
<p>�ڿ���һЩ����ѧ��һЩ���ƺ�����Ҫ��һЩ���ݽṹ���������֡��������ĺ����Ѿ�����������������һ���⡣</p>
<p>����һ������Ϊ $n$ ������ $A$���������� $m$ �β��������������֣�</p>
<ol><li>�������е� $i \in [l,r]$���� $A_i$ ��� $A_i+x$��</li>
<li>�������е� $i \in [l,r]$���� $A_i$ ��� $\lfloor \sqrt {A_i} \rfloor$��</li>
<li>�������е� $i \in [l,r]$��ѯ�� $A_i$ �ĺ͡�</li>
</ol><p>��Ϊһ������ô�����ĳ�ѧ�ߣ�sylvia ���˺þö�û�������������������������ȥ�ˣ�һʱ����ϵ���ϡ���������������Ѱ����������ܰ���������������</p>
<h2>�����ʽ</h2>
<p>��һ����������$ n, m $��</p>
<p>������һ�� $ n $ ���� $A_i$��</p>
<p>������ $ m $ ���У��� $ i $ �е�һ���� $ t_i $ ��ʾ�������ͣ�</p>
<p>�� $ t_i = 1 $����������������� $ l_i, r_i, x_i $����ʾ����һ��</p>
<p>�� $ t_i = 2 $����������������� $ l_i, r_i$����ʾ��������</p>
<p>�� $ t_i = 3 $����������������� $ l_i, r_i$����ʾ��������</p>
<h2>�����ʽ</h2>
<p>����ÿ��ѯ�ʲ��������һ�б�ʾ�𰸡�</p>


<pre><code class="language-input1">5 5
1 2 3 4 5
1 3 5 2
2 1 4
3 2 4
2 3 5
3 1 5
</code></pre>


<pre><code class="language-output1">5
6
</code></pre>

<h2>������</h2>
<p>�������������ء�</p>
<h2>������Լ��</h2>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th><th>$n$ �Ĺ�ģ</th><th>$m$ �Ĺ�ģ</th><th>����Լ��</th></tr></thead><tbody><tr><td>1</td><td rowspan="3">$n \leq 3000$</td><td rowspan="3">$m \leq 3000$</td><td rowspan="3"></td></tr><tr><td>2</td></tr><tr><td>3</td></tr><tr><td>4</td><td rowspan="7">$n \leq 100000$</td><td rowspan="7">$m \leq 100000$</td><td rowspan="2">�����������</td></tr><tr><td>5</td></tr><tr><td>6</td><td rowspan="2">$t_i \neq 1$</td></tr><tr><td>7</td></tr><tr><td>8</td><td rowspan="3"></td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p>�����������ݣ���֤�� $1 \leq l_i \leq r_i \leq n,1 \leq A_i,x_i \leq 10^5$</p>
<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20668/file/attachment.zip">������������</a></p>
