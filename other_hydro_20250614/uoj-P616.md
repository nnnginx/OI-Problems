<p>Anna �� Bruno �ǿ���ѧ�ҡ��������ھ� IOI �������ż������ż� A �У�Anna ������һ�����ϻ��������ͼ�����ż� B �У�Bruno ������һ̨��ʵ�Ļ�����</p>
<p>����������� $N$ ��װ�á�װ���ų�һ�����ӵ�һ�������ϡ����������͵�װ�÷ֱ�Ϊ $X$��$Y$ �� $Z$������߿�ʼ��ÿ��װ�õı������Ϊ $0$ �� $N-1$��װ�� $i$ ��$0\leq i\leq N-1$��������Ϊ $S_i$���� $S_i$ Ϊ $X$��$Y$ �� $Z$ ֮һ��</p>
<p>��Ϊ����̫��Bruno ����һ��һ���ӻ������Ƴ�װ�á�Ȼ����Ϊװ��֮�以��ͨ���������ӣ�������ǳ�С���Ƴ�ʱ��˳��</p>
<p>����һ�ִӻ����н�װ���Ƴ��ķ��������������¶��壺</p>
<ul>
<li>����װ�� $x,y,z$ ��$0\leq x\lt y\lt z\leq N-1$����û�б��Ƴ����� $S_x=X$��$S_y=Y$��$S_z=Z$�����⣬�������ÿ�� $x\lt j\lt y$��װ�� $j$ �ѱ��Ƴ����Ҷ���ÿ�� $y\lt k\lt z$��װ�� $k$ Ҳ�ѱ��Ƴ������������Щ���������������ǽ�װ�� $y$ �ӻ������Ƴ�����ô�ⱻ��Ϊһ��<strong>�õ��Ƴ�</strong>��</li>
<li>�κ�������װ�ôӻ������Ƴ��ķ��������Ǻõ��Ƴ���</li>
</ul>
<p>Bruno ��Ҫ������ $N$ ��װ�ôӻ������Ƴ���<strong>�õ��Ƴ�</strong>�Ĵ������Ȼ������Ϊ�������͵�װ�ÿ����������ƣ������ֱܷ�װ�õ����͡�</p>
<p>����Ϊ Anna �л��������ͼ����֪�����ڻ����ϵ�װ�õ����͡����������ͨ�����ߵ緢���������� Bruno��ͨ�����ߵ緢���������ܹ�����һ�����У��������е�ÿ���ַ����� $0$ �� $1$��</p>
<p>дһ��������ʵ�� Anna �Ĺ滮�� Bruno �Ĺ滮ʹ��<strong>�õ��Ƴ�</strong>�Ĵ�������ڸ������� Anna ���͸� Bruno ���ַ�Խ����ĵ÷�Խ�ߡ�</p>
<h2>ʵ��ϸ��</h2>
<p>����Ҫ�ύ�����ļ���</p>
<p>��һ���ļ�Ϊ <code>Anna.cpp</code>����Ҫʵ�� Anna �Ĺ滮������ģ�����Ҫʵ�����º����ҳ�����Ҫʹ�� <code>#include</code> ���� <code>Anna.h</code> ͷ�ļ���</p>
<ul>
<li><code>void Anna(int N, std::vector&lt;char&gt; S)</code> ����ÿ����������������������ڿ�ʼʱ������ǡ��һ�Ρ�<ul>
<li>���� <code>N</code> Ϊװ�õ����� $N$��</li>
<li>���� <code>S</code> Ϊһ�� $N$ �����顣����ζ�� <code>S[i]</code> Ϊװ�� $i$��$0\leq i\leq N-1$�������� $S_i$������ַ� <code>S[i]</code> Ϊ <code>X</code>��<code>Y</code> �� <code>Z</code> ֮һ��</li>
</ul>
</li>
</ul>
<p>��ĳ�����Ե������º�����</p>
<ul>
<li><code>void Send(int a)</code> ʹ�øú�����Anna ������һ���ַ� $0$ �� $1$ �� Bruno��<ul>
<li>���� <code>a</code> Ϊ���� Bruno ����Ϣ����Ӧ��Ϊ $0$ �� $1$��������������������ĳ��򽫻ᱻ�ж�Ϊ <strong>Wrong Answer [1]</strong>��</li>
<li>�ú��� <code>Send</code> ��Ӧ�����ó��� $200000$ �Σ�������ĳ��򽫻ᱻ�ж�Ϊ <strong>Wrong Answer [2]</strong>��</li>
</ul>
</li>
</ul>
<hr>
<p>�ڶ����ļ��� <code>Bruno.cpp</code>����Ҫʵ�� Bruno �Ĺ滮������Ҫ�������º����Ҹó�����Ҫʹ�� <code>#include</code> ���� <code>Bruno.h</code> ͷ�ļ���</p>
<ul>
<li><code>void Bruno(int N, int L, std::vector&lt;int&gt; A)</code> �ں��� <code>Anna</code> �����ú󣬸ú����ᱻ����һ�Ρ�<ul>
<li>���� <code>N</code> Ϊװ�õ����� $N$��</li>
<li>���� <code>L</code> Ϊ Anna ���͵��ַ���$0$ �� $1$����������</li>
<li>���� <code>A</code> Ϊһ�� $L$ �����顣����ζ�� Anna ������һ������ <code>A[0],A[1],...,A[L-1]</code> ��������˳��� Bruno�������е�ÿ���ַ�Ϊ $0$ �� $1$��</li>
</ul>
</li>
</ul>
<p>��ĳ�����Ե������º�����</p>
<ul>
<li><code>void Remove(int d)</code> ��ĳ�����øú������ش�����Ƴ�װ�á�<ul>
<li>���� <code>d</code> Ϊװ�õ���������ζ�� Bruno �Ƴ���װ�� $d$��</li>
<li>�������� $0\leq d\leq N-1$��������ĳ��򽫻ᱻ�ж�Ϊ <strong>Wrong Answer [3]</strong>��</li>
<li>������ʹ����ͬ�Ĳ��� $d$ �����øú�������һ�Σ�������ĳ��򽫻ᱻ�ж�Ϊ <strong>Wrong Answer [4]</strong>��</li>
<li>���� <code>Remove</code> ��Ҫ������ǡ�� $N$ �Ρ������� <code>Bruno</code> ��ֹʱ��������� <code>Remove</code> �Ĵ�����Ϊ $N$ �Σ���ĳ��򽫻ᱻ�ж�Ϊ <strong>Wrong Answer [5]</strong>��</li>
<li>������ $N$ ��װ�ñ��Ƴ��󣬺õ��Ƴ��Ĵ�����ҪΪ���ܵ����ֵ��������ĳ��򽫻ᱻ�ж�Ϊ <strong>Wrong Answer [6]</strong>��</li>
</ul>
</li>
</ul>
<h2>ע������</h2>
<ul>
<li>��ĳ������ʵ�������ĺ������ڲ�ʹ�ã�����ʹ��ȫ�ֱ������ύ���ļ����ᱻ�� grader һ������һ����ִ���ļ�������ȫ�ֱ������ڲ�����Ӧ����һ�������������ռ��������������������ļ��ĳ�ͻ����������Ϊ��������ִ�У��ֱ�Ϊ Anna �� Bruno��Anna �Ľ��̺� Bruno �Ľ��̼��޷�����ȫ�ֱ�����</li>
<li>��ĳ�������ʹ�ñ�׼���������Ҳ�����������ļ�ͨ���κη�ʽ������������ĳ������ͨ����׼����������� debug ��Ϣ��</li>
</ul>
<p>����������������Ҫ��һ�����ӣ�����һ���������� grader �Ĵ浵�ļ���������ĳ��򡣴浵�ļ�Ҳ������һ����ĳ����������</p>
<p>���� grader Ϊ <code>grader.cpp</code> �ļ���Ϊ�˲�����ĳ��򣬽� <code>grader.cpp</code>��<code>Anna.cpp</code>��<code>Bruno.cpp</code>��<code>Anna.h</code>��<code>Bruno.h</code> ����ͬһ��Ŀ¼�²�ʹ�����б�������</p>
<p><code>g++ -std=gnu++17 -O2 -fsigned-char -o grader grader.cpp Anna.cpp Bruno.cpp</code></p>
<p>������ɹ�ʱ�����ɿ�ִ���ļ� <code>grader</code>��</p>
<p>ע��ʵ�ʵ� grader ������ grader ��ͬ������ grader ����ʹ�õ������Ҵӱ�׼����������ݲ������д����׼�����</p>
<p>ʵ�ʲ����У����ĳ���ᱻ�������Σ����ε�ʱ�����ƾ�Ϊ $2$ �롣</p>
<h2>�����ʽ</h2>
<p>���� grader �ӱ�׼��������������ݣ�</p>
<p>$N$</p>
<p>$S_0\space S_1\space \cdots \space S_{N-1}$</p>
<p>���� $S_i$ �� $S_{i+1}$��$0\leq i\leq N-2$��֮��ʹ��һ���ո�ָ���</p>
<h2>�����ʽ</h2>
<p>������ɹ�ֹͣʱ������ grader ���ڱ�׼���д��������Ϣ��</p>
<ul>
<li>�����Ĵ𰸱��ж�Ϊ Wrong Answer [1]��[2]��[3]��[4]��[5] ֮һ��������������� <code>Wrong Answer [1]</code>��</li>
<li>����������� <code>Send</code> ���������õĴ��� $L$ �ͺõ��Ƴ��Ĵ��� $D$ �� <code>Accepted: L D</code>��ע������ grader ��ʵ�� grader ��ͬ������ grader ��������ĳ����Ƿ��ж�Ϊ Wrong Answer [6]��</li>
</ul>
<p>�����ĳ����ж�Ϊ Wrong Answer [1]��[2]��[3]��[4]��[5] ֮�еĶ������ͣ����� grader ��ֻ�ᱨ������һ����</p>
<h2>��������</h2>
<p>������һ����������������� grader ���Ӧ�ĺ������á�</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th>Sample Input 1</th>
<th>Sample Function Calls</th>
<th>Sample Function Calls</th>
</tr>
</thead>
<tbody>
<tr>
<td>$ $</td>
<td>Call</td>
<td>Call</td>
</tr>
<tr>
<td><code>4 X Y X Z</code></td>
<td><code>Anna(4, {X, Y, X, Z})</code></td>
<td>$ $</td>
</tr>
<tr>
<td>$ $</td>
<td>$ $</td>
<td><code>Send(0)</code></td>
</tr>
<tr>
<td>$ $</td>
<td>$ $</td>
<td><code>Send(1)</code></td>
</tr>
<tr>
<td>$ $</td>
<td><code>Bruno(4, 2, {0, 1})</code></td>
<td>$ $</td>
</tr>
<tr>
<td>$ $</td>
<td>$ $</td>
<td><code>Remove(2)</code></td>
</tr>
<tr>
<td>$ $</td>
<td>$ $</td>
<td><code>Remove(1)</code></td>
</tr>
<tr>
<td>$ $</td>
<td>$ $</td>
<td><code>Remove(0)</code></td>
</tr>
<tr>
<td>$ $</td>
<td>$ $</td>
<td><code>Remove(3)</code></td>
</tr>
</tbody>
</table>
</div>
<p>�������ĺ��������У��ĸ�װ�ý��������·�ʽ�Ƴ���</p>
<ol>
<li>�ڿ�ʼʱ���ĸ�װ��Ϊ <code>X Y X Z</code>��</li>
<li>Bruno �Ƴ���װ�� 2��ע������Ϊ���������ǵڶ�������ʣ���װ�ñ�Ϊ <code>X Y - Z</code>������ <code>-</code> ��ζ��ԭ�������λ�õ�װ���ѱ��Ƴ���</li>
<li>Bruno �Ƴ���װ�� 1��ʣ���װ�ñ�Ϊ <code>X - - Z</code>����Ϊ $(x,y,z)=(0,1,3)$ ��������������Ǻõ��Ƴ���</li>
<li>Bruno �Ƴ���װ�� 0��ʣ���װ�ñ�Ϊ <code>- - - Z</code>��</li>
<li>��� Bruno �Ƴ���װ�� 3.ʣ���װ�ñ�Ϊ <code>- - - -</code>��</li>
</ol>
<p>�õ��Ƴ��Ĵ���Ϊһ�Σ�����������У��õ��Ƴ��Ĵ��������ܴ���һ��</p>
<h2>������Լ��</h2>
<ul>
<li>$3\leq N\leq 100000$��</li>
<li><p>$S_i$ Ϊ <code>X</code>��<code>Y</code> �� <code>Z</code> ֮һ��$0\leq i\leq N-1$����</p>
</li>
<li><p>��5 �֣�$N\leq 18$��</p>
</li>
<li>��95 �֣��޶���Լ�����ڸ��������У���ķ�������ʹ�����·�ʽ���㡣<ul>
<li>�� $L$ Ϊ����������ÿ�����������е��� <code>Send</code> �����Ĵ��������ֵ����ķ������������淽�����㣺<ul>
<li>�� $160000\lt L\leq 200000$ ʱ����ķ���Ϊ $\displaystyle 25+\left\lfloor 10\times \frac{200000-L}{40000}\right\rfloor$ �֡�</li>
<li>�� $100000\lt L\leq 160000$ ʱ����ķ���Ϊ $\displaystyle 35+\left\lfloor 30\times \frac{160000-L}{60000}\right\rfloor$ �֡�</li>
<li>�� $70000\lt L\leq 100000$ ʱ����ķ���Ϊ $\displaystyle 65+\left\lfloor 30\times \left(\frac{100000-L}{30000}\right)^2\right\rfloor$ �֡�</li>
<li>�� $L\leq 70000$ ʱ����ķ���Ϊ 95 �֡�</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>���� $\lfloor x\rfloor$ Ϊ������ $x$ �����������</p>
<p><strong>ʱ������</strong>��$2\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$256\texttt{MB}$</p>
