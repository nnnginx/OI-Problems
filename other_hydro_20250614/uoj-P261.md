<p>СCͬѧ��Ϊ�ܲ��ǳ���Ȥ�����Ǿ�������һ����������찮�ܲ�������Ϸ�������찮�ܲ�����һ����������Ϸ����Ҫ���ÿ�찴ʱ���ߣ���ɴ�����</p>
<p>�����Ϸ�ĵ�ͼ���Կ���һ�ð��� $n$ ������ $n-1$ ���ߵ�����ÿ��������������㣬����������������һ��·������ɴ���Ͻ����Ϊ�� $1$ �� $n$ ��������������</p>
<p>������ $m$ ����ң��� $i$ ����ҵ����Ϊ $S_i$���յ�Ϊ $T_i$��ÿ�������ʼʱ���������<strong>�ڵ� $0$ ��</strong>ͬʱ��<strong>�Լ������</strong>��������<strong>ÿ����һ����</strong>���ٶȣ�����ϵ��������·������<strong>�Լ����յ�</strong>��ȥ���ܵ��յ�����Ҿ�������˴����񡣣����ڵ�ͼ��һ����������ÿ���˵�·����Ψһ�ģ�</p>
<p>СC��֪����Ϸ�Ļ�Ծ�ȣ�������ÿ������϶�������һ���۲�Ա���ڽ�� $j$ �Ĺ۲�Ա��ѡ���ڵ� $W_j$ ��۲���ң�һ������ܱ�����۲�Ա�۲쵽���ҽ���������ڵ� $W_j$ ��Ҳ<strong>����</strong>�����˽�� $j$��СC��֪��ÿ���۲�Ա��۲쵽�����ˣ�</p>
<p><strong>ע�⣺</strong>������Ϊһ����ҵ����Լ����յ�����Ҿͻ������Ϸ�������ܵȴ�һ��ʱ����ٱ��۲�Ա�۲쵽�������ڰѽ�� $j$ ��Ϊ�յ����ң������ڵ� $W_j$ ��<strong>ǰ</strong>�����յ㣬���ڽ�� $j$ �Ĺ۲�Ա<strong>���ܹ۲쵽</strong>����ң�����<strong>����</strong>�ڵ� $W_j$ �뵽���յ㣬���ڽ�� $j$ �Ĺ۲�Ա<strong>���Թ۲쵽</strong>�����ҡ�</p>
<h2>�����ʽ</h2>
<p>�ӱ�׼����������ݡ�</p>
<p>��һ������������ $n$ �� $m$������ $n$ �������Ľ��������ͬʱҲ�ǹ۲�Ա��������$m$ ������ҵ�������</p>
<p>������ $n-1$ ��ÿ���������� $u$ �� $v$����ʾ��� $u$ ����� $v$ ��һ���ߡ�</p>
<p>������һ�� $n$ �����������е� $j$ ������Ϊ $W_j$����ʾ��� $j$ ���ֹ۲�Ա��ʱ�䡣</p>
<p>������ $m$ �У�ÿ���������� $S_i$ �� $T_i$����ʾһ����ҵ������յ㡣</p>
<p>�������е����ݣ���֤ $1 \leq S_i, T_i \leq n$��$0 \leq W_j \leq n$��</p>
<h2>�����ʽ</h2>
<p>�������׼�����</p>
<p>��� $1$ �� $n$ ���������� $j$ ��������ʾ��� $j$ �Ĺ۲�Ա���Թ۲쵽�����ˡ�</p>


<pre><code class="language-input1">6 3
2 3
1 2
1 4
4 5
4 6
0 2 5 1 2 3
1 5
1 3
2 6
</code></pre>



<pre><code class="language-output1">2 0 0 1 1 1
</code></pre>


<p>���� $1$ �ŵ㣬$W_1=0$����ֻ�����Ϊ $1$ �ŵ����ҲŻᱻ�۲쵽��������� $1$ ����� $2$ ���۲쵽���� $2$ �˱��۲쵽��</p>
<p>���� $2$ �ŵ㣬û������ڵ� $2$ ��ʱ�ڴ˽�㣬�� $0$ �˱��۲쵽��</p>
<p>���� $3$ �ŵ㣬û������ڵ� $5$ ��ʱ�ڴ˽�㣬�� $0$ �˱��۲쵽��</p>
<p>���� $4$ �ŵ㣬��� $1$ ���۲쵽���� $1$ �˱��۲쵽��</p>
<p>���� $5$ �ŵ㣬��� $1$ ���۲쵽���� $1$ �˱��۲쵽��</p>
<p>���� $6$ �ŵ㣬��� $3$ ���۲쵽���� $1$ �˱��۲쵽��</p>


<pre><code class="language-input2">5 3
1 2
2 3
2 4
1 5
0 1 0 3 0
3 1
1 4
5 5
</code></pre>


<pre><code class="language-output2">1 2 1 0 1
</code></pre>

<h2>������Լ��</h2>
<p>ÿ�����Ե�����ݹ�ģ���ص����±���ʾ����ʾ�����ݷ�Χ�ĸ�λ�ϵ����ֿ��԰����ж�����һ���������͡�</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th rowspan="1">���Ե���</th><th rowspan="1">$n$</th><th rowspan="1">$m$</th><th rowspan="1">Լ��</th></tr></thead><tbody><tr><td rowspan="1">1</td><td rowspan="2">$=991$</td><td rowspan="2">$=991$</td><td rowspan="2">�����˵��������Լ����յ㣬�� $S_i = T_i$</td></tr><tr><td rowspan="1">2</td></tr><tr><td rowspan="1">3</td><td rowspan="2">$=992$</td><td rowspan="2">$=992$</td><td rowspan="2">$W_j=0$</td></tr><tr><td rowspan="1">4</td></tr><tr><td rowspan="1">5</td><td rowspan="1">$=993$</td><td rowspan="1">$=993$</td><td rowspan="1">��</td></tr><tr><td rowspan="1">6</td><td rowspan="3">$=99994$</td><td rowspan="3">$=99994$</td><td rowspan="3">���˻���һ���������� $1$ �� $2$ �бߣ�$2$ �� $3$ �бߣ�$\dots$��$n-1$ �� $n$ �б�</td></tr><tr><td rowspan="1">7</td></tr><tr><td rowspan="1">8</td></tr><tr><td rowspan="1">9</td><td rowspan="4">$=99995$</td><td rowspan="4">$=99995$</td><td rowspan="4">���е� $S_i=1$</td></tr><tr><td rowspan="1">10</td></tr><tr><td rowspan="1">11</td></tr><tr><td rowspan="1">12</td></tr><tr><td rowspan="1">13</td><td rowspan="4">$=99996$</td><td rowspan="4">$=99996$</td><td rowspan="4">���е� $T_i=1$</td></tr><tr><td rowspan="1">14</td></tr><tr><td rowspan="1">15</td></tr><tr><td rowspan="1">16</td></tr><tr><td rowspan="1">17</td><td rowspan="3">$=99997$</td><td rowspan="3">$=99997$</td><td rowspan="4">��</td></tr><tr><td rowspan="1">18</td></tr><tr><td rowspan="1">19</td></tr><tr><td rowspan="1">20</td><td rowspan="1">$=299998$</td><td rowspan="1">$=299998$</td></tr></tbody></table></div>


<p><strong>ʱ�����ƣ�</strong>$2\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20690/file/attachment.zip">������������</a></p>
