<p>С R �� $m$��$1 \le m \le 1000$���������˺� $m$ ��ֽ������ $i$��$1 \le i \le m$���������˸���Ե� $i$ ��ֽ�����в���������ÿ��ֽ�������Ƕ��������ҷֳ��� $n$��$1 \le n \le 32$�������ӣ����α��Ϊ $0, 1, \ldots , n - 1$��ÿ�������� $3$ ��״̬��1. ������д������ $0$��2. ������д������ $1$��3. ������һ���ո��ӡ�</p>
<p>������ʱ�̣�������<strong>����</strong>վ��ֽ���ϵ�һ�������С����趨�û�������ֽ���ϵĳ�ʼλ�ú󣬵� $i$ �������˻�����ִ��Ԥ���趨�Ĳ������� $S_i$�������� <code>R</code>��<code>0</code>��<code>1</code>��<code>*</code> �����ַ���ɣ����У�</p>
<ol>
<li><code>R</code> ��ʾ������������һ������ұ�û�и��ӣ�������˻�ԭ�ر�ը��</li>
<li><code>0</code> ��ʾ������������ڸ��ӷǿգ��򽫸ø����ϵ����ָ�Ϊ $0$�������޸ģ�</li>
<li><code>1</code> ��ʾ������������ڸ��ӷǿգ��򽫸ø����ϵ����ָ�Ϊ $1$�������޸ģ�</li>
<li><code>*</code> ��ʾ������������ڸ��ӷǿգ��򽫸����ϵ����� $x$ ��Ϊ $1 - x$�������޸ġ�</li>
</ol>
<p>�� $i$ ��ֽ����״̬������һ������Ϊ $n$ �����б�ʾ��ÿ��Ԫ��Ϊ <code>0</code>��<code>1</code> �� <code>-</code>���ո��ӣ������α�ʾ��ÿ�����ӵ�״̬���� $i$ ��ֽ���ĳ�ʼ״̬��Ϊ������ $i$ ������ $X_i$������ִ����ɺ�ֽ����״̬��Ϊ������ $i$ ����� $Y_i$��ע�⣬��������˱�ը�ˣ���ô��������˾�û�������</p>
<p>���Է��֣����һ������Ϊ�գ���ô��������Զ�����޸���������ÿ�������˶����������ԣ������ $i$ �����������ڵ�ֽ���ϵ�<strong>���и���</strong>��Ϊ�գ���ô���Ͳ���ִ���κβ��������������Ϊ���и��Ӷ�Ϊ�ա�</p>
<p>����С R ������ÿһ�������˵����� $X_i$����ÿ��ֽ���ĳ�ʼ״̬���Լ�Ŀ����� $Y_i$��С R ϣ��С D �ҵ�һ��λ�� $p$��$0 \le p &lt; n$����ʹ��<strong>���л�����</strong>������������ֽ���ĵ� $p$ ������Ϊ��ʼλ�ã��ڲ���ը�������ִ�������в�������������� $i$ �������˵����Ϊ $Y_i$��</p>
<p>С D ���˼������������⣬��������֪�����ж��ٸ�������������Ϸ�ʽʹ�����������н⣬���ж�����Ϊÿ���������趨���� $X_0, X_1, \ldots , X_{m - 1}$ ��Ŀ����� $Y_0, Y_1, \ldots , Y_{m - 1}$ �ķ�ʽ��ʹ�����ٴ���һ��λ�� $p$��$0 \le p &lt; n$����ʹ�����л����˶�����������ֽ���ĵ� $p$ ������Ϊ��㣬�ڲ���ը�������ִ�������в������������ $i$ �������˵����Ϊ $Y_i$���������С D ���������⣬�������յĴ𰸿��ܴܺ���������𰸶� ${10}^9 + 7$ ȡģ���������</p>
<p>������Ϸ�ʽ��ͬ���ҽ�������������һ�������ˣ������������Ŀ�������������ʽ�в�ͬ��</p>
<h2>�����ʽ</h2>
<p>��һ�а������������� $n, m$���ֱ��ʾÿ��ֽ���ϵĸ�������ֽ��������</p>
<p>������ $m$ �У��� $i$ ������һ�������� <code>R</code> <code>0</code> <code>1</code> <code>*</code> �������ַ����ַ��� $S_i$����ʾ�� $i$ �������˵Ĳ������С�</p>
<h2>�����ʽ</h2>
<p>��һ��һ������������ʾ��ģ ${10}^9 + 7$ ���������</p>


