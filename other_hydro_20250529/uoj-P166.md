<p>����һ��<strong>������</strong>��</p>
<p>����������ڴ�����������������������</p>
<p>���Ǹ�ÿֻ����һ���� $0$ ��ʼ��������š�</p>
<p>����������������Ƚ����ÿֻ����ֻ�ܴ洢һ�� $0$ �� $1$ ��ֵ�����ڵ� $i$ ֻ�������ֵ��Ϊ $v_i$��</p>
<p>�������б��С�� $2n$ �����飬���ǵ�ֵ��������������������� $2n$ ��ֵ���Կ��������롣</p>
<p>���Ǽ�
\begin{equation}
F(a,b,f) = \left \lfloor \frac{f}{2 ^ {2 a + b}} \right \rfloor \mod 2
\end{equation}</p>
<p>���ڱ�Ŵ��ڵ��� $2n$ ��ÿֻ���飬�����ı��Ϊ $i$ ��
����Ҫ����ָ���������� $a_i, b_i, f_i$ ($0 \le a_i &lt; i, 0 \le b_i &lt; i, 0 \le f_i &lt; 16$)����
\begin{equation}
v_i = F \left ( v_{a_i}, v_{b_i}, f_i \right ) = \left \lfloor \frac{f_i}{2 ^ {2 v_{a_i}  + v_{b_i} }} \right \rfloor \mod 2
\end{equation}
���ǳƵ� $i$ ֻ���������ڵ� $a_i$ �͵� $b_i$ ֻ���飨<strong>ע��$a_i$���Ե���$b_i$</strong>����</p>
<p>��������˼������� $F$ �����ӣ�</p>
<div class="table-responsive">
  <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>$a$</th><th>$b$</th><th>$F(a,b,14)$</th><th>$F(a,b,8)$</th><th>$F(a,b,6)$</th></tr></thead><tbody><tr><td>$0$</td><td>$0$</td><td>$0$</td><td>$0$</td><td>$0$</td></tr><tr><td>$0$</td><td>$1$</td><td>$1$</td><td>$0$</td><td>$1$</td></tr><tr><td>$1$</td><td>$0$</td><td>$1$</td><td>$0$</td><td>$1$</td></tr><tr><td>$1$</td><td>$1$</td><td>$1$</td><td>$1$</td><td>$0$</td></tr></tbody></table></div>

