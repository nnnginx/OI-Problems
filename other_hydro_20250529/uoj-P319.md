<p>���ڵ�ac����Ӧ�ÿ��ס�����ӭ���hack<del>����������ڱ�̹��ˡ�����λ���Ը���ṩһ�¿��׵ı��ѽ����</del></p>
<p>"�֣�������" ���� СP</p>
<p>ƽ������ $n$ ��СP�ķ�������һ�����ռ�������Ϊ��������������С͹����Ρ�СP�������ޣ�ÿһʱ�̶��������ɷ�����ʧ��������һʱ��֮ǰ��СP��ʹ��</p>
<p>"�֣�������"</p>
<p>ʹ����Щ��ʧ�ķ������³�����ԭ����λ�á�СP��֪����ÿһʱ�̷�����ʧ��ʣ�µķ���ռ�����������Ƕ��٣�</p>
<h2>�����ʽ</h2>
<p>�ӱ�׼����������ݡ�</p>
<p>�����һ�а������������� $n, m$��������ʼʱ����ĸ���������ʱ������</p>
<p>������ $n$ �У��� $i$ ������������ $x_i, y_i$ �������� $i$ �������λ�á�</p>
<p>������ $m$ �У�ÿ�еĵ�һ������ $k$ ��ʾ��һʱ���� $k$ ��������ʧ���������� $k$ ���Ǹ����� $c_1,c_2,\cdots c_k$������������ʧ�ķ���ı�š�</p>
<p>���ɷ�ʽ���£�</p>
<p>����һ��ʱ���У�����ռ�������<strong>����</strong>Ϊ $S$�����ʱ����ʧ�ķ��� $p_{1}, p_{2}, \dots, p_{k}$ �ı��Ϊ��</p>
<p>$$p_i = [(S + c_i) ~\mathrm{mod}~ n] + 1$$</p>
<p>�ر�ģ��ڵ�һ��ʱ�̣�������Ϊ��һ��ʱ���У� $S=-1$ ��������һ��ʱ����ʧ�ķ��� $p_{1}, p_{2}, \dots, p_{k}$ �ı��Ϊ��</p>
<p>$$p_i = [(-1+c_i) ~\mathrm{mod}~ n] + 1$$</p>
<h2>�����ʽ</h2>
<p>�������׼�����</p>
<p>������ʱ�̵�˳��������� $m$ �У�ÿ��һ����������ʾ��ʱ��ʣ�������ռ�����������<strong>����</strong>��</p>


<pre><code class="language-input1">6 2
-1 0
-1 -1
0 -1
1 0
0 1
0 0
3 1 3 6
2 0 1
</code></pre>




<pre><code class="language-output1">3
2
</code></pre>


<p>����ͼ��ʾ����ͼ��ʾ�����6�������λ�ü�����ռ���������ͼ��ʾ��һ��ʱ�̵����Σ���ʧ�ķ����ŷֱ�Ϊ 1,3,6��ʣ��3����ռ��ͼ��ʵ���ڲ�����ռ�����������Ϊ 3����ͼ��ʾ�ڶ���ʱ�̵����Σ���ʧ�ķ����ŷֱ�Ϊ 
$$[(0+3) ~\mathrm{mod}~ 6] + 1 = 4$$ 
$$[(1+3) ~\mathrm{mod}~ 6] + 1 = 5$$ </p>
<p>ʣ���4����ռ��ͼ��ʵ���ڲ�����</p>
<p> <img class="img-responsive center-block" src="//img.uoj.ac/problem/319/example.png" alt="��������"></p>
<h2>������</h2>
<p>���������������ء�</p>
<h2>������</h2>
<p>���������������ء�</p>
<h2>������</h2>
<p>���������������ء� </p>
<h2>������Լ��</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th rowspan="1">���Ե���</th><th rowspan="1">$n$</th><th rowspan="1">$m$</th><th rowspan="1">$k$</th></tr></thead><tbody><tr><td rowspan="1">1</td><td rowspan="1">10</td><td rowspan="1">10</td><td rowspan="4">$\leq n - 3$</td></tr><tr><td rowspan="1">2</td><td rowspan="3">1000</td><td rowspan="3">1000</td></tr><tr><td rowspan="1">3</td></tr><tr><td rowspan="1">4</td></tr><tr><td rowspan="1">5</td><td rowspan="16">100000</td><td rowspan="16">100000</td><td rowspan="4">$=1$</td></tr><tr><td rowspan="1">6</td></tr><tr><td rowspan="1">7</td></tr><tr><td rowspan="1">8</td></tr><tr><td rowspan="1">9</td><td rowspan="2">$=2$</td></tr><tr><td rowspan="1">10</td></tr><tr><td rowspan="1">11</td><td rowspan="1">$\leq 3$</td></tr><tr><td rowspan="1">12</td><td rowspan="1">$\leq 5$</td></tr><tr><td rowspan="1">13</td><td rowspan="1">$\leq 9$</td></tr><tr><td rowspan="1">14</td><td rowspan="1">$\leq 12$</td></tr><tr><td rowspan="1">15</td><td rowspan="1">$\leq 20$</td></tr><tr><td rowspan="1">16</td><td rowspan="5">$\leq 100$</td></tr><tr><td rowspan="1">17</td></tr><tr><td rowspan="1">18</td></tr><tr><td rowspan="1">19</td></tr><tr><td rowspan="1">20</td></tr></tbody></table></div>

<p>�����������ݣ���֤��</p>
<ul><li>$|x_i|, |y_i|\leq 10^{8}$��</li>
<li>û�������������������ȫ��ͬ�ģ�</li>
<li>$k \leq 100$��</li>
<li>����ʱ�̵� $k$ ֮�Ͳ����� $2 \times 10^{6}$��</li>
<li>$0 \leq c_i \leq 2^{31}-1$��</li>
<li>��ʼʱ�����е� $n$ ������ռ������������� $0$��</li>
<li>�������� $n$ ��������ռ�������<strong>���㼯��</strong>Ϊ $S$�� $|S|\geq 3$��������ʱ�̣�$S$ �����ٴ�������δ��ʧ�ķ��� </li>
</ul><p><strong>ʱ�����ƣ�</strong>$3\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20746/file/attachment.zip">������������</a></p>
