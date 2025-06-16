<p>�����Ǹ�ϲ�������С����,��һ�������õ�������һ���޴�� $n$ �� $m$ �еľ����㲻�õ�������δ洢���������ɵ������������һ����������ʣ�
���� $F_{i,j}$ ����ʾ�����е� $i$ �е� $j$ �е�Ԫ�أ��� $F_{i,j}$ ��������ĵ���ʽ��</p>
<p>\begin{cases}
F_{1,1} &amp; = &amp; 1 \\
F_{i,j} &amp; = &amp; a \cdot F_{i,j - 1} + b &amp; j \neq 1 \\
F_{i,1} &amp; = &amp; c \cdot F_{i - 1,m} + d &amp; i \neq 1
\end{cases}</p>
<p>����ʽ�� $a, b, c, d$ ���Ǹ����ĳ�����
����������֪�� $F_{n,m}$ ��ֵ�Ƕ��٣�������������������ս�����ܴܺ���ֻ��Ҫ��� $F_{n,m}$ ���� $1000000007$ ��������</p>
<h2>�����ʽ</h2>
<p>����һ������������ $n, m, a, b, c, d$����������������</p>
<h2>�����ʽ</h2>
<p>��ʾ $F_{n,m}$ ���� $1000000007$ ��������</p>


<pre><code class="language-input1">3 4 1 3 2 6
</code></pre>


<pre><code class="language-output1">85
</code></pre>


<p>�����еľ���Ϊ��</p>
<p>\begin{equation}
\left(\begin{array}{cccc}
1 &amp; 4 &amp; 7 &amp; 10\\
26 &amp; 29 &amp; 32 &amp; 35\\
76 &amp; 79 &amp; 82 &amp; 85
\end{array}
\right)
\end{equation}</p>
<h2>������</h2>
<p>�������������ء�</p>
<h2>������Լ��</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th>
<th>���ݷ�Χ</th>
</tr></thead><tbody><tr><td>1</td><td>$1 \leq n, m \leq 10$��$1 \leq a, b, c, d \leq 1000$</td></tr><tr><td>2</td><td>$1 \leq n, m \leq 100$��$1 \leq a, b, c, d \leq 1000$</td></tr><tr><td>3</td><td>$1 \leq n, m \leq 10^3$��$1 \leq a, b, c, d \leq 10^9$</td></tr><tr><td>4</td><td>$1 \leq n, m \leq 10^3$��$1 \leq a, b, c, d \leq 10^9$</td></tr><tr><td>5</td><td>$1 \leq n, m \leq 10^9$��$1 \leq a = c \leq 10^9$��$1 \leq b = d \leq 10^9$</td></tr><tr><td>6</td><td>$1 \leq n, m \leq 10^9$��$a = c = 1$��$1 \leq b, d \leq 10^9$</td></tr><tr><td>7</td><td>$1 \leq n, m, a, b, c, d \leq 10^9$</td></tr><tr><td>8</td><td>$1 \leq n, m, a, b, c, d \leq 10^9$</td></tr><tr><td>9</td><td>$1 \leq n, m, a, b, c, d \leq 10^9$</td></tr><tr><td>10</td><td>$1 \leq n, m, a, b, c, d \leq 10^9$</td></tr><tr><td>11</td><td>$1 \leq n, m \leq 10^{1000}$��$a = c = 1$��$1 \leq b, d \leq 10^9$</td></tr><tr><td>12</td><td>$1 \leq n, m \leq 10^{1000}$��$1 \leq a = c \leq 10^9$��$1 \leq b = d \leq 10^9$</td></tr><tr><td>13</td><td>$1 \leq n, m \leq 10^{1000}$��$1 \leq a, b, c, d \leq 10^9$</td></tr><tr><td>14</td><td>$1 \leq n, m \leq 10^{1000}$��$1 \leq a, b, c, d \leq 10^9$</td></tr><tr><td>15</td><td>$1 \leq n, m \leq 10^{20000}$��$1 \leq a, b, c, d \leq 10^9$</td></tr><tr><td>16</td><td>$1 \leq n, m \leq 10^{20000}$��$1 \leq a, b, c, d \leq 10^9$</td></tr><tr><td>17</td><td>$1 \leq n, m \leq 10^{1000000}$��$a = c = 1$��$1 \leq b, d \leq 10^9$</td></tr><tr><td>18</td><td>$1 \leq n, m \leq 10^{1000000}$��$1 \leq a = c \leq 10^9$��$1 \leq b = d \leq 10^9$</td></tr><tr><td>19</td><td>$1 \leq n, m \leq 10^{1000000}$��$1 \leq a, b, c, d \leq 10^9$</td></tr><tr><td>20</td><td>$1 \leq n, m \leq 10^{1000000}$��$1 \leq a, b, c, d \leq 10^9$</td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20564/file/attachment.zip">������������</a></p>
