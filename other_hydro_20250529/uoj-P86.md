<p>���� $p, n, l, r$������ $p$ ����������� $0$ �� $p - 1$ ������ֵ $a$��������� $l \le x \le r$ �� ${x \choose n} \equiv a \pmod{p}$ �� $x$ �ĸ����� $998244353$��$7 \times 17 \times 2^{23} + 1$��һ��������ȡģ��Ľ�������� ${x \choose n}$ �Ƕ���ʽϵ������ $x$ ������ѡ $n$ ���ķ�������</p>
<h2>�����ʽ</h2>
<p>һ���ĸ��Ǹ��������ֱ��ʾ $p, n, l, r$����֤ $l \le r$��</p>
<h2>�����ʽ</h2>
<p>$p$ �У��� $i$ �б�ʾ $a = i - 1$ ʱ�Ĵ𰸡�</p>


<pre><code class="language-input1">7 3 1 7
</code></pre>


<pre><code class="language-output1">3
1
0
1
1
0
1
</code></pre>


<p>${1 \choose 3} = {2 \choose 3} = 0 \equiv 0 \pmod{7}$</p>
<p>${3 \choose 3} = 1 \equiv 1 \pmod{7}$</p>
<p>${4 \choose 3} = 4 \equiv 4 \pmod{7}$</p>
<p>${5 \choose 3} = 10 \equiv 3 \pmod{7}$</p>
<p>${6 \choose 3} = 20 \equiv 6 \pmod{7}$</p>
<p>${7 \choose 3} = 35 \equiv 0 \pmod{7}$</p>
<p>��ģ $7$ ������ֵΪ$0$����������ֵΪ $1, 3, 4, 6$ �ĸ�һ����������������Ϊ����𰸡�</p>
<h2>������Լ��</h2>
<p>���� 10% �����ݣ�$n, l, r \le 1000$��</p>
<p>���� 20% �����ݣ�$n, l, r \le 100000$��</p>
<p>�������� 20% �����ݣ�$r - l \le 10000$��</p>
<p>�������� 30% �����ݣ�$p \le 1000$����ĳЩ���ݵ��� $p \le 100$��</p>
<p>���� 100% �����ݣ�$p \le 30000$��$l, r, n \le 10^{30}$��</p>
<p>����Ϊ���չ˱���������ͬѧ��������ڹ������ݡ�Ϊ���չ˲�֪���߾��ȵ�С���ѣ��ڸ������͵������о��ֲ���һЩ $l, r, n \le 10^{18}$ �����ݡ�</p>
<p><strong>ʱ�����ƣ�</strong>$2\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<h2>��Դ</h2>
<p>matthew99</p>
<h2>���</h2>
<p><a href="https://matthew99.blog.uoj.ac/blog/240">https://matthew99.blog.uoj.ac/blog/240</a></p>
<h2>����</h2>
<p><a href="./20526/file/attachment.zip">������������</a></p>
