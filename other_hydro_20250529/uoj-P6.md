<p>СH������о�����㷨������㷨������Ҫͨ��������������ɺ���������Pascal�е�random��C/C++�е�rand�����������ԡ���ʵ�ϣ���������ɺ���Ҳ�����������ġ����������һ�㶼������ĳ���㷨��������ġ�</p>
<p>���磬����������ζ���ʽ�����㷨����һ�������㷨��</p>
<p>�㷨ѡ���Ǹ�����$x_0,a,b,c,d$��Ϊ������ӣ����������µ��ƹ�ʽ���м��㡣</p>
<p>��������$i\ge 1,x_i= \left(ax_{i-1}^2+bx_{i-1}+c \right) \bmod d$��</p>
<p>�������Եõ�һ�����ⳤ�ȵķǸ�����<strong>����</strong>$\{x_i\}_{i\ge 1}$��һ����˵��������Ϊ���<strong>����</strong>������ġ�</p>
<p>�����������$\{x_i\}_{i\ge 1}$�����ǻ����Բ��������㷨������һ��$1$��$K$��<strong>�������</strong>$\{T_i\}_{i=1}^K$��</p>
<ol><li>��ʼ��$T$Ϊ$1$��$K$�ĵ������У�</li>
<li>��$T$����$K$�ν�������$i$�ν���������$T_i$��$T_{(x_i \bmod i)+1}$ ��ֵ��</li>
</ol><p>���⣬СH����$K$�ν����Ļ����ϣ���<strong>����</strong>������$Q$�ν������������ڵ�$i$�ζ��⽻����СH��ѡ�������±�$u_i$��$v_i$��������$T_{u_i}$��$T_{v_i}$��ֵ��</p>
<p>Ϊ�˼������������������㷨��ʵ���ԣ�СH������������⣺</p>
<p>СH��һ��$N$��$M$�е����̣������Ȱ����������̣�ͨ��$N \times M+Q$�ν���������������һ�� $1 \sim N \times M$���������$\{T_i\}_{i=1}^{N\times M}$Ȼ����$N\times M$��������������������������̣�Ҳ���ǵ� $i$ �е� $j$ �еĸ��������������ӦΪ$T_{(i-1)\times M+j}$��</p>
<p>����СHϣ�������̵����Ͻǣ�Ҳ���ǵ�һ�е�һ�еĸ��ӳ�����<strong>ÿ�������߻���������</strong>���ڲ��߳����̵�ǰ���£��ߵ����̵����½ǣ�Ҳ���ǵ�$N$�е�$M$�еĸ��ӡ�</p>
<p>СH�������������ϵ����ֶ���¼��������<strong>����С��������</strong>�������������κ�һ���Ϸ����ƶ�·����СH�����Եõ�һ������Ϊ$N+M-1$���������У����ǳ�֮Ϊ<strong>·������</strong>��</p>
<p>СH��֪���������ܵõ���<strong>�ֵ�����С</strong>��<strong>·������</strong>Ӧ�����������أ�</p>
<h2>�����ʽ</h2>
<p>�����ļ��ĵ�1�а���5������������Ϊ$x_0,a,b,c,d$ ������СH���õ�����������㷨�����������ӡ�</p>
<p>��2�а����������� $N,M,Q$ ����ʾСHϣ������һ��$1$��$N\times M$��������������$N$��$M$�е����̣�����СH�ڳ�ʼ��$N \times M$�ν����������ֽ�����$Q$�ζ���Ľ���������</p>
<p>������$Q$�У���$i$�а�����������$u_i,v_i$����ʾ��$i$�ζ��⽻������������ $T_{u_i}$��$T_{v_i}$��ֵ</p>
<h2>�����ʽ</h2>
<p>���һ�У����� $N+M-1$ ���ɿո����������������ʾ���Եõ����ֵ�����С��·�����С�</p>


<pre><code class="language-input1">1 3 5 1 71
3 4 3
1 7
9 9
4 9
</code></pre>


<pre><code class="language-output1">1 2 6 8 9 12
</code></pre>

<h2>explanation</h2>
<p>���������������ӣ�СH���õ���ǰ$12$�������$x_i$Ϊ��</p>
<pre>9 5 30 11 64 42 36 22 1 9 5 30
</pre>

<p>������$12$���������СH�ڽ��г�ʼ��$12$�ν���������õ�������Ϊ��</p>
<pre>6 9 1 4 5 11 12 2 7 10 3 8
</pre>

<p>�ڽ��ж����$3$�ν�������֮��СH�õ������յ��������Ϊ��</p>
<pre>12 9 1 7 5 11 6 2 4 10 3 8
</pre>

<p>���������п��Եõ���������̣�</p>
<div class="row">
<div class="col-sm-offset-4 col-sm-4">
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><tbody><tr><td style="width:40px;">12</td><td style="width:40px;">9</td><td style="width:40px;">1</td><td style="width:40px;">7</td></tr><tr><td>5</td><td>11</td><td>6</td><td>2</td></tr><tr><td>4</td><td>10</td><td>3</td><td>8</td></tr></tbody></table></div>
</div>
</div>

<p>����·�����ξ���������Ϊ</p>
<p>$12\rightarrow 9\rightarrow 1\rightarrow 6\rightarrow 2\rightarrow8$</p>


<pre><code class="language-input2">654321 209 111 23 70000001
10 10 0
</code></pre>


<pre><code class="language-output2">1 3 7 10 14 15 16 21 23 30 44 52 55 70 72 88 94 95 97
</code></pre>



<pre><code class="language-input3">123456 137 701 101 10000007
20 20 0
</code></pre>


<pre><code class="language-output3">1 10 12 14 16 26 32 38 44 46 61 81 84 101 126 128 135 140 152 156 201 206 237 242 243 253 259 269 278 279 291 298 338 345 347 352 354 383 395
</code></pre>

<h2>������</h2>
<p>��������������</p>
<h2>������Լ��</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th><th>$N,M$�Ĺ�ģ</th><th>$Q$�Ĺ�ģ</th><th>Լ��</th></tr></thead><tbody><tr><td>1</td><td>$2 \leq N, M \leq 8$</td><td rowspan="3">$Q = 0$</td><td rowspan="10">$0 \leq a \leq 300$<br>$0 \leq b, c \leq 10^8$<br>$0 \leq x_0 &lt; d \leq 10^8$<br>$1 \leq u_i, v_i \leq N \times M$</td></tr><tr><td>2</td><td rowspan="2">$2 \leq N, M \leq 200$</td></tr><tr><td>3</td></tr><tr><td>4</td><td rowspan="3">$2 \leq N, M \leq 2000$</td><td rowspan="7">$0 \leq Q \leq 50000$</td></tr><tr><td>5</td></tr><tr><td>6</td></tr><tr><td>7</td><td rowspan="4">$2 \leq N, M \leq 5000$</td></tr><tr><td>8</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�</strong>$5\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<p>����Ŀռ�������$256\texttt{MB}$������ر�֤�ύ�Ĵ�������ʱ��ʹ�õ����ڴ�ռ䲻���������ơ�</p>
<p>һ��32λ����������C/C++�е�int��Pascal�е�Longint��Ϊ$4$�ֽڣ��������ڳ���������һ������Ϊ$1024 \times 1024$��32λ���ͱ��������飬����ռ��$4\texttt{MB}$���ڴ�ռ䡣</p>
<h2>����</h2>
<p><a href="./20446/file/attachment.zip">������������</a></p>