<p>һ��ʼ���� $0$ ʱ�̣������б��С�� $2n$ �������ֵ��ͬʱ��ȷ����
Ȼ�����ÿֻ��Ŵ��ڵ��� $2n$ �����飬
����ֵ�����������������ֵ��ȷ��֮��������ʼȷ����
�������������Ϣ���������
ÿֻ����ȷ������ֵ��Ҫ1Сʱ��ע���ֻ�������ͬʱȷ�����ǵ�ֵ����</p>
<p>������һ�����ӣ���id��ʾ��ţ�t��ʾ�������ֵ��ȷ����ʱ�䣬��ͷ��ʾ�����������ϵ��</p>
<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/166/king.jpg" alt="����" style="width:400px;"></p>
<p>���ǿ��԰ѱ��С�� $2n$ �������ֵ�������� $n$ λ�Ķ������� $\mathrm{A}, \mathrm{B}$��
���� $\mathrm{A} = (v_{n-1} \  v_{n-2} \  \cdots \  v_0)_2$��
$\mathrm{B} = (v_{2n-1} \  v_{2n-2} \  \cdots \  v_{n})_2$��
�������Ҫ�� $\mathrm{A}$ �� $\mathrm{B}$ ��һЩ���㣬�õ�һ�� $n$ λ����������
���� $n$ ֻ�����ʾ������</p>
<p>�������������Ҫ����������ȥ��ᣬ����ʹ�õ������������ʱ�䶼���ޡ�
������˵�������ʹ�� $\mathrm{M}$ ֻ���飬��Ҫ��˳��ָ�� $n$ ֻ���飬
�� $\mathrm{T}$ Сʱ�ڣ���ʹ�õ����������ֵ���ܱ�ȷ����
��ָ���� $n$ ֻ�����ֵ��ʾ�Ķ�������Ϊ�����������Ĵ𰸡�</p>
<p><strong>��Ϊ���������������������һ��UOJ����
��һ��ͨ�����һ�����Ե��ѡ�ֽ����һ��UOJ����
���û��ѡ��ͨ�����һ�����Ե㣬���һ���õ�������߷ֵ�ѡ�ֽ����һ��UOJ����</strong></p>
<h2>����</h2>
<p>����Ҫ��дһ������ <code>build_computer</code>�����������������������</p>
<ul><li><code>build_computer(task_id, n, M, T)</code><ul><li><code>task_id</code>: ��������</li>
<li><code>n</code>: �����$\mathrm{A}$��$\mathrm{B}$��λ��</li>
<li><code>M</code>: ���˱��С��$2n$������֮�⣬�����ʹ�õ��������Ŀ</li>
<li><code>T</code>: ��ʹ�õ����������ֵ��Ҫ��$\mathrm{T}$Сʱ�ڱ�ȷ��</li>
</ul></li>
</ul><p>����Ե���һ������ <code>add_flea(a, b, f)</code>��
��ʾ����һֻ���飬���ڵ� $i$ �ε��ã�
���ӵ�����ı��Ϊ$2n + i - 1$��
$a_{2n+i-1}, b_{2n+i-1}, f_{2n+i-1}$�ֱ�����Ϊ$a, b, f$��
Ȼ����������᷵��$2n + i - 1$��
������ܵ���$\mathrm{M}$�� <code>add_flea</code>��</p>
<p>�㻹��Ҫ��ÿ�� $[0, n-1]$ �е����� $i$ ���� <code>set_output</code> ���������԰�����˳����ã���
<code>set_output(i, id)</code> ��ʾ��������Ķ��������ĵ� $i$ λΪ���Ϊ $id$ �������ֵ��</p>
<h2>������</h2>
<div class="table-responsive">
  <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>��������</th><th>��Ҫ����ı��ʽ</th></tr></thead><tbody><tr><td>1</td><td>     $(\mathrm{A} + 1) \mod 2 ^ n$           </td></tr><tr><td>2</td><td>  $(\mathrm{A} + \mathrm{B}) \mod 2 ^ n$     </td></tr><tr><td>3</td><td> $(\mathrm{A} \times \mathrm{B}) \mod 2 ^ n$ </td></tr></tbody></table></div>

