<p>DZY��ʼ�� $n$ ���㣬���������� $n$ ��������� $m$ �β��������ڵ� $i$ ���������� $1$ ��ʼ��ţ��п��ܵ����������</p>
<ol><li>Add a b�� ��ʾ�� $a$ �� $b$ ֮������һ������Ϊ $i$ �ıߣ�<strong>ע�⣬$i$�ǲ������</strong>������֤ $1 \leq a, b \leq n$��</li>
<li>Delete k�� ��ʾɾ���˵�ǰͼ�б�Ȩ����k���ߡ���֤ $k$ һ������ȵ�ǰͼ�бߵ������ࡣ</li>
<li>Return�� ��ʾ������ $i-1$ �β�������֤�� $1$ �β������� Return �ҵ� $i-1$ �β��� Return ������</li>
</ol><p>������ÿ�β��������DZY��ǰͼ����С��������Ȩ�͡������С����������������� $0$��</p>
<h2>�����ʽ</h2>
<p>��һ������������ $n,m$����ʾ�� $n$ ���� $m$ ��������
������ $m$ ��ÿ������һ��������</p>
<h2>�����ʽ</h2>
<p>����ÿһ���������һ��һ��������ʾ��ǰ��С��������Ȩ�͡�</p>


<pre><code class="language-input1">2 2
Add 1 2
Return
</code></pre>


<pre><code class="language-output1">1
0
</code></pre>



<pre><code class="language-input2">5 10
Add 2 1
Add 3 2
Add 4 2
Add 5 2
Add 2 3
Return
Delete 1
Add 2 3
Add 5 2
Return
</code></pre>


<pre><code class="language-output2">0
0
0
10
10
10
0
0
15
0
</code></pre>

<h2>������</h2>
<p>��������������</p>
<h2>������Լ��</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th>
<th>$n$</th>
<th>$m$</th>
<th>����</th>
</tr></thead><tbody><tr><td>1</td><td rowspan="3">$n \leq 10^3$</td><td rowspan="3">$m \leq 10^3$</td><td>ֻ��Add����</td></tr><tr><td>2</td><td></td></tr><tr><td>3</td><td></td></tr><tr><td>4</td><td>$n \leq 2 \times 10^5$</td><td>$m \leq 2 \times 10^5$</td><td rowspan="2">ֻ��Add����</td></tr><tr><td>5</td><td>$n \leq 3 \times 10^5$</td><td>$m \leq 5 \times 10^5$</td></tr><tr><td>6</td><td>$n \leq 2 \times 10^5$</td><td>$m \leq 2 \times 10^5$</td><td rowspan="2">û��Return����</td></tr><tr><td>7</td><td>$n \leq 3 \times 10^5$</td><td>$m \leq 5 \times 10^5$</td></tr><tr><td>8</td><td>$n \leq 2 \times 10^5$</td><td>$m \leq 2 \times 10^5$</td><td></td></tr><tr><td>9</td><td rowspan="2">$n \leq 3 \times 10^5$</td><td rowspan="2">$m \leq 5 \times 10^5$</td><td></td></tr><tr><td>10</td><td></td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$64\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20454/file/attachment.zip">������������</a></p>
