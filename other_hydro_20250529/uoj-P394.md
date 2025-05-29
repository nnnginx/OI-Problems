<p>�����СS��ð�����������Ũ�����Ȥ��Ϊ������򵥣�С S ֻ�о��� <strong>$1$ �� $n$ ������</strong>��ð������</p>
<p>�����Ƕ�ð��������㷨������</p>
<pre><code class="sh_cpp">input��һ������Ϊ n ������ p[1...n]
output��p�����Ľ����
for i = 1 to n do
    for j = 1 to n - 1 do
        if(p[j] &gt; p[j + 1])
            ���� p[j] �� p[j + 1] ��ֵ</code></pre>
<p>ð������Ľ�������������Ϊ�������̵�ִ�д���������֤������������һ���½��� $\frac{1}{2}\sum_{i=1}^{n}{|i-p_i|}$������$p_i$ ������ $p$ �е� $i$ ��λ�õ����֡�������֤������Ȥ�����Կ���ʾ��</p>
<h2>��Ŀ����</h2>
<p>СS��ʼרע���о�����Ϊ $n$ �������У����� ��������$=\frac{1}{2}\sum_{i=1}^{n}{|i-p_i|}$ �����У��ں����У�Ϊ�˷��㣬���ǰ��������������нС��á������У�������һ���룬���������е��׶಻�ࣿ���Ƿֲ����ܲ��ܼ���</p>
<p>СS��Ҫ����һ�������ĳ���Ϊ $n$ ������ $q$�������ֵ����ϸ���� $q$ �ġ��á������и������������������������������㣬ϣ����������������⣬���ǵ��𰸿��ܻ�ܴ����ֻ������𰸶� $998244353$ ȡģ�Ľ����</p>
<h2>�����ʽ</h2>
<p>�ӱ�׼����������ݡ�</p>
<p>�����һ�а���һ�������� $T$����ʾ����������</p>
<p>����ÿ�����ݣ���һ����һ�������� $n$, ��֤ $n \le 6 \times 10^{5}$��</p>
<p>������һ�л����� $n$ ������������Ӧ����Ŀ�����е� $q_i$����֤�������һ��$1$ �� $n$ �����С�</p>
<h2>�����ʽ</h2>
<p>�������׼�����</p>
<p>����� $T$ �У�ÿ��һ��������</p>
<p>����ÿ�����ݣ����һ����������ʾ�ֵ����ϸ���� $q$ �ġ��á������и����� 998244353 ȡģ�Ľ����</p>


<pre><code class="language-input1">1
3
1 3 2
</code></pre>




<pre><code class="language-output1">3
</code></pre>

<h4>����</h4>
<p>�ֵ���� $1~~3~~2$ ��������У����� $3~~2~~1$ ���ⶼ�ǡ��á������У��ʴ�Ϊ 3��</p>


<pre><code class="language-input2">1
4
1 4 2 3
</code></pre>




<pre><code class="language-output2">9
</code></pre>




<h2>������</h2>
<p>��<a href="./20799/file/attachment.zip">����Ŀ¼</a>�µ� <em>ex_3.in</em> �� <em>ex_3.ans</em>��</p>
<h2>������</h2>
<p>�����ǶԱ���ÿ�����Ե��input��ģ��˵����</p>
<p>�����������ݣ������� $T = 5$ (�������ܲ�����). </p>
<p>�� $n_{max}$ ��ʾÿ�������� $n$ �����ֵ��$\sum{n}$ ��ʾ�������ݵ� $n$ �ĺ͡�</p>
<div class="table-responsive"><table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th rowspan="1">���Ե�</th><th rowspan="1">$n_{max}=$</th><th rowspan="1">$\sum n\leq$</th><th rowspan="1">��������</th></tr></thead><tbody><tr><td rowspan="1">1</td><td rowspan="1">$8$</td><td rowspan="11">$5n_{max}$</td><td rowspan="11">$\text{��}$</td></tr><tr><td rowspan="1">2</td><td rowspan="1">$9$</td></tr><tr><td rowspan="1">3</td><td rowspan="1">$10$</td></tr><tr><td rowspan="1">4</td><td rowspan="1">$12$</td></tr><tr><td rowspan="1">5</td><td rowspan="1">$13$</td></tr><tr><td rowspan="1">6</td><td rowspan="1">$14$</td></tr><tr><td rowspan="1">7</td><td rowspan="2">$16$</td></tr><tr><td rowspan="1">8</td></tr><tr><td rowspan="1">9</td><td rowspan="1">$17$</td></tr><tr><td rowspan="1">10</td><td rowspan="2">$18$</td></tr><tr><td rowspan="1">11</td></tr><tr><td rowspan="1">12</td><td rowspan="1">$122$</td><td rowspan="5">$700$</td><td rowspan="1">$\forall i ~~q_i=i$</td></tr><tr><td rowspan="1">13</td><td rowspan="1">$144$</td><td rowspan="4">$\text{��}$</td></tr><tr><td rowspan="1">14</td><td rowspan="1">$166$</td></tr><tr><td rowspan="1">15</td><td rowspan="1">$200$</td></tr><tr><td rowspan="1">16</td><td rowspan="1">$233$</td></tr><tr><td rowspan="1">17</td><td rowspan="1">$777$</td><td rowspan="4">$4000$</td><td rowspan="1">$\forall i ~~q_i=i$</td></tr><tr><td rowspan="1">18</td><td rowspan="1">$888$</td><td rowspan="3">$\text{��}$</td></tr><tr><td rowspan="1">19</td><td rowspan="1">$933$</td></tr><tr><td rowspan="1">20</td><td rowspan="1">$1000$</td></tr><tr><td rowspan="1">21</td><td rowspan="1">$266666$</td><td rowspan="5">$2000000$</td><td rowspan="1">$\forall i ~~q_i=i$</td></tr><tr><td rowspan="1">22</td><td rowspan="1">$333333$</td><td rowspan="4">$\text{��}$</td></tr><tr><td rowspan="1">23</td><td rowspan="1">$444444$</td></tr><tr><td rowspan="1">24</td><td rowspan="1">$555555$</td></tr><tr><td rowspan="1">25</td><td rowspan="1">$600000$</td></tr></tbody></table></div> 

<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$512\texttt{MB}$</p>
<h2>��ʾ</h2>
<p>�����ǶԽ��������½��� $\frac{1}{2}\sum_{i=1}^{n}{|i-p_i|}$ ��֤����</p>
<p>�������Ͼ������ֵ��ƶ����������Ľ�������Ӧ�������������ƶ����ܾ��������������ڵ� $i$ ��λ�ã������ڳ�ʼ�����У����λ���ϵ������� $p_i$����ô������Ҫ����������ƶ����� $p_i$ ��λ���ϣ��ƶ��ľ����� $|i - p_i|$���Ӷ��ƶ����ܾ������ $\sum_{i=1}^n |i - p_i|$����ð������ÿ�λύ���������ڵ����֣�ÿ�ν�������ʹ�ƶ����ܾ���������� 2����� $\frac{1}{2}{\sum_{i=1}^{n}{|i-p_i|}}$ ��ð������Ľ����������½硣</p>
<p>���������е����ж��ﵽ���½磬������ $n=3$ ��ʱ�򣬿������� $3 ~~ 2~~1$, ������н���ð�������Ժ�Ľ��������� 3������ $\frac{1}{2}\sum_{i=1}^{n}{|i-p_i|}$ ֻ�� 2��</p>
<h2>����</h2>
<p><a href="./20799/file/attachment.zip">������������</a></p>
