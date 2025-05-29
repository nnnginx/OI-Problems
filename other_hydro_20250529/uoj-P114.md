<p>���ڵ��ż����ķ�չ����Ϣ�Ľ������ʮ�ַ��㡣</p>
<p>������ $n$ ���ˣ����α��Ϊ $1, \dots, n$����ʼʱ�� $i$ �����ֻ���洢�ű��Ϊ $i$ �������ܱ��顣���ڶ��Լ��ı��鲢��ʮ�����⣬���Ǽƻ�����һ�δ󽻻���</p>
<p>�� $n$ ��������һЩ���ѹ�ϵ�����Գ���Ϊһ��������ͼ $G$��������ͼ�����ر����Ի�������ͼ��</p>
<p>ÿ����������״̬�����������������⡣��ʼʱ��Ϊ������</p>
<p>��һ�������ˣ��������ǰ����·�ʽ�ж���</p>
<pre><code class="sh_php">function dfs(v):
    v ��Ϊ����״̬
    for u = 1, ..., n:
        if v �� u ������ and u ���ڲ���״̬:
            ���� v �� u ���ֻ��е������ܱ���
            dfs(u)
    v ��Ϊ����״̬

for v = 1, ..., n:
    if v ���ڲ���״̬:
        dfs(v)</code></pre>
<p>һ�������һλ����ѧ�ҵ���������ÿ���ֻ��д洢�������ܱ���ı�ţ���Ҫ��ԭ�����ѹ�ϵͼ $G$��Ȼ���⼸���ǲ����ܵģ���������֪���ж����ֿ��ܵ� $G$��</p>
<h2>�����ʽ</h2>
<p>��һ��һ�������� $n$��</p>
<p>�ڶ��а��� $n$ ������ $a_1, \dots, a_n$����ʾ���յ� $i$ ���˵��ֻ��ϴ洢�������ܱ����š���֤ $a_1, \dots, a_n$ ��һ�� $1$ �� $n$ �����С�</p>
<h2>�����ʽ</h2>
<p>һ�У�һ��������ʾ $G$ ����������ֻ������𰸶� $998244353$��$7 \times 17 \times 2^{23} + 1$��һ��������ȡģ��Ľ����</p>


<pre><code class="language-input1">3
2 3 1
</code></pre>


<pre><code class="language-output1">2
</code></pre>


<p>���������֣�</p>
<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/114/sample.png" alt="��������ͼ"></p>


<pre><code class="language-input2">9
7 2 9 1 3 8 6 5 4
</code></pre>


<pre><code class="language-output2">3528
</code></pre>

<h2>������</h2>
<p>�������������ء�</p>
<h2>������Լ��</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th>
<th>$n$�Ĺ�ģ</th>
</tr></thead><tbody><tr><td>1</td><td>$n \leq 6$</td></tr><tr><td>2</td><td rowspan="2">$n \leq 9$</td></tr><tr><td>3</td></tr><tr><td>4</td><td rowspan="4">$n \leq 50$</td></tr><tr><td>5</td></tr><tr><td>6</td></tr><tr><td>7</td></tr><tr><td>8</td><td rowspan="3">$n \leq 500$</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20554/file/attachment.zip">������������</a></p>
