<p>��бһֱ�����Լ��ͱ�����Э�Ǹ�ά�ռ���ĳ�����ε�������֧��֧������۵��֤���кܶࡣ��һ�����Ƕ�����б����Э������������Ƕ��͵����ݻ������ں���˧�������⡢�����������������ǵĺ����Ѷ���þ�ţ����ţ���</p>
<p>��бҲ����˼�����ڸ�ά�ռ�����ͱ�����Э֮����ʲô��ϵ�أ����������ڸ߶ˣ�������������һ����ά�İ汾�ɡ�</p>
<p>�������µķ��Σ�</p>
<ol><li>$0$ ���� <code>o</code> ��һ�� $1\times 1$ ���ַ��������������һ���ַ� <code>o</code>��</li>
<li>$0$ ���� <code>x</code> ��һ�� $1 \times 1$ ���ַ��������������һ���ַ� <code>x</code>��</li>
<li>$i$ ���� <code>x</code> �� <code>o</code> ���� $3^i \times 3^i$ ���ַ���������ͨ���� $i-1$ ����� <code>x</code>,<code>o</code> ͨ�����·�ʽ���еõ�������ʾ <code>x</code>���Ҳ��ʾ <code>o</code>����</li>
</ol><pre>xox ooo
oxo oxo
xox ooo</pre><p>������˵�������� <code>x</code> �� <code>o</code> �ֱ�Ϊ��</p>
<pre>xoxoooxox ooooooooo
oxooxooxo oxooxooxo
xoxoooxox ooooooooo
oooxoxooo oooxoxooo
oxooxooxo oxooxooxo
oooxoxooo oooxoxooo
xoxoooxox ooooooooo
oxooxooxo oxooxooxo
xoxoooxox ooooooooo</pre><p>һ�����һ�����Ӵ�����Ҳֻ�����������һ���֡��������ά�İ汾�У������Χ���Ա�ʾ�� $n$ ����� <code>x</code> �е�һ���Ӿ��Σ��������� $xl$ ������ $xr$ �еĵ� $yl$ ���� $yr$ �С�</p>
<p>��һ���нӴ�����һЩ�����������ģ�������������е� <code>o</code> һ����������һЩ������ͻȻ�����ģ�������������е� <code>x</code> һ��������ЩͻȻ�����������ְ�������һ�������ֳ���һ��һ��ḻ��ʵ�ƪ�¡��������У���бϣ������� $n$ �� <code>x</code> ��ĳһ���Ӿ����У�<code>o</code> ���ָ���˶��ٸ�����ͨ�顣</p>
<p>����һ�����������ַ� <code>o</code> ��ͬһ������ͨ������ҽ�����һ�� <code>o</code> ��������ͣ�������������ƶ���������ֻ���� <code>o</code> ������µ�����һ�� <code>o</code>��</p>
<h2>�����ʽ</h2>
<p>�����һ����һ������ $t(1 \leq t \leq 50)$����ʾ����������</p>
<p>����ÿ�����ݣ��������һ��������� $n, xl, xr, yl, yr (1 \leq n \leq 35, 1 \leq xl \leq xr \leq 3^n, 1 \leq yl \leq yr \leq 3^n)$��</p>
<h2>�����ʽ</h2>
<p>����ÿ�����ݣ����һ��һ��������ʾ <code>o</code> ������ͨ��������𰸿��ܴܺ���ֻ��Ҫ����� $998244353$ ȡģ���ֵ��</p>


<pre><code class="language-input1">5
1 1 3 1 3
2 1 9 1 9
2 3 5 4 8
2 1 6 2 7
35 1 50031545098999707 1 50031545098999707
</code></pre>


<pre><code class="language-output1">4
12
3
5
679477107
</code></pre>


<p>����Ե���������Ϊ�����ڵ����������У��漰�����Ӿ���Ϊ��</p>
<pre>oooxo
xoxoo
oxoox</pre><p>��Ȼ��������Ӿ����У�<code>o</code> �� <code>x</code> ���ֳ��� $3$ ������ͨ�顣</p>
<h2>������Լ��</h2>
<p><strong>Small Task</strong>: $n \leq 35, xr - xl \leq 2$��</p>
<p><strong>Large Task</strong>: $n \leq 35$��</p>
<p><strong>ʱ�����ƣ�</strong>$2\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20933/file/attachment.zip">������������</a></p>