<pre><code class="language-input1">2 1
1R*
</code></pre>


<pre><code class="language-output1">9
</code></pre>


<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">�������</th>
<th style="text-align:center;">���� $X_0$</th>
<th style="text-align:center;">Ŀ����� $Y_0$</th>
<th style="text-align:center;">���г�ʼλ�� $p$</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;"><code>--</code></td>
<td style="text-align:center;"><code>--</code> </td>
<td style="text-align:center;">$0, 1$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;"><code>0-</code></td>
<td style="text-align:center;"><code>1-</code></td>
<td style="text-align:center;">$0$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;"><code>1-</code></td>
<td style="text-align:center;"><code>1-</code> </td>
<td style="text-align:center;">$0$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;"><code>-0</code></td>
<td style="text-align:center;"><code>-1</code></td>
<td style="text-align:center;">$0$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;"><code>-1</code></td>
<td style="text-align:center;"><code>-0</code></td>
<td style="text-align:center;">$0$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;"><code>00</code></td>
<td style="text-align:center;"><code>11</code></td>
<td style="text-align:center;">$0$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;"><code>10</code></td>
<td style="text-align:center;"><code>11</code> </td>
<td style="text-align:center;">$0$</td>
</tr>
<tr>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;"><code>01</code></td>
<td style="text-align:center;"><code>10</code></td>
<td style="text-align:center;">$0$</td>
</tr>
<tr>
<td style="text-align:center;">$9$</td>
<td style="text-align:center;"><code>11</code></td>
<td style="text-align:center;"><code>10</code> </td>
<td style="text-align:center;">$0$</td>
</tr>
</tbody>
</table>
</div>
<p>���� <code>-</code> ��ʾ�ո��ӡ�ע�ⷽ�� $1$ �������������������ո��ӡ�</p>
<p>������ȫΪ��ʱ����ʼλ�ÿ����� $0$ �� $1$����Ϊ�������⣬����ȫΪ��ʱ�����˲���ִ���κβ�����</p>
<p>�����벻ȫΪ��ʱ����ʼλ��ֻ��Ϊ $0$�������ʼλ��Ϊ $1$ ������һ���ᱬը�����Դ�ʱʵ��ִ�еĲ����ǽ���һ������ָ�Ϊ $1$�������ڶ�������� $x$ ��Ϊ $1 - x$��</p>


<pre><code class="language-input2">3 2
1R0
*
</code></pre>


<pre><code class="language-output2">1468
</code></pre>



<pre><code class="language-input2">3 2
1R0
*
</code></pre>


<pre><code class="language-output2">1468
</code></pre>


