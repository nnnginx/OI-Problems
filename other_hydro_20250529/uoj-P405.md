<p>������һ��������Ϸ����Ϸ�������� $ 4 $ ��������<code>A</code>��<code>B</code>��<code>X</code> �� <code>Y</code>������Ϸ�У�������϶�����׬��ҡ���������ΰ���Щ���������һ����϶�����</p>
<p>�����Ϸ��һ�����صİ������У����Ա�ʾΪ���� $ 4 $ ���ַ���ɵĴ� $ S $���㲢��֪������� $ S $��������֪�����ĳ���Ϊ $ N $��</p>
<p><strong>�㻹֪����$S$ �����ַ������ڴ����ظ����֡�</strong>���磬$S$ �����ǡ�<code>ABXYY</code>�����ߡ�<code>XYYAA</code>�����������ǡ�<code>AAAAA</code>����<code>BXYBX</code>����</p>
<p>��������ΰ���� $ 4N $ �����������һ����϶������� $ p $ Ϊ�������İ������С����������϶���׬���Ľ������������ͬʱΪ $ p $ ֮�Ӵ��� $ S $ ֮ǰ׺����ַ����ĳ��ȡ��� $ t $ ���Ӵ�����Ϊ $ t $ �е������ַ����У�����Ϊ�գ���$ t $ ��ǰ׺����Ϊ $ t $ ���Ӵ��������Ϊ�գ����߰��� $ t $ �����ַ���</p>
<p>���磬��� $S$ �ǡ�<code>ABXYY</code>������ $ p $ �ǡ�<code>XXYYABYABXAY</code>�������õ� $ 3 $ ����ң���Ϊ��<code>ABX</code>���ǿ���Ϊ $ p $ ���Ӵ��� $ S $ ��ǰ׺����ġ�</p>
<p>��������ǣ�����������϶������ҳ������ַ��� $ S $��</p>
<h2>ʵ��ϸ��</h2>
<p>����Ҫʵ������ĺ�����</p>
<pre><code class="sh_cpp">std::string guess_sequence(int N)</code></pre>
<ul><li><code>N</code>���� $S$ �ĳ��ȡ�</li>
<li>��ÿ�������������ú���������ǡ��һ�Ρ�</li>
<li>�ú���Ӧ���ش� $S$��</li>
</ul><p>��ĳ�����Ե�������ĺ�����</p>
<pre><code class="sh_cpp">int press(std::string p)</code></pre>
<ul><li><code>p</code>����İ������С�</li>
<li><code>p</code> �����ǳ���Ϊ�� $0$ �� $4N$ �Ĵ������� $0$ �� $4N$����<code>p</code> ��ÿ���ַ������� <code>A</code>��<code>B</code>��<code>X</code> ���� <code>Y</code>��</li>
<li>��ÿ����������������øú����Ĵ������ܳ��� $8\ 000$ �Ρ�</li>
<li>�ú����ķ��ؽ���ǣ��������������� <code>p</code> ����׬���Ľ��������</li>
</ul><p>����������������������ĳ��򽫱���Ϊ <code>Wrong  Answer</code>��������ĳ��򽫱���Ϊ <code>Accepted</code>������ĵ÷ֽ����� <code>press</code> �ĵ��ô��������㣨�μ������񣩡�</p>
<h2>����</h2>
<p>�� $S$ Ϊ��<code>ABXYY</code>���������������� <code>guess_sequence(5)</code>�����ݽ������̵�����������ʾ��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>����</th>
<th>����ֵ</th>
</tr></thead><tbody><tr><td> $ \texttt{press("XXYYABYABXAY")} $ </td><td> $ 3 $ </td></tr><tr><td> $ \texttt{press("ABXYY")} $ </td><td> $ 5 $ </td></tr><tr><td> $ \texttt{press("ABXYYABXYY")} $ </td><td> $ 5 $ </td></tr><tr><td> $ \texttt{press("")} $ </td><td> $ 0 $ </td></tr><tr><td> $ \texttt{press("X")} $ </td><td> $ 0 $ </td></tr><tr><td> $ \texttt{press("BXYY")} $ </td><td> $ 0 $ </td></tr><tr><td> $ \texttt{press("YYXBA")} $ </td><td> $ 1 $ </td></tr><tr><td> $ \texttt{press("AY")} $ </td><td> $ 1 $ </td></tr></tbody></table></div>

