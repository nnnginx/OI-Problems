<p><strong>����һ�������⡣</strong>���������м��ܣ������Ҫ Hack������ϵ immortalCO��</p>
<p>СM����һ����ʱս��(Real Time Strategy)��Ϸ����ͬ�ڴ����ͬ����Ϸ�������Ϸ�ĵ�ͼ�����εġ�Ҳ����˵����ͼ������һ���� $n$ ����㣬$n - 1$ ���߹��ɵ���ͨͼ����ʾ����Щ��㱻���Ϊ $1$ ~ $n$��</p>
<p>ÿ����������ֿ��ܵ�״̬������֪�ġ���δ֪�ġ�����Ϸ��ʼʱ��ֻ�� $1$ �Ž������֪�ġ�����Ϸ�Ĺ����У�СM���Գ���̽������Ľ�㡣������˵��СMÿ�β���ʱ��Ҫѡ��һ����֪�Ľ�� $x$����һ����ͬ�� $x$ �������� $y$����� $y$ ������δ֪�ģ���Ȼ����Ϸ���Զ�Ѱ·ϵͳ����� $x$ �� $y$ �����·���ϵĵڶ������ $z$��Ҳ���Ǵ� $x$ �ߵ� $y$ �����·������ $x$ ���ڵĽ�㡣��ʱ�������� $z$ ��δ֪�ģ�СM�Ὣ�����Ϊ��֪�ġ�</p>
<p>�����Ϸ��Ŀ���ǣ��������� $T$ ��̽�������������н���״̬����Ϊ��֪�ġ�Ȼ��СM���������Ϸ�����֣���ϣ���õ���İ�����</p>
<p><strong>Ϊ������Ϸ���̸������ף�СM�����ṩ�������Ϸ�Ľ����⣬������������������͡�ʵ��ϸ�ڡ���</strong></p>
<p><strong>���⣬СMҲ�ṩ��һЩ��Ϸ����ʾ���������Ŀ�����һ�ڡ���ʾ����</strong></p>
<h2>�������</h2>
<p>����Ҫʵ��һ������ <code>play</code>���԰���СM�����Ϸ��Ŀ�ꡣ</p>
<ul><li><code>play(n, T, dataType)</code><ul><li><code>n</code> Ϊ���Ľ�������</li>
<li><code>T</code> Ϊ̽�������Ĵ������ƣ�</li>
<li><code>dataType</code> Ϊ�ò��Ե���������ͣ�����������ݹ�ģ��Լ������</li>
</ul></li>
</ul><p>��ÿ�����Ե��У������ⶼ�����ǡ��һ�� <code>play</code> �������ú���������֮ǰ����Ϸ���ڸտ�ʼ��״̬��</p>
<p>����Ե��ú��� <code>explore</code> ������������Ϸ��̽�������㣬������������ĵ��ô������ܳ��� $T$ �Ρ�</p>
<ul><li><code>explore(x, y)</code><ul><li><code>x</code> Ϊһ����֪�Ľ�㣻</li>
<li><code>y</code> Ϊһ����ͬ�� $x$ �������㣨���Բ�����֪�Ľ�㣩��</li>
<li>��������᷵�ؽ�� $x$ �� $y$ �����·���ϵĵڶ������ı�š�</li>
</ul></li>
</ul><p>�ں��� <code>play</code> ����֮�󣬽����������Ϸ��״̬��ֻ�е�ÿ����㶼����֪�ģ�������Ϸ��Ŀ����ɡ�</p>
<h2>ʵ�ַ���</h2>
<p>����Ҫ��ֻ���ύһ��Դ�ļ� rts.cpp/c/pas ʵ����������������ѭ����������ͽӿڡ�</p>
<p><strong>�� C/C++ ���Ե�ѡ�֣�</strong></p>
<p>Դ��������Ҫ����ͷ�ļ� rts.h��</p>
<p>����Ҫʵ�ֵĺ��� <code>play</code>��</p>
<pre><code class="sh_c">void play(int n, int T, int dataType);</code></pre>
<p>���� <code>explore</code> �Ľӿ���Ϣ���£�</p>
<pre><code class="sh_c">int explore(int x, int y);</code></pre>
<p><strong>�� Pascal ���Ե�ѡ�֣�</strong></p>
<p>����Ҫʹ�õ�Ԫ graderhelperlib��</p>
<p>����Ҫʵ�ֵĺ��� <code>play</code>��</p>
<pre><code class="sh_pascal">procedure play(n, T, dataType : longint);</code></pre>
<p>���� <code>explore</code> �Ľӿ���Ϣ���£�</p>
<pre><code class="sh_pascal">function explore(x, y : longint) : longint;</code></pre>
<h2>��β�����ĳ���</h2>
<p><strong>�� C/C++ ���Ե�ѡ�֣�</strong></p>
<p>����Ҫ�ڱ���Ŀ¼��ʹ�������������õ���ִ�г���</p>
<p>���� C ���ԣ�</p>
<p><code>gcc grader.c rts.c -o rts -O2</code></p>
<p>���� C++ ���ԣ�</p>
<p><code>g++ grader.cpp rts.cpp -o rts -O2</code></p>
<p><strong>�� Pascal ���Ե�ѡ�֣�</strong></p>
<p>����Ҫ�ڱ���Ŀ¼��ʹ�������������õ���ִ�г���</p>
<p><code>fpc grader.pas -o"rts" -O2</code></p>
<p>��ִ���ļ�����<strong>��׼����</strong>�������¸�ʽ�����ݣ�</p>
<p>��һ�а����������� $n$, $T$, $\texttt{dataType}$����Ҫ��֤ $n$ �� [$2$, $3 \times 10^5$] ֮�䣬$T$ �� [$1$, $5 \times 10^6$] ֮�䣬$\texttt{dataType}$ �� [$1$, $3$] ֮�䡣</p>
<p>������ $n - 1$ �У�ÿ���������� $u$, $v$����Ҫ��֤ $1 \le u, v \le n$ �� $u \ne v$����ʾһ�� $u$ �� $v$ ֮��ıߡ�</p>
<p>���������Ҫ��֤�� $n - 1$ ���߹���һ������</p>
<p>�������֮�󣬽����⽫���� <code>play</code> �����������ʱ����� <code>explore</code> �Ĵ������� $T$ �Σ��򽻻���������ϸ�Ĵ�����Ϣ�����˳���</p>
<p>��������������ж���ϷĿ���Ƿ���ɡ������ɣ������� "Correct"������������Ӧ�Ĵ�����Ϣ��</p>
<p>������� <code>explore</code> �����Ĳ����Ƿ���$x,y$ ���� $1$ �� $n$ �ķ�Χ�ڣ��� $x$ ������֪��㣬�� $x$ ���� $y$������ô������������ϸ�Ĵ�����Ϣ�����˳���</p>
<p>���Ҫʹ���Լ��������ļ����в��ԣ��뱣֤�����ļ��������ϸ�ʽҪ�󣬷��򲻱�֤��������ȷ���С�</p>
<h2>���ʹ������Դ����</h2>
<p>����Ŀ¼�£������ÿ�����Ե�����Դ���� rts_sample.cpp/c/pas��ѡ������������ԣ����临��Ϊ rts.cpp/c/pas�������������ᵽ�ķ�ʽ���б��룬����ͨ������õ���ִ�г��� </p>
<p>���ڷ���ʽѡ�֣���ֻ��ѡ��һ�����Խ������𣬼��㱾�������Ŀ¼�²���ͬʱ���ڶ�����Ե� rts.cpp/c/pas������ϵͳ����ѡһ��Դ����������Ⲣ��Ϊ���ս����</p>
<p>����������Ҫ�޸�����ļ���ʵ�֣��Դﵽ��Ŀ��Ҫ��</p>


