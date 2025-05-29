<p>�����������������ķ�չ���������������������������������ǳ���Ľ��</p>
<p>������һ��,��������������������չ������ļ������ҵ��Ȼ�����������δ���й�ҵ�������޷���������Ӽ���������Ԫ����������������������һ��������뷨����ÿֻ������Ϊһ������ڵ㣬ÿֻ����ֻ���һ���ض���С����</p>
<p>����������� $n$ ֻ����������һƬ��Ұ�ϣ���������Ϊ����ڵ��ڿ�Ұ�����кã������Ϊ $1$ �� $n$��ÿ������ڵ���ĳ������Ҳ�п����� $0$ ��������ڵ�Ľ����Ϊ���룬����õ����������֮�⣬�����������һ�����͵��նˣ����Դ��ն������������ݣ���̨�ն˺����м���ڵ������һ̨�������</p>
<p>�ǵ� $t$ ������ڵ�����Ϊ $x_t$���ýڵ�Ĳ����ɷ�Ϊ���¼������ͣ�</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th>����</th>
<th>�����������ͣ�</th>
<th>������</th>
<th>������</th>
</tr>
</thead>
<tbody>
<tr><td>����ڵ�</td><td><samp>I</samp></td><td>��</td><td>���ն˶���һ��ʵ����Ϊ $x_t$</td></tr>
<tr><td>����ڵ�</td><td><samp>O</samp></td><td>$i$</td><td>$x_t = x_i$������ $x_t$ ������ն�</td></tr>
<tr><td>�ӷ��ڵ�</td><td><samp>+</samp></td><td>$i,j$</td><td>$x_t = x_i + x_j$</td></tr>
<tr><td>ƫ�ƽڵ�</td><td><samp>C</samp></td><td>$i,c$</td><td>$x_t = x_i + c$</td></tr>
<tr><td>ȡ���ڵ�</td><td><samp>-</samp></td><td>$i$</td><td>$x_t = -x_i$</td></tr>
<tr><td>���ƽڵ�</td><td><samp>&lt;</samp></td><td>$i,k$</td><td>$x_t = x_i \cdot 2^k$</td></tr>
<tr><td>���ƽڵ�</td><td><samp>&gt;</samp></td><td>$i,k$</td><td>$x_t = x_i / 2^k$</td></tr>
<tr><td>S�ͽڵ�</td><td><samp>S</samp></td><td>$i$</td><td>$x_t = s(x_i)$</td></tr>
<tr><td>�ȽϽڵ�</td><td><samp>P</samp></td><td>$i,j$</td><td>\begin{equation}x_t = \begin{cases}-1 &amp; x_i \lt x_j \\ 0 &amp; x_i = x_j \\ 1 &amp; x_i \gt x_j \end{cases}\end{equation}</td></tr>
<tr><td>Max�ڵ�</td><td><samp>M</samp></td><td>$i,j$</td><td>\begin{equation}x_t = \begin{cases}x_i &amp; x_i \gt x_j \\ x_j &amp; x_i \le x_j \end{cases}\end{equation}</td></tr>
<tr><td>�˷��ڵ�</td><td><samp>*</samp></td><td>$i,j$</td><td>$x_t = x_i \cdot x_j$</td></tr>
</tbody>
</table>
</div>

