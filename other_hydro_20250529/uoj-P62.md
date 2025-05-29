<div class="hide">
$\newcommand\lcm{\mathbin{\mathrm{lcm}}}$
</div>

<p>����ˮ������ʦ������ʦ���Ҿ����ҹ��������ǲ����ġ������ҳԲ��˿������������󣬵���ȴû�������ܲ����ٶȡ��������������ܵø��죿���Թ��԰ײˣ�û��Ч������</p>
<p>��ʦǳЦ���𣺡������ܼ򵥣����������ҽ��㣬���ȿ������UOJ Round��C�⡣��</p>
<p>�� $p = 998244353$��$7 \times 17 \times 2^{23} + 1$��һ����������</p>
<p>�������� $n, c, d$������������ $x_1, \dots, x_n$ �� $b_1, \dots, b_n$ ���� $0 \leq x_1, \dots, x_n, b_1, \dots, b_n &lt; p$���Ҷ��� $1 \leq i \leq n$ ���㣺</p>
<p>\begin{equation}
\sum_{j = 1}^{n} \gcd(i, j)^c \cdot \lcm(i, j)^d \cdot x_j \equiv b_i \pmod{p}
\end{equation}
���� $v \equiv u \pmod{p}$ ��ʾ $v$ �� $u$ ���� $p$ ��������ȡ�$\gcd(i, j)$ ��ʾ $i$ �� $j$ �����Լ����$\lcm(i, j)$ ��ʾ $i$ �� $j$ ����С��������</p>
<p>�� $q$ ��ѯ�ʣ�ÿ�θ��� $b_1, \dots, b_n$�������� $x_1, \dots, x_n$ ��ֵ��</p>
<h2>�����ʽ</h2>
<p>��һ���ĸ����� $n, c, d, q$����֤ $n, q \geq 1$��</p>
<p>������ $q$ �У�ÿ�� $n$ ���������α�ʾ $b_1, \dots, b_n$����֤ $0 \leq b_1, \dots, b_n &lt; p$��</p>
<h2>�����ʽ</h2>
<p>�� $q$ �У�ÿ�жԸ����� $b_1, \dots, b_n$�������Ӧ�� $x_1, \dots, x_n$������ж�����������һ�鼴�ɡ�����޽���ô��һ��ֻ�����һ������ $-1$��</p>


<pre><code class="language-input1">3 1 0 2
1 0 0
1 2 3
</code></pre>


<pre><code class="language-output1">499122179 998244352 499122176
998244352 1 1
</code></pre>


<p>���ڵ�һ��ѯ�ʣ�Ҫ����ĵ�ʽΪ��</p>
<p>\begin{eqnarray}
\begin{cases}
x_1 + x_2 + x_3 &amp; \equiv &amp; 1 &amp; \pmod{p}\\
x_1 + 2x_2 + x_3 &amp; \equiv &amp; 0 &amp; \pmod{p}\\
x_1 + x_2 + 3x_3 &amp; \equiv &amp; 0 &amp; \pmod{p}
\end{cases}
\end{eqnarray}</p>
<h2>������</h2>
<p>�������������ء�</p>
<h2>������Լ��</h2>
<p>�����������ݣ�$nq \leq 3 \times 10^5$��$0 \leq c, d \leq 10^9$��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th>
<th>$n$</th>
<th>$q$</th>
<th>����</th>
</tr></thead><tbody><tr><td>1</td><td>$\leq 3$</td><td>$=1$</td><td>$c, d \leq 1000$</td></tr><tr><td>2</td><td rowspan="7">$\leq 100$</td><td>$=1$</td><td>$c = d$</td></tr><tr><td>3</td><td rowspan="2">$\leq 10$</td><td rowspan="2">��֤��Ψһ��</td></tr><tr><td>4</td></tr><tr><td>5</td><td rowspan="4">$\leq 1000$</td><td>$c = 1, d = 0$</td></tr><tr><td>6</td><td rowspan="3">��֤��Ψһ��</td></tr><tr><td>7</td></tr><tr><td>8</td></tr><tr><td>9</td><td rowspan="6">$\leq 1000$</td><td rowspan="3">$=1$</td><td rowspan="3">��֤��Ψһ��</td></tr><tr><td>10</td></tr><tr><td>11</td></tr><tr><td>12</td><td rowspan="3">$\leq 10$</td><td>$c = d$</td></tr><tr><td>13</td><td rowspan="2">��֤��Ψһ��</td></tr><tr><td>14</td></tr><tr><td>15</td><td rowspan="6">$\leq 10^5$</td><td rowspan="6">$\leq 3$</td><td rowspan="2">$c = 1, d = 0$</td></tr><tr><td>16</td></tr><tr><td>17</td><td>$c = d$</td></tr><tr><td>18</td><td rowspan="3">��</td></tr><tr><td>19</td></tr><tr><td>20</td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<h2>���</h2>
<p>��û�����⣬����ˮ�־�˻���ţ���̫�����Ҳ����Ҳ��ᣡ�����ɿ���ܵ��ˡ�</p>
<p>��ʦ���Ŵ���ˮ����ʧ�ı�Ӱ��̾�˿���˵����������Щ�˰���ÿ�������Щ��ˮ�⣬һ�������⣬�ܵò�֪����˭���졣��</p>
<p>��������ˮ�ְ�UOJ Round��C�����������������ĺ󵲷粣���ϣ�����Ӵ������˹������е���ȷ��ʽ��</p>
<h2>����</h2>
<p><a href="./20502/file/attachment.zip">������������</a></p>