<p>�������ݳ�ԭ�����������������</p>
<ol>
<li>��ʼλ�� $p = 0$ ����ʹ��ִ�������в�����������������ô��һ�������˵�ֽ�� $0$ �Ÿ���Ҫô����������ǿգ�ҪôĿ������� $1$����������ν���������� $3$ �ַ�����$1$ �Ÿ���Ҫô����������ǿգ�ҪôĿ������� $0$��Ҳ�� $3$ �ַ�����$2$ �Ÿ���Ҫô����������ǿգ�Ҫô�����Ŀ�������ͬ����Ϊû�жԸø���ִ���κβ�������ͬ���� $3$ �ַ������� $27$ �ַ������ڶ��������˵� $0$ �Ÿ���Ҫô����������ǿգ�Ҫô�����Ŀ�������ͬ���� $3$ �ַ�����$1$ �ź� $2$ �Ÿ���Ҳ���� $3$ �ַ������� $27$ �ַ����������ܹ� $27 \times 27 = 729$ �ַ�����</li>
<li>��ʼλ�� $p = 1$ ����ʹ��ִ�������в�����������������ô��һ�������˵�ֽ���������Ӷ��� $3$ �ַ��������� $0$ �Ÿ���Ҫô���������Ϊ�գ�Ҫô��ͬ��$1$ �Ÿ���Ҫô���������Ϊ�գ�ҪôĿ������� $1$��$2$ �Ÿ��ӵ��������Ҫô��Ϊ�գ�Ҫô����� $0$���� $27$ �ַ������ڶ��������˵� $1$ �Ÿ���Ҫô����������ǿգ�Ҫô�����Ŀ�������ͬ���� $3$ �ַ�����$0$ �ź� $2$ �Ÿ���Ҫô���������Ϊ�գ�Ҫô���������ͬ��Ҳ���� $3$ �ַ������� $27$ �ַ������ܹ� $27 \times 27 = 729$ �ַ�����</li>
<li>��ʼλ�� $p = 2$ ����ʹ��ִ�������в�����������������ô��һ�������˵�ֽ�������������ȫΪ�գ�����ը����ֻ�� $1$ �ַ������ڶ����������� $27$ �ַ������ܹ� $27$ �ַ�����</li>
<li>��ʼλ�� $p = 0, 1$ ��������������Ҫ���һ�������˵� $1$ �Ÿ������������Ϊ�գ�$0$ �Ÿ��ӵ����������Ϊ�ջ�Ϊ $1$��$2$ �Ÿ��ӵ����������Ϊ�ջ�Ϊ $0$�����Ե�һ�������˵�ֽ���� $4$ �ַ������ڶ��������� $0$ �Ÿ��Ӻ� $1$ �Ÿ��Ӷ�Ϊ�գ�$2$ �Ÿ����� $3$ �ַ������ڶ��������˵� $0$ �ź� $1$ �Ÿ��ӱ��붼Ϊ�գ�$2$ �Ÿ���Ҫô���������Ϊ�գ�Ҫô����������ͬ���� $3$ �ַ������ܹ� $12$ �ַ�����</li>
<li>��ʼλ�� $p = 0, 2$ ��������������ô��һ�������˵�ֽ�������������ȫΪ�գ�����ը����ֻ�� $1$ �ַ������ڶ��������� $0$ �ź� $2$ �Ÿ��Ӷ�Ϊ�գ�$1$ �Ÿ����� $3$ �ַ������ܹ� $3$ �ַ�����</li>
<li>��ʼλ�� $p = 1, 2$ ��������������ô��һ�������˵�ֽ�������������ȫΪ�գ�ֻ�� $1$ �ַ������ڶ��������� $1$ �ź� $2$ �Ÿ��Ӷ�Ϊ�գ�$0$ �Ÿ����� $3$ �ַ������ܹ� $3$ �ַ�����</li>
<li>��ʼλ�� $p = 0, 1, 2$ ��������������ô���������˵�����������붼Ϊ�գ��ܹ� $1$ �ַ�����</li>
</ol>
<p>�����ݳ�ԭ�����Ĵ�Ϊ $729 + 729 + 27 - 12 - 3 - 3 + 1 = 1468$��</p>
<h2>��������������</h2>
<p>�������������ء�</p>
<h2>���ݷ�Χ</h2>
<p>�������в��Ե㣺$1 \le n \le 32$��$1 \le m \le 1000$��$1 \le \lvert S_i \rvert \le 100$��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">���Ե���</th>
<th style="text-align:center;">$n \le$</th>
<th style="text-align:center;">$m \le$</th>
<th style="text-align:center;">��������</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 2$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">��</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">��</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$16$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">��</td>
</tr>
<tr>
<td style="text-align:center;">$5 \sim 6$</td>
<td style="text-align:center;">$32$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">��</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">$16$</td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">��</td>
</tr>
<tr>
<td style="text-align:center;">$8 \sim 10$</td>
<td style="text-align:center;">$32$</td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">��</td>
</tr>
<tr>
<td style="text-align:center;">$11 \sim 12$</td>
<td style="text-align:center;">$16$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">��</td>
</tr>
<tr>
<td style="text-align:center;">$13 \sim 15$</td>
<td style="text-align:center;">$32$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">A</td>
</tr>
<tr>
<td style="text-align:center;">$16 \sim 21$</td>
<td style="text-align:center;">$32$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">B</td>
</tr>
<tr>
<td style="text-align:center;">$22 \sim 25$</td>
<td style="text-align:center;">$32$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">��</td>
</tr>
</tbody>
</table>
</div>
<p>�������� A�����������в����� <code>R</code>��</p>
<p>�������� B��ÿ�����������У�<code>R</code> ���������� $15$ ���� </p>
<p><strong>ʱ�����ƣ�$\texttt{3s}$</strong></p>
<p><strong>�ռ����ƣ�$\texttt{1GB}$</strong></p>