<p>���У�$s(x)$ �Ķ������£���$e$ Ϊ��Ȼ����,��ֵԼΪ $2.718281828459045\dots$��
\begin{equation}
s(x) = \frac{1}{1 + e^{-x}}
\end{equation}
$s(x)$ �ĺ���ͼ������ͼ��ʾ��</p>
<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/224/w.png" alt="sigmoid"></p>
<p>��������еĲ����� $i, j$ ��ҪС�ڵ�ǰ�ڵ�ı�� $t$�������������������һ�����£�����Ϳ��԰���Ŵ�С�����˳�����λ������Ȼ����������ÿ������ļ��������������޵ģ����ǽ����Ծ�ȷ��ʮ����С����� $90$ λ�������Ĳ��ֽ��ᱻ�������롣ͬ����������еĲ����� $c$ ��С������Ҳ���ܳ��� $90$ λ�����⣬���ƽڵ�����ƽڵ��еĲ����� $k$ �����ǷǸ��������Ҳ��ܳ��� $10000$��</p>
<p>���������кú�Ұ�Ĳ���������������Ĳ���һ����̨��������ɵļ�����ļ�����������������󳼸�������������� $10$ �������������ÿ�������������Ҫ���ն˻�ȡ���룬�����м���㣬��������ڵ㽫����������������˵������:</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th>���</th>
<th>����</th>
<th>��������</th>
<th>���</th>
</tr>
</thead>
<tbody>
<tr><td>1</td><td>$a,b$</td><td><div>$\lvert a \rvert, \lvert b \rvert \le 10^9$</div><div>С�����ֲ����� $9$ λ</div></td><td>$-2a-2b$</td></tr>
<tr><td>2</td><td>$a$</td><td><div>$\lvert a \rvert \le 10^9$</div><div>С�����ֲ����� $9$ λ</div></td><td>$\frac{1}{1+e^{17a}}$</td></tr>
<tr><td>3</td><td>$a$</td><td><div>$\lvert a \rvert \le 10^9$</div><div>С�����ֲ����� $9$ λ</div></td><td>\begin{equation}\begin{cases}-1 &amp; a \lt 0 \\ 0 &amp; a = 0 \\ 1 &amp; a \gt 0\end{cases}\end{equation}</td></tr>
<tr><td>4</td><td>$a$</td><td><div>$\lvert a \rvert \le 10^9$</div><div>С�����ֲ����� $9$ λ</div></td><td>$\lvert a \rvert$���� $a$ �ľ���ֵ</td></tr>
<tr><td>5</td><td>$a_1, \dots, a_{32}$</td><td>$a_1, \dots, a_{32} \in \{0, 1\}$</td><td>�� $a_1, \dots, a_{32}$ �����ҿ���һ����������������λ�����λ���ң������������ֵ</td></tr>
<tr><td>6</td><td>$a$</td><td><div>$0 \le a \lt 2^{32}$</div><div>$a$ Ϊ����</div></td><td>��� $32$ ���������Ӹ�λ����λ��� $a$ �Ķ����Ʊ�ʾ������ $32$ λ���ڸ�λ�� $0$��</td></tr>
<tr><td>7</td><td>$a,b$</td><td><div>$0 \le a, b \lt 2^{32}$</div><div>$a,b$ ��Ϊ����</div></td><td>$a, b$ ��λ���Ľ��</td></tr>
<tr><td>8</td><td>$a$</td><td><div>$\lvert a \rvert \le 10^9$</div><div>С�����ֲ����� $9$ λ</div></td><td>$\frac{a}{10}$</td></tr>
<tr><td>9</td><td>$a_1, \dots, a_{16}$</td><td><div>$\lvert a_1 \rvert, \dots, \lvert a_{16} \rvert \le 10^9$</div><div>С�����ֲ����� $9$ λ</div></td><td>��� $16$ ��ʵ������ʾ $a_1, \dots, a_{16}$ ��С���������Ľ��</td></tr>
<tr><td>10</td><td>$a,b,m$</td><td><div>$0 \le a, b \lt 2^{32}$</div><div>$1 \le m \lt 2^{32}$</div><div>$a,b,m$ ��Ϊ����</div></td><td>$a \cdot b$ ���� $m$ ������</td></tr>
</tbody>
</table>
</div>

<p>������������Լ�û���㹻��������������ļ�������������ҵ������μ� NOI ���㡣�����������ÿ������ڵ�����ͼ����������������󳼸����� $10$ ������������Ҫ��ʹ�õļ���ڵ��������١�</p>
<h2>�����ʽ</h2>
<p>������������ nodes1.in~nodes10.in ���������أ��ֱ��Ӧ $10$ ����������</p>
<p>ÿ���������ݽ�����һ����������ʾ��Ҫ����ļ��������š�</p>
<h2>�����ʽ</h2>
<p>����ļ�Ϊ nodes1.out~nodes10.out���ֱ��Ӧ��Ӧ�������ļ���</p>
<p>����ÿ���������ݣ�����Ҫ������������У��� $i$ �������� $i$ ������ڵ㡣</p>
<p>����ÿ������ڵ�ʱ������һ���ַ���ʾ�ü���ڵ�����ͣ����������ɸ�����˳���ʾ�ü���ڵ�����ò������ַ�������������֮����ÿո������</p>
<p>������������ܳ��� $10^4$ �С�</p>


<pre><code class="language-input1">1
</code></pre>


<pre><code class="language-output1">I
+ 1 1
- 2
I
+ 4 4
- 5
+ 3 6
- 7
- 8
O 9
</code></pre>


