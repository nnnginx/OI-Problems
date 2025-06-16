<p>SingleDog���跨�����˺��ģ����Ƿ��֣���̨TPU�����ĳ��������һ��ÿ��������Ӧһ����ɫ����Ļ�ϳ����˰�쵵�ɫ����</p>
<p>������˵�����Ƿ�����һ������Ϊ$n$����ɫ����ÿ��λ���Ǻ�/��/�̣���Ϊ <samp>R/G/B</samp> ��������ɫ�е�һ�֡�Ϊ�˳��׶ž�AlphaGo������Ȧ������������Ҫ���ⲿ�ִ�����ȫ��д��</p>
<p>�������������������Ϣ��ÿ�������ѡ�����ڵ�����ɫ�飬����һ�β�����Ϊ�˷�����⣬�ǲ���ǰ������λ�õ���ɫΪ $c_a,c_b$ ���������Ϊ $c_a^{'},c_b^{'}$ ��</p>
<ol><li>�����ѡ�������ɫ����ͬɫ�� $c_a=c_b$ ��������԰����Ǳ������<strong>��ͬ������ɫ</strong>���� $c_a^{'}\neq c_b^{'},c_a\neq c_a^{'},c_b\neq c_b^{'}$ �������磬����ѡ���� <samp>GG</samp> ������Խ����Ǳ�Ϊ <samp>RB</samp> �� <samp>BR</samp>��</li>
<li>�����ѡ�������ɫ������ɫ�� $c_a\neq c_b$ ��������԰����Ǳ������<strong>��ͬ������ɫ</strong>���� $c_a^{'}=c_b^{'},c_a\neq c_a^{'},c_b\neq c_b^{'}$ �������磬����ѡ���� <samp>RB</samp> ������Խ����Ǳ�Ϊ <samp>GG</samp> ��</li>
</ol><p>���Ŀ���ǰ��⴮�����״̬ $S$ ��Ϊ״̬ $T$ ������С������</p>
<h2>�����ʽ</h2>
<p>��һ��һ�������� $n$ ����ʾ�⴮����ĳ��ȡ�</p>
<p>�ڶ���һ������Ϊ $n$ ���ַ��� $S$ ����ʾ�⴮�������ʼ״̬��</p>
<p>������һ������Ϊ $n$ ���ַ��� $T$ ����ʾ�⴮�������ֹ״̬��</p>
<h2>�����ʽ</h2>
<p>���һ��һ����������ʾ���⴮�����״̬ $S$ ��Ϊ״̬ $T$ ����С������</p>


<pre><code class="language-input1">3
GBR
BBB
</code></pre>


<pre><code class="language-output1">3
</code></pre>


<p>��һ�β����� <samp>GB</samp> ��Ϊ <samp>RR</samp> ��������Ĵ���Ϊ <samp>RRR</samp> ��</p>
<p>�ڶ��β����� <samp>RR</samp> ��Ϊ <samp>BG</samp> ��������Ĵ���Ϊ <samp>BGR</samp> ��</p>
<p>�����β����� <samp>GR</samp> ��Ϊ <samp>BB</samp> ��������Ĵ���Ϊ <samp>BBB</samp> ��</p>
<p>����֤��û�д������ٵĲ������С�</p>


<pre><code class="language-input2">4
GBRB
GRRG
</code></pre>


<pre><code class="language-output2">2
</code></pre>


<p>��һ�β����� <samp>RB</samp> ��Ϊ <samp>GG</samp> ��������Ĵ���Ϊ <samp>GBGG</samp> ��</p>
<p>�ڶ��β����� <samp>BG</samp> ��Ϊ <samp>RR</samp> ��������Ĵ���Ϊ <samp>GRRG</samp> ��</p>
<p>����֤��û�д������ٵĲ������С�</p>


<pre><code class="language-input3">20
RBBGRBBGRBBBBGRBRGGB
RBGRRBRBGBRRGBBBGBGG
</code></pre>


<pre><code class="language-output3">14
</code></pre>


<h2>������Լ��</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th>
<th>$n$�Ĺ�ģ</th>
<th>����</th>
</tr></thead><tbody><tr><td>1</td><td rowspan="2">$n \leq 10$</td><td rowspan="2">��</td></tr><tr><td>2</td></tr><tr><td>3</td><td rowspan="4">$n = 100$</td><td rowspan="3">����һ�ֲ��������� 50 ��ÿ�β���ѡȡ�� $i$ �� $[1,n-1]$ ������Ľ�</td></tr><tr><td>4</td></tr><tr><td>5</td></tr><tr><td>6</td><td rowspan="5">��</td></tr><tr><td>7</td><td rowspan="4">$n\leq 5\times 10^5$</td></tr><tr><td>8</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p>��֤ $S$ �� $T$ ֻ�ɴ�д��ĸ <samp>'R','G','B'</samp> ��ɣ���֤����һ����������������״̬�� $S$ ��Ϊ $T$ ��</p>
<p><strong>ʱ�����ƣ�</strong>$2\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<p>������ʾ����Ŀ�ѶȺ���Ŀ˳��<strong>û��</strong>��ϵ</p>
<h2>����</h2>
<p><a href="./20779/file/attachment.zip">������������</a></p>