<p>���� <code>press</code> �ĵ� $1$ �ε��ã���<code>ABX</code>���ǡ�<code>XXYYABYABXAY</code>�����Ӵ�������<code>ABXY</code>�����ǣ���˷��� $3$��</p>
<p>���� <code>press</code> �ĵ� $3$ �ε��ã���<code>ABXYY</code>�������ǡ�<code>ABXYYABXYY</code>�����Ӵ�����˷��� $5$��</p>
<p>���� <code>press</code> �ĵ� $6$ �ε��ã����˿մ�����û�С�<code>ABXYY</code>��������ǰ׺�����ǡ�<code>BXYY</code>�����Ӵ�����˷��� $0$��</p>
<p>���<code>guess_sequence(5)</code> Ӧ�����ء�<code>ABXYY</code>����</p>
<p>���������������е��ļ�<code>ex_combo1.in</code>��Ӧ�ڱ�����ע�⣺�������е����û���κ����塣</p>
<h2>��������</h2>
<ul><li>$1\le N\le 2\ 000$</li>
<li>�� $S$ ��ÿ���ַ������� <code>A</code>��<code>B</code>��<code>X</code> �� <code>Y</code>��</li>
<li>$S$ �����ַ������� $S$ ���ظ����֡�</li>
</ul><p>�ڱ����У��������<strong>����</strong>��Ӧ�Եġ���˼��˵�����������ʼ���е�ʱ�� $S$ �͹̶����������Ҳ���������ĳ���������ѯ�ʡ�</p>
<h2>������</h2>
<ol><li>��5�֣�$N=3$</li>
<li>��95�֣�û�и������ơ��Ը�����������ÿ�����������ϵĵ÷ֽ��������¡��� $q$ Ϊ���� <code>press</code> �Ĵ�����<ul><li>��� $q\le N+2$ ����ĵ÷�Ϊ $95$��</li>
<li>��� $N+2 \lt q \le N+10$����ĵ÷�Ϊ $95-3(q-N-2)$��</li>
<li>��� $N+10\lt q \le 2N+1$����ĵ÷�Ϊ $25$��</li>
<li>��� $\max\{N+10,2N+1\}\lt q \le 4N$����ĵ÷�Ϊ $5$��</li>
<li>������ĵ÷�Ϊ $0$��</li>
</ul></li>
</ol><p>ע�⣬����ÿ���������ϵĵ÷֣��������ڸ������������в��������ϵ���͵÷֡�</p>
<p><strong>��ע�⣺�ڲ����У������ĳ����ѯ�ʴ������� $ N + 2 $�����õ� $ 0 $ �֡�</strong>��</p>
<h2>�������ʾ��</h2>
<p>�������ʾ������ȡ���¸�ʽ�����룺</p>
<ul><li>�� $1$ �У�$S$</li>
</ul><p>�����ĳ�����Ϊ <code>Accepted</code>������ϵͳʾ������ӡ�� <code>Accepted:  q</code>������ <code>q</code> Ϊ���� <code>press</code> �ĵ��ô�����</p>
<p>�����ĳ�����Ϊ <code>Wrong Answer</code>������ӡ�� <code>Wrong Answer: MSG</code>������ <code>MSG</code> �ĺ������£�</p>
<ul><li><code>invalid press</code>�����뵽 <code>press</code> ��ֵ <code>p</code> ����Ч�ġ�Ҳ����˵��<code>p</code> �ĳ��Ȳ��� $0$ �� $4N$ ֮�䣨�� $0$ �� $4N$�������� <code>p</code> ��ĳЩ�ַ����� <code>A</code>��<code>B</code>��<code>X</code> �� <code>Y</code>��</li>
<li><code>too many moves</code>������ <code>press</code> �ĵ��ô������� $8\ 000$ �Ρ�</li>
<li><code>wrong guess</code>��<code>guess_sequence</code> ���صĲ��� $S$��</li>
</ul><h2>Լ��������</h2>
<p>������֧�ֵĸ��ֱ�����ԣ������г��˶�Ӧ���������͡������������͵�ϸ�ڵȣ��μ�ʵ��ʾ����</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>����</th>
<th>$\texttt{int}$</th>
<th>$\texttt{int64}$</th>
<th>$\texttt{int[]}$</th>
<th>����$a$�ĳ���</th>
<th>$\texttt{string}$</th>
</tr></thead><tbody><tr><td>$\texttt{C++}$</td><td>$\texttt{int}$</td><td>$\texttt{long long}$</td><td>$\texttt{std::vector&lt;int&gt;}$</td><td>$\texttt{a.size()}$</td><td>$\texttt{std::string}$</td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$268\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20810/file/attachment.zip">������������</a></p>