<p>���������Ϊ��һ����������һ�����ܵĹ��졣������ $10$ ������ڵ㣬�ɻ�� $3$ �֡�</p>
<h2>�����񼰲��ַ�</h2>
<p>�����ṩ��ʮ�������ļ� nodes1.ans~nodes10.ans���ֱ��Ӧÿ����������</p>
<p>ÿ�������ļ��� 10 �У��� i ��һ�����ֲ��� $w_i$���������彫�����������</p>
<p>�����У�ÿ�����Ե㵥���������֣�ÿ�����Ե� $10$ �֡�</p>
<p>���ѡ�ֵ������ʽ���Ϸ����߲�����������ĿԼ��,��� $0$ �֡�</p>
<p>���򣬰������¹����ж�ѡ�ֵ�����Ƿ���ȷ��</p>
<p>���Ȳ������������������������ݣ������������ݴ����㹹��ļ������</p>
<p>����ڴ���ĳһ����������ʱ���㹹��ļ�����ļ�������У�ĳ������ڵ�ļ������ľ���ֵ���� $10^{1000}$����� $0$ �֣��㹹��ļ����������е�ĳ��ֵ��Ԥ�ڵ����ֵ���� $10^{-9}$������Ϊ����������ȷ���� $0$ �֡�</p>
<p>����������Ϊ��ļ��������ɸ����ļ������񣬲��������¹���÷֡�</p>
<p>����ÿ�����Ե㣬���������� $10$ �����ֲ��� $w_1 , w_2 , w_3 , \dots , w_9 , w_{10}$��</p>
<p>���蹲ʹ���� $n$ ������ڵ�,��ķ����������±������</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th>�÷�</th>
<th>����</th>
<th>�÷�</th>
<th>����</th>
</tr>
</thead>
<tbody>
<tr><td>$10$</td><td>$n \le w_{10}$</td><td>$5$</td><td>$n \le w_5$</td></tr>
<tr><td>$9$</td><td>$n \le w_{9}$</td><td>$4$</td><td>$n \le w_4$</td></tr>
<tr><td>$8$</td><td>$n \le w_{8}$</td><td>$3$</td><td>$n \le w_3$</td></tr>
<tr><td>$7$</td><td>$n \le w_{7}$</td><td>$2$</td><td>$n \le w_2$</td></tr>
<tr><td>$6$</td><td>$n \le w_{6}$</td><td>$1$</td><td>$n \le w_1$</td></tr>
</tbody>
</table>
</div>

<p>�������ϱ��������������� 0 �֣������ϱ��еĶ����������ȡ������ߵġ�</p>
<p>����֮�⣬ʹ�ñȽϽڵ㡢Max �ڵ�ͳ˷��ڵ�Ĵ����Ǽ�Ϊ����ġ���ˣ������ֽڵ�ÿʹ��<strong>һ��</strong>���ͻ����������Ե�ĵ÷��е��� 4 �֡�</p>
<p>ע�������ǰ�ʹ�ýڵ������������۷֣���ʹ�ô����޹ء�������ʹ�ñȽϽڵ㣬ֻ��۳� $4$ �֣�����ͬʱʹ���˱ȽϽڵ�ͳ˷��ڵ㣬��ʹ��ֻʹ����һ�Σ�Ҳ��۳� 8 �֡�</p>
<p>һ�����Ե����౻�۵� $0$ �֣���ʹ���������۳���Ҳ������ָ�����</p>
<h2>��β���������</h2>
<p>���ն������л����������Ŀ¼�£���windows�û���ʹ��cmd�������������������ļ���checker ʲô�Ķ������� nodes ����ļ����£�</p>
<p><code>cd nodes</code></p>
<p>�����ṩchecker��������������������ļ��Ƿ��ǿɽ��ܵġ�ʹ��������ߵķ����ǣ����ն�������</p>
<p><code>./checker_linux64 &lt;case_no&gt;</code></p>
<p>����<code>case_no</code>�ǲ������ݵı�š�����</p>
<p><code>./checker_linux64 3</code></p>
<p>������ nodes3.out �Ƿ���Խ��ܡ���windows�û���ʹ��<code>checker_win32 3</code>����ʲô����windows 64λ�����İɿ�������win32Ӧ�ó���ġ���</p>
<p>��Ȼ�����ж�Ӧ�� linux 32 λ�汾��<code>checker_linux32</code>����� linux �û������޷����г����볢��ִ�� <code>chmod +x checker_linux64</code> �� <code>chmod +x checker_linux32</code> �����ԡ�</p>
<p>��������ϵͳ�밲װ <a href="//nodejs.org/">node.js</a> Ȼ��ʹ�� <code>node checker.js &lt;case_no&gt;</code> ����checker��</p>
<p>���������������checker �����������������ļ��������ԵĽ����</p>
<p>����,�㻹�������ն���ʹ������</p>
<p><code>./checker �Cf &lt;file_name&gt;</code></p>
<p>������ <code>&lt;file_name&gt;</code> ��ʾ�ļ��������ͨ���ն˽��н�����</p>
<p><strong>ע��: checker �����㹹��ļ����ʱ��ʹ�õ����ݸ����ղ���ʱ���ܲ�ͬ��</strong></p>
<h2>����</h2>
<p><a href="./20664/file/attachment.zip">�������ݼ�checker����</a></p>