<p>�� $m$ Ϊ <code>add_flea</code> �ĵ��ô�����$t$ Ϊ���������ֵ��ȷ��������ʱ�̡�</p>
<div class="table-responsive">
  <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th><th>��������</th><th>��ֵ</th><th>$n$</th><th>$\mathrm{M}$</th><th>$\mathrm{T}$</th><th>��ע</th></tr></thead><tbody><tr><td>1 </td><td>1</td><td>1 </td><td>   $1$   </td><td>      $10000$    </td><td>    $10000$ </td><td> </td></tr><tr><td>2 </td><td>1</td><td>2 </td><td>   $2$   </td><td>      $10000$    </td><td>    $10000$  </td><td>  </td></tr><tr><td>3 </td><td>1</td><td>5 </td><td>  $256$  </td><td>      $10000$    </td><td>    $10000$  </td><td>  </td></tr><tr><td>4 </td><td>1</td><td>9 </td><td>$10^5$ </td><td>$5 \times 10^5$   </td><td> $50$  </td><td> �ò��Ե�÷�Ϊ$\min \left \{ \left \lfloor \frac{5 \times 10^5 - m}{20000} \right \rfloor, 9 \right \}$��  </td></tr><tr><td>5 </td><td>1</td><td>10</td><td> $10^5$</td><td> $1.5 \times 10^6$</td><td>    $30$  </td><td> �ò��Ե�÷�Ϊ$\min \left \{30-t, 10 \right \}$��  </td></tr><tr><td>6 </td><td>2</td><td>3 </td><td>   $2$   </td><td>      $10000$    </td><td>    $10000$</td><td>      </td></tr><tr><td>7 </td><td>2</td><td>6 </td><td>  $233$  </td><td>      $10000$    </td><td>    $10000$</td><td>      </td></tr><tr><td>8 </td><td>2</td><td>13</td><td>$10^5$ </td><td> $1.2 \times 10^6$</td><td>  $100$ </td><td> �ò��Ե�÷�Ϊ$\min \left \{ \left \lfloor \frac{1.2 \times 10^6-m}{30000} \right \rfloor, 13 \right \}$��     </td></tr><tr><td>9 </td><td>2</td><td>14</td><td>$10^5$ </td><td>  $5 \times 10^6$ </td><td>  $42$</td><td>�ò��Ե�÷�Ϊ$\min \left \{42-t, 14 \right \}$��          </td></tr><tr><td>10</td><td>3</td><td>4 </td><td>   $2$   </td><td>      $10000$    </td><td>    $10000$ </td><td>      </td></tr><tr><td>11</td><td>3</td><td>7 </td><td>  $233$  </td><td>      $10^6$     </td><td>  $10^6$ </td><td>      </td></tr><tr><td>12</td><td>3</td><td>8 </td><td>  $512$  </td><td>  $3 \times 10^6$ </td><td>  $255$   </td><td>    </td></tr><tr><td>13</td><td>3</td><td>17</td><td>  $1024$ </td><td>  $4 \times 10^6$ </td><td>  $94$    </td><td> �ò��Ե�÷�Ϊ$\min \left \{ \left \lfloor\frac{94-t}{2} \right \rfloor, 17 \right \}$��   </td></tr><tr><td>14</td><td>3</td><td>1 </td><td>  $1024$ </td><td>    $1920000$    </td><td> $288$   </td><td> <b>��һ��ͨ���ò��Ե��ѡ�ֽ����һ��UOJ����</b>  </td></tr></tbody></table></div>

<h2>ʵ��ϸ��</h2>
<p>����ֻ֧��C++��</p>
<p>��ֻ���ύһ��Դ�ļ�ʵ������������ <code>build_computer</code> ������������ѭ����������ͽӿڡ�</p>
<p>����Ҫ����ͷ�ļ� <code>king.h</code>��</p>
<pre><code class="sh_cpp">void build_computer(int task_id, int n, int M, int T);</code></pre>
<p>���� <code>add_flea</code> �� <code>set_output</code> �Ľӿ���Ϣ���¡�</p>
<pre><code class="sh_cpp">int add_flea(int a, int b, int f);
void set_output(int i, int id);</code></pre>
<h2>���ⷽʽ</h2>
<p>����ϵͳ���������¸�ʽ�����ݣ�</p>
<ol><li>��1�У���������</li>
<li>��2�У�$n, \mathrm{M}, \mathrm{T}$</li>
</ol><p>�������� <code>add_flea</code> �Ĵ������� $\mathrm{M}$��
����� <code>set_output</code>�Ĵ��������� $n$��
��û�ж� $[0, n-1]$ �е�ÿ��������Ϊ <code>set_output</code> �ĵ�һ���������� <code>set_output</code>��
��ĳ��򽫱���Ϊ��Incorrect����</p>
<p>�� <code>build_computer</code> ���غ������ $\mathrm{T}$ Сʱ�󣬴���һֻ�����ֵ��û��ȷ����������ϵͳ�����Incorrect����
�������ǽ������������������ļ�������в��ԣ�
������������������ݣ�����������ȷ������ϵͳ�������Correct�������������Incorrect����</p>
<p>�������ϵͳ��һ������ˡ�Correct������ڶ��н������ $m$ �� $t$��������������񡱣���������������Ĵ�����Ϣ��</p>
<p><a href="/faq">����ʽ���͵���Ŀ��ô���ز���</a></p>
<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$512\texttt{MB}$</p>
<p><strong>���κ�ʱ�򣬽�����ʹ�õ��ڴ涼���ᳬ��$128\texttt{MB}$����ѡ��������$384\texttt{MB}$�Ŀ����ڴ档</strong></p>
<h2>����</h2>
<p><a href="./20606/file/attachment.zip">����������������</a></p>