<pre><code class="language-input1">4 100 1
1 3
3 4
3 2
</code></pre>



<pre><code class="language-output1">Correct
</code></pre>


<p>����ʹ������Ŀ¼�� grader ����ȷ��Դ����õ�������ļ���</p>
<p>���ڴ�������һ�ֿ��ܵ� <code>explore</code> �����ĵ���˳��Ϊ��</p>
<ul><li><code>explore(1, 2)</code>������ 3</li>
<li><code>explore(3, 2)</code>������ 2</li>
<li><code>explore(2, 4)</code>������ 3</li>
<li><code>explore(3, 4)</code>������ 4</li>
</ul><h2>������</h2>
<p>��<a href="./20775/file/attachment.zip">����Ŀ¼</a>�µ� <em>ex_2.in</em> �� <em>ex_2.ans</em>��</p>
<p>�������������ݷ�Χͬ�� 5 �����Ե㡣</p>
<h2>������</h2>
<p>��<a href="./20775/file/attachment.zip">����Ŀ¼</a>�µ� <em>ex_3.in</em> �� <em>ex_3.ans</em>��</p>
<p>�������������ݷ�Χͬ�� 8 �����Ե㡣</p>
<h2>���ַ�ʽ</h2>
<p>��������ʱֻ����ȡ rts.cpp/c/pas���޸�ѡ��Ŀ¼�е������ļ���������Ч��</p>
<p>��Ŀ���Ȼ��ܵ��ͷǽ���ʽ��������ͬ�����ơ�����������ᵼ��������Ŀ�� 0 �֣�����ʱ���󡢳���ʱ�����ơ������ռ����ƵȻᵼ����Ӧ���Ե�� 0 �ֵȡ� ��ֻ�ܷ����Լ�����ĺͽ���������ı��������Ӧ���ڴ�ռ䣬���Է��������ռ佫���ܵ��±����������д��� </p>
<p>������������������Ὺʼ������ȷ�ԡ�ֻ�е���ϷĿ�����ʱ���ò��Ե�����֣���������ò��Ե�� 0 �֡�</p>
<p>��Ŀ��������ʱ�䡢�ռ�����Ϊ��Ĵ���ͽ��������������ʹ�õ�ʱ��Ϳռ䡣���Ǳ�֤�������κκϷ������ݼ������Ʒ�Χ�ڵĵ��ã��κ������κΰ汾�Ľ����⣨�����·���ѡ�ֵĺ���������ʹ�õģ����������õ�ʱ�䲻�ᳬ�� 1s���������õĿռ䲻�ᳬ�� 64MB��Ҳ����˵��ѡ��ʵ�ʿ��õ�ʱ������Ϊ 2s��ʵ�ʿ��õĿռ�����Ϊ 448MB��</p>
<h2>��ʾ</h2>
<p>������СM�����һЩ���ĵ���ʾ��</p>
<ul><li>ͼ������ͼ���ɽ��ͱ߹��ɣ����ǽ�������ԣ������������֮����໥��ϵ</li>
<li>·����һ�����ķǿ����У�ʹ�������������������֮�䶼�б�����</li>
<li>�����������ͨ�ģ����ҽ�������һ��������һ����㿪ʼ����һ����������·��</li>
<li>һ��ͼ����ͨ�ģ����ҽ������ͼ�ϵ�ÿ�Խ�㶼����ͨ��</li>
<li>һ�� $n$ ������������һ���� $n$ ����㣬$n - 1$ ���߹��ɵ���ͨͼ</li>
<li>�����������·������ָ���������������п��ܵ�·���У����г�����С��</li>
<li>��һ�����У��������������������·��������Ψһ��</li>
<li>ͨ��������������ļ�����������ϵͳ�򹥻������ȷ�ʽ�÷�����������Ϊ�����÷�����Ч��</li>
</ul><h2>������Լ��</h2>
<p>һ���� 20 �����Ե㣬ÿ�����Ե� 5 �֡�</p>
<p>�������в��Ե㣬�Լ���������������$2 \le n \le 3 \times 10^5, 1 \le T \le 5 \times 10^6, 1 \le \texttt{dataType} \le 3$��
��ͬ $\texttt{dataType}$ ��Ӧ�������������£�</p>
<ul><li>���� $\texttt{dataType} = 1$ �Ĳ��Ե㣬û����������</li>
<li>���� $\texttt{dataType} = 2$ �Ĳ��Ե㣬��Ϸ�ĵ�ͼ��һ���Խ�� $1$ Ϊ������ȫ��������
��������һ�� $1$ ~ $n$ ������ $a$������ $a_1 = 1$���ҽ�� $a_i ~ (1 &lt; i \le n)$ ���� $a_{\lfloor i/2 \rfloor}$ ֮����һ��������</li>
<li>���� $\texttt{dataType} = 3$ �Ĳ��Ե㣬��Ϸ�ĵ�ͼ��һ������
��������һ�� $1$ ~ $n$ ������ $a$�������� $a_i ~ (1 &lt; i \le n)$ ���� $a_{i-1}$ ֮����һ��������</li>
</ul><p>����ÿ�����Ե㣬$n, T, \texttt{dataType}$ ��ȡֵ���±�</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th rowspan="1">���Ե���</th><th rowspan="1">$n$</th><th rowspan="1">$T$</th><th rowspan="1">$\texttt{dataType}$</th></tr></thead><tbody><tr><td rowspan="1">1</td><td rowspan="1">2</td><td rowspan="1">10000</td><td rowspan="4">1</td></tr><tr><td rowspan="1">2</td><td rowspan="1">3</td><td rowspan="1">10000</td></tr><tr><td rowspan="1">3</td><td rowspan="1">10</td><td rowspan="1">10000</td></tr><tr><td rowspan="1">4</td><td rowspan="1">100</td><td rowspan="1">10000</td></tr><tr><td rowspan="1">5</td><td rowspan="1">1000</td><td rowspan="1">10000</td><td rowspan="3">2</td></tr><tr><td rowspan="1">6</td><td rowspan="1">20000</td><td rowspan="1">300000</td></tr><tr><td rowspan="1">7</td><td rowspan="1">250000</td><td rowspan="1">5000000</td></tr><tr><td rowspan="1">8</td><td rowspan="1">1000</td><td rowspan="1">20000</td><td rowspan="6">3</td></tr><tr><td rowspan="1">9</td><td rowspan="1">5000</td><td rowspan="1">15500</td></tr><tr><td rowspan="1">10</td><td rowspan="1">30000</td><td rowspan="1">63000</td></tr><tr><td rowspan="1">11</td><td rowspan="1">150000</td><td rowspan="1">165000</td></tr><tr><td rowspan="1">12</td><td rowspan="1">250000</td><td rowspan="1">250100</td></tr><tr><td rowspan="1">13</td><td rowspan="1">300000</td><td rowspan="1">300020</td></tr><tr><td rowspan="1">14</td><td rowspan="1">1000</td><td rowspan="1">50000</td><td rowspan="7">1</td></tr><tr><td rowspan="1">15</td><td rowspan="1">5000</td><td rowspan="1">200000</td></tr><tr><td rowspan="1">16</td><td rowspan="1">30000</td><td rowspan="1">900000</td></tr><tr><td rowspan="1">17</td><td rowspan="1">150000</td><td rowspan="1">3750000</td></tr><tr><td rowspan="1">18</td><td rowspan="1">200000</td><td rowspan="1">4400000</td></tr><tr><td rowspan="1">19</td><td rowspan="1">250000</td><td rowspan="1">5000000</td></tr><tr><td rowspan="1">20</td><td rowspan="1">300000</td><td rowspan="1">5000000</td></tr></tbody></table></div>

<h2>����</h2>
<p><a href="./20775/file/attachment.zip">�����ͽ���������</a></p>
<p><strong>ʱ�����ƣ�</strong><del>2s</del> $3\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$512\texttt{MB}$</p>
