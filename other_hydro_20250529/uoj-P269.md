<p>$\pi\text{+}e$ �ڸ�������ѧ��ʱ����˯����Ȼ��ÿ�ο��Զ��� $AK$����������ͬ��Ҷ�Ӻ���Ĥ�ݡ�</p>
<p>ĳ�죬��ʦ�ڿ��Ͻ�����ֲ�����Ŀ��</p>
<pre><code>(2010���,18��)
ĳ����ÿ���������Ŀ��ĸ���p=1/3, �Ҹ�������Ľ���໥����, ����Ӱ�졣
��4���л��еĴ���ΪX, ��X����ѧ�����������ķ��
(�𰸣�4/3��8/9)</code></pre>
<p>��ʦ˵�������������ֲ����������� $np$��������� $np(1-p)$�����������Լ��κ��ȥ�㡣��</p>
<p>$\pi\text{+}e$ һ���и����⣬���ϴ����˾�������������������ĺڿƼ���ĸ�����󵼡�������׾ٵĽ����������⡣˳���Ҷ��Ҳ��������һ�¡�</p>
<p>2016����ٵ�ĳ�죬$\pi\text{+}e$ ͻȻ����������¡��������룬��ԭ���������ǿ��һ�£��������������ӣ�</p>
<p>��һ������ʽ���� $f(x)$����ߴ���Ϊ $x^m$������任 $Q$��</p>
<p>$$Q(f,n,x) = \sum_{k = 0}^{n}f(k){n\choose k}x^k(1 - x) ^{n - k}$$</p>
<p>���ڸ������� $f$ �� $n,x$���� $Q(f,n,x)\bmod 998244353$��</p>
<p>Ȼ����������֪���߿������ǻ���ܶ����̵ġ�$\pi\text{+}e$ �����Լ��Ѿ����ǵ���ô�õĺڿƼ��ˣ�����绰��Ҷ�ӣ�Ҷ��Ҳ˵���ǵ��ˡ�</p>
<p>���ܰ������</p>
<p>����ĳ��ԭ�򣬺��� $f$ �ɵ�ֵ��ʽ������������ $a_0,a_1,\cdots,a_m$ �� $m+1$ ������$f(x)=a_x$������֤���ú���Ψһ��</p>
<h2>�����ʽ</h2>
<p>��һ���������� $n,m,x$��������ǰ������</p>
<p>�ڶ��й� $m+1$ ����������ʾ $a_0,a_1,\cdots,a_m$��</p>
<h2>�����ʽ</h2>
<p>���һ��һ������ʾ�𰸣���� $998,244,353$ ȡģ��</p>


<pre><code class="language-input1">4 1 332748118
0 1
</code></pre>


<pre><code class="language-output1">332748119
</code></pre>


<p>ע�⵽ $332748118 \equiv \frac{1}{3} \pmod{ 998244353 }$, $332748119 \equiv \frac{4}{3} \pmod{ 998244353 }$, $f(x)=x$, ��Ŀ������ı��ʽΪ��</p>
<p>$$\sum_{k=0}^4 k{4\choose k}\left(\frac{1}{3}\right)^k\left(\frac{2}{3}\right)^{4-k}=\frac{4}{3}$$</p>
<p>�˼�Ϊ��Ŀ��ͷ����ֲ�������������ı��ʽ��</p>


<pre><code class="language-input2">4 3 12
0 1 8 27
</code></pre>



<pre><code class="language-output2">46704
</code></pre>


<p>������ɵ� $f(x)=x^3$</p>
<h2>������</h2>
<p>�������������ء�</p>
<h2>������Լ��</h2>
<p>�������еĲ��Ե㣬��֤ $1 \le n \le 10^{9},\ 1 \le m \le 2 \times 10^{4},\ 0\le a_i,x&lt; 998,244,353$��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th rowspan="1">���Ե�</th><th rowspan="1">$n \le$</th><th rowspan="1">$m \le$</th><th rowspan="1">��������</th></tr></thead><tbody><tr><td rowspan="1">1</td><td rowspan="1">$10^{2}$</td><td rowspan="1">$10^{2}$</td><td rowspan="2">$n=m$</td></tr><tr><td rowspan="1">2</td><td rowspan="1">$10^{3}$</td><td rowspan="1">$10^{3}$</td></tr><tr><td rowspan="1">3</td><td rowspan="1">$10^{4}$</td><td rowspan="3">$10^{2}$</td><td rowspan="4">��Լ��</td></tr><tr><td rowspan="1">4</td><td rowspan="1">$10^{5}$</td></tr><tr><td rowspan="1">5</td><td rowspan="1">$10^{6}$</td></tr><tr><td rowspan="1">6</td><td rowspan="12">$10^{9}$</td><td rowspan="1">$= 1$</td></tr><tr><td rowspan="1">7</td><td rowspan="2">$= 2$</td><td rowspan="1">$f(x)=x^2$</td></tr><tr><td rowspan="1">8</td><td rowspan="1">$f(x)=x^2-x$</td></tr><tr><td rowspan="1">9</td><td rowspan="1">$= 3$</td><td rowspan="10">��Լ��</td></tr><tr><td rowspan="1">10,11</td><td rowspan="1">$10$</td></tr><tr><td rowspan="1">12,13,14</td><td rowspan="1">$10^{2}$</td></tr><tr><td rowspan="1">15</td><td rowspan="1">$10^{3}$</td></tr><tr><td rowspan="1">16</td><td rowspan="1">$2,000$</td></tr><tr><td rowspan="1">17</td><td rowspan="1">$4,000$</td></tr><tr><td rowspan="1">18</td><td rowspan="1">$8,000$</td></tr><tr><td rowspan="1">19</td><td rowspan="1">$12,000$</td></tr><tr><td rowspan="1">20</td><td rowspan="1">$2 \times 10^{4}$</td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20698/file/attachment.zip">������������</a></p>
