<p>����OS ������������з��Ĺ���ǿ��Ĳ���ϵͳ��</p>
<p>����OS���ļ�ϵͳ����ͨ���ļ�ϵͳ���ƣ��Ǹ��ļ������ļ��еĽṹ���ļ�ϵͳ��Ŀ¼��Ϊ��$\texttt{/}$�������ǿ������ļ�·���������ļ����ڵ�λ�ã����硰$\texttt{/flea/uoj}$����ʾ��Ŀ¼�µ�$\texttt{flea}$�ļ����µ�$\texttt{uoj}$�ļ���</p>
<p>����OS���ļ�ϵͳ�С���ݷ�ʽ��һ��������ļ��У��㿪�ÿ�ݷ�ʽ�൱�ڴ򿪸ÿ�ݷ�ʽָ����ļ��С�</p>
<p>���磬�����һ����ݷ�ʽ ��$\texttt{/etc/abc}$�����ÿ�ݷ�ʽָ�� ��$\texttt{/flea/def}$������ļ��У���ôһ�����ʡ�$\texttt{/etc/abc}$�����൱�ڷ��ʡ�$\texttt{/flea/def}$����</p>
<p>��һ�죬�����������ʹ������OS����ʼʱ�ļ�ϵͳΪ�գ�ֻ�и�Ŀ¼����ÿ�λ�������²�����</p>
<ol><li>���ȣ����д�������ļ�·�� $s$ �� $t$��</li>
<li>���ţ����λ�� $t$ ���������ļ������ڸô�����һ�����ļ��С�</li>
<li>����������<strong>��֤ $s$ ���λ��û���ļ�</strong>�������� $s$ ������һ����ݷ�ʽָ�� $t$����� $t$ �Ǹ���ݷ�ʽ����ô $s$ ��ָ�� $t$ ��ָ����ļ��С�</li>
</ol><p>������˵�ġ��������ڸ���Ŀ¼�����ڵ�ʱ��Ҫһ�������丸��Ŀ¼�����磬�����ļ�ϵͳ��ֻ�� ��$\texttt{/v}$�� ����ļ��У���ô�����Ҵ��� ��$\texttt{/v/flea/king/qaq}$�� �ͻ����ļ�ϵͳ�����������ļ��У���$\texttt{/v/flea}$��, ��$\texttt{/v/flea/king}$��, ��$\texttt{/v/flea/king/qaq}$����</p>
<p>������������� $n$ �������Ĳ����󣬿�ʼ�������������ַ��أ������������ $p$ ���·��������һ���ļ��У�����Ѵ����򲻴���������ô����ļ��е���ʵ·����ʲô��</p>
<p>���Ƿ���ֻ�����������ˣ������һ�����ɣ�<strong>�������������������������⡣</strong></p>
<h2>�����ʽ</h2>
<p>��һ������������$n, m$����ʾ�������������$n$������������$m$�����⡣</p>
<p>������$n$��ÿ�������ÿո�������ַ���$s, t$����ʾ���������һ�β�����</p>
<p>������ $m$ ��ÿ��һ���ַ��� $p$ ��ʾ���������һ��ѯ�ʡ�</p>
<p>��֤���е� $s, t, p$ ���ǺϷ����ļ�·���������ļ�����һ������СдӢ����ĸ��ɵķǿ��ַ�����·����һ�����硰$\texttt{/xxx/xxx/xxx/.../xxx}$�������ӡ���֤��·����Ϊ��Ŀ¼��$\texttt{/}$��ʱ��·�����ԡ�$\texttt{/}$����β��</p>
<h2>�����ʽ</h2>
<p>�������������ÿ��ѯ�������ʵ·����</p>


<pre><code class="language-input1">6 5
/root /
/duliu /picks
/vfk /vfleaking
/orz/orz/orz /duliu
/otl /duliu/duliu
/vfk/sb /vfleaking
/vfk/sb/nothing/nothing
/orz
/orz/orz/orz
/qaq
/otl
</code></pre>


<pre><code class="language-output1">/vfleaking/nothing/nothing
/orz
/picks
/qaq
/picks/duliu
</code></pre>


<p>�����Ŀ�ݷ�ʽ�ֱ�Ϊ��</p>
<ul><li>$\texttt{/root} \rightarrow \texttt{/}$</li>
<li>$\texttt{/duliu} \rightarrow \texttt{/picks}$</li>
<li>$\texttt{/vfk} \rightarrow \texttt{/vfleaking}$</li>
<li>$\texttt{/orz/orz/orz} \rightarrow \texttt{/picks}$</li>
<li>$\texttt{/otl} \rightarrow \texttt{/picks/duliu}$</li>
<li>$\texttt{/vfleaking/sb} \rightarrow \texttt{/vfleaking}$</li>
</ul>

<pre><code class="language-input2">2 3
/ba/la /
/w/o/w /w
/ba/la/ba/la/ba/la/ba/la/ba/la/ba/la/ba/la
/ba/la/ba/la/ba/la/ba/la/ba/la/ba/la/ba/la/ba
/w/o/w/o/w/o/w/o
</code></pre>


<pre><code class="language-output2">/
/ba
/w/o
</code></pre>

<h2>������</h2>
<p>��������������</p>
<h2>������Լ��</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th>
<th>$n$</th>
<th>$m$</th>
<th>����</th>
</tr></thead><tbody><tr><td>1</td><td rowspan="3">$\leq 200$</td><td rowspan="10">$\leq 10$</td><td rowspan="3">��֤�����ַ������Ȳ��ᳬ�� $40$</td></tr><tr><td>2</td></tr><tr><td>3</td></tr><tr><td>4</td><td rowspan="3">$\leq 20000$</td><td rowspan="3">��֤ÿ�������·���ַ����н�����һ����$\texttt{/}$����λ���ַ�����ͷ��<br> ��֤�����ַ������Ȳ�����$15$��</td></tr><tr><td>5</td></tr><tr><td>6</td></tr><tr><td>7</td><td rowspan="4">$\leq 20000$</td><td rowspan="4"></td></tr><tr><td>8</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p>�����������ݣ�������·���ַ����ܳ��Ȳ��ᳬ�� $5 \times 10^5$��</p>
<p><strong>ʱ�����ƣ�</strong>$1 \texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256 \texttt{MB}$</p>
<p><br></p>
<p>Ϊ�˷�ֹ��Щͬѧ�����ˣ��һ��������¼��䡣�����·�������ǷǷ��ģ�</p>
<ul><li>$\texttt{/orz/}$</li>
<li>$\texttt{/orz//otl}$</li>
<li>$\texttt{/233}$ ��ע�⣬ֻ�ܺ���СдӢ����ĸ��</li>
</ul><p>�����·�������ǺϷ��ģ�</p>
<ul><li>$\texttt{/}$</li>
<li>$\texttt{/orz/otl/oorrzz/oottll}$</li>
<li>$\texttt{/a}$</li>
</ul><h2>����</h2>
<p><a href="./20453/file/attachment.zip">������������</a></p>
